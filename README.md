Breast cancer is a leading cause of death among women [1, 2]. This type of cancer affects one in every eight women during their lifetime, while it is rarely observed in men. Breast cancer is a malignant tumor that develops in breast cells. Despite scientists' knowledge of factors contributing to the development of breast cancer, such as aging, genetic risk factors, family history, infertility, obesity, and more [3, 4], a comprehensive solution to eliminate the effects of these factors has not been achieved yet.

Early detection and localization of the tumor are crucial for reducing the mortality rate. X-ray mammography is the most widely used diagnostic tool for breast cancer screening. However, the use of X-rays for breast cancer detection has significant limitations [5]. In clinical reports, Artificial Neural Networks (ANNs) have been applied in breast cancer diagnosis using various features [6, 7]. Numerous studies in the literature have attempted to predict cancer diagnosis using ANNs, not only in breast cancer but also in various cancer types. ANNs have been combined with other intuitive methods to enhance their effectiveness. Fogel [8] trained neural networks using radioactive features and the patient's age for breast cancer detection. Revett [9] and Gorunescu [10] designed a medical decision support system for breast cancer based on a hybrid model involving rough sets and probabilistic neural networks. Hsiao conducted a training of an MLP classifier using vascular indices (harmonic and non-harmonic 3D power Doppler imaging) to determine whether breast tumors are benign or malignant.

The aim of this study is to analyze the diagnosis of breast cancer. The goal is to determine whether the tumor is benign or malignant in individuals diagnosed with breast cancer. This way, the crucial time loss in the diagnostic process will be eliminated, and the remaining time can be utilized for effective disease treatment.

The dataset used in the application was obtained from the Kaggle platform [11]. The dataset consists of 596 rows and 32 columns describing the shape and characteristics of the tumor. Class distribution: 357 benign, 212 malignant tumors. Columns:

ID number

Diagnosis (M = malignant, B = benign)

Ten real-valued features are computed for each cell nucleus:
a) Radius (mean of distances from the center to points on the perimeter)
b) Texture (standard deviation of gray-scale values)
c) Perimeter
d) Area
e) Smoothness (local variation in radius lengths)
f) Compactness (perimeter^2 / area - 1.0)
g) Concavity (severity of concave portions of the contour)
h) Concave points (number of concave portions of the contour)
i) Symmetry
j) Fractal dimension ("coastline approximation")

Mean, standard error, and "worst" (mean of three largest values) were calculated for each feature, resulting in 30 features. For example, mean radius is 3, mean area is 13, and worst radius is 23. All feature values were re-coded with four significant digits. Missing feature values: none Class distribution: 357 benign, 212 malignant. I modified the dataset to represent B (benign tumor) = 0, M (malignant tumor) = 1.

I applied the KNN algorithm to this dataset using artificial neural networks in the implementation. The reason for choosing these algorithms is to obtain good results from the dataset.
