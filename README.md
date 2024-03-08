# G-s-kanseri-tespiti
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


[1] Klemm M., Craddock I., Leendertz J., Preece A. ve Benjamin R., “Radar-based breast cancer detection using a hemi-spherical antenna  array experimental results”, IEEE Trans. Antennas  Propag., (2009), 57 (6), sayfa 1692–1704. 
[2]  Abbosh  A.,  “Early  breast  cancer  detection  using  Doppler  frequency  shift”,  Asia-Pacific  Microwave Conference Proceedings (APMC), Yokohama, (2010), sayfa 275-278. 
[3] Karabatak M., “Özellik seçimi, sınıflama ve  öngörü Uygulamalarına yönelik birliktelik kuralı Çıkarımı ve yazılım geliştirilmesi”, Ph.D. Thesis, Fırat University Institute of Science, Elazığ, (2008). 
[4] Nass S.,  Henderson I. ve Lashof  J., “Mammography  and  Beyond: Developing  Technologies for  the Early  Detection  of  Breast  Cancer”,  National  Cancer  Policy  Board,  National  Academy  Press,  USA, (2001). 
[5]  Arbacha  L.,  Stolpenb  A.  H.,  Berbaum  K.  S.,  Fajardo  L.  L.,  Reinhardt  J.  M.,  “Breast  MRI  lesion classification:  Improved  performance  of  human  readers  with  a  backpropagation  neural  networkcomputeraided computeraided diagnosis (CAD) system”, J Magnetic  Resonance Imaging, (2007),  25 (1), sayfa 89-95. 
[6]  Abdolmaleki  P., Buadu  L.D., ve Naderimanesh  H., “Feature  extraction  and  classification  of  breast cancer  on  dynamic  magnetic  resonance  imaging  using  artificial  neural  network”,  Elsevier,  Cancer Letters, (2001), 171 (2), sayfa 183-191. 
[7]  Fogel  D.  B.,  Wasson  E.C.,  Boughton  E.M.  ve  Porto  V.W.,  “A  step  toward  computerassisted mammography using  evolutionary programming  and  neural Networks”, Cancer  Letters, (1997), 119 (1), sayfa 93-97. 
[8] Revett K., Gorunescu F., Gorunescu M., El-Darzı E. ve Ene M., “A breast cancer diagnosis system: a combined approach using rough sets  and  probabilistic neural  Networks”, Computer as a tool  Eurocon 2005, Belgrade, (2005), pp. 1124- 1127. 
[9] Gorunescu M., Gorunescu F., ve Revett K., “Investigating a Breast Cancer Dataset Using a Combined Approach: Probabilistic Neural Networks and Rough Sets”, Proc. 3rd ACM International Conference on Intelligent Computing and Information Systems -ICICIS07, Cairo, Egypt, (2007), pp. 246-249. 
[10]  Hsiao  Y.H.,  Huang  Y.L.,  Liang  W.M., Kuo  S.J.  and  Chen  D.R.,  “Characterization  of  benign  and malignant solid breast masses: harmonic versus nonharmonic 3D power Doppler imaging”, Ultrasound Medicine & Biology, (2009), 35 (3), pp. 353-359.
[11] https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data
