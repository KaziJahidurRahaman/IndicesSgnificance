# Significance Analysis of Normalized Indices in Land Use and Land Class Classification in an Urban Landscape Using Google Earth Engine and Machine Learning

<p><i>The repository contains the code and output of the study "Significance Analysis of Normalized Indices in Land Use and Land Class Classification in an Urban Landscape Using Google Earth Engine and Machine Learning".</i></p>
<br> 
 
 ## 1. About the Study
<p>The study applies 3 ML/DL algorithms (Support Vector Machine, Random Forest, and Artificial Neural Network) to do 7 class Land Use Land Cover classification for the area of Phnom Penh in Cambodia.
The classes are- 
0 'Tree',
1 'RoadsAndPavements',
2 'SavannahGrassland',
3 'Building',
4 'Water', 
5 'AgriculturalLand', 
6 'BareLand'
</p>
<p>The algorithms are applied in 2 different combinations of Sentinel 2B dataset. One with only Bands 1, 2, 3, 4, 5, 6, 7, 8, 8A, 9, 11 and 12 of Sentinel dataset. The another contains these bands along with 4 additional bands namely, Normalized Difference Builtup Index(NDBI), Normalized Difference Vegetation Index(NDVI), Normalized Difference Water Index(NDWI), and Bare Soil Index(BSI).</p> 
<p>The objectives of this study includes understanding the impact of these indices on LULC classification, producing updated LULC maps. At the end, a new approach (hybrid) combining the outputs from the best models for each of the classes were proposed. This new approach shows the better accuracy then all other models attempted in the study.</p> 

## 2. Study Area
![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/388e1a6d-8cd8-41f5-8dc3-54473b501919)

## 3. General Workflow
![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/409c0039-ad95-4b7f-9c18-0df282911d41)

## 4. Outputs
### 4.1 The class wise and overall accuracies for SVM, RF and ANN with 2 datasets

![OA and class wise accuracies of the attempted models](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/7e9bf5d3-c89c-474f-af0e-85ea9dc5419c)


### 4.2 Impact of indices on classwise and OA

![Impact on accuracy due to the index’s incorporation](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/79c11a97-4b52-4456-94b2-bd193535c20b)

### 4.3 Confusion Metrices of the algorithms with both datasets
![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/b8960e15-721e-47f8-974e-c0f68a27eedd)

![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/30d84197-f5fe-403c-9bd5-7f417b021805)

![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/54729982-dc22-4239-bccd-cfda2c4c0bea)

### 4.4 Impact of the indices on time complexity of the models
#### 4.4.1 SVM's accuracy reduces with the indices, but computation time decreases significantly
![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/99bf3789-4fe6-493d-b790-f800aef97a76)

#### 4.4.2 RF and ANN gains accuracy when indices are added with data. But computation time increases
![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/1f99adaa-0ab2-4765-8154-9fc4ee7e422f)

#### 4.4.3 Learning Curves of ANN shows better ability to generalise when indices added
![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/619e7edf-549f-4fb6-be1f-8e1cf2d6c173)

### 4.5 Proposed new approach performance and comaing with previous 2 best models shows better performance
![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/173fc4bc-c626-45d6-9d3a-5610f48b0604)

![Comparison of class wise and overall accuracies of 2 best models(previous) and proposed new approach](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/5194c8f8-8284-4cc9-a4e6-45eec60b63be)

### 4.6 Classified LULC Maps
![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/9f1043e7-0812-4e65-85fc-f04d6799b4c9)

![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/873fb266-a224-4f28-b2d2-89fd080b6590)

![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/b378fc44-d145-4cb2-959d-29988f4b28f5)

![image](https://github.com/KaziJahidurRahaman/IndicesSignificanceLULC/assets/109986838/76900cdf-9466-49be-acf9-98fc373947e0)


## 5. Conclusion
<p>The study finds that, indices has diferring effects on various ML/DL algorithms, specially for DL algorithms, it improves the OA significantly. On the otherhand, it drops the accuracy of SVM algorithm, however, yet in this case, it significantly improves the computation complexity. As of the best algorithm to classiy the LULC is concerned, SVM with only the Band 1-12 is the opmtimal one. However, the newly proposed approach based best class wise models overtrumps the accuracy of SVM .</p>

##### [A detailed report of the task can be found in the report file. The classified outputs are availabale in the outputs folder].
