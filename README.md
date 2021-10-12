# InsightEngineer_JC_DS_VL_01_FinalProject
## Marketing Strategy: Increasing Sales of IKEA by Predicting Price of Products
### by InsightEngineer ( JCDS VL_01 ) 

## Sekilas IKEA
IKEA adalah perusahaan yang bergerak di bidang furniture atau perabot rumah tangga dengan kantor pusat di Swedia. IKEA menjual beragam pilihan produk berkualitas dengan harga yang murah. Konsep penjualan IKEA juga mengusung pengantaran ke rumah atau membeli komponen agar dapat dirakit di rumah. Bahan produk IKEA juga terbuat dari kayu yang ramah lingkungan. Toko IKEA di Indonesia mengusung konsep wholesales seperti gudang sehingga dapat berfungsi menyimpan produk dalam kapasitas besar.
<br /> <br />
Prediksi harga produk yang tepat dapat meminimalkan penetapan harga yang terlalu rendah dan tinggi setelah dihitung dengan diskon, karakteristik produk serta volume produknya sehingga dapat memaksimalkan potensi penjualan produk melalui strategi pengaturan harga.
<br />
<p align="center">
<img src="https://user-images.githubusercontent.com/92136872/136832726-dba93177-fa47-47ed-9289-1fb65ab4b8cd.jpg"/>
</p>

## Problem
IKEA mempunyai beragam product untuk dijual. Semakin lama produk disimpan di gudang, semakin besar pula cost penyimpanan dan pemeliharaan yang dikeluarkan oleh perusahaan. Sehingga perlu dilakukan strategi pemasaran salah satunya dengan menentukan harga produk yang tepat untuk meningkatkan penjualan IKEA.

Di dalam Proyek ini, Tim Insight Engineer akan menganalisis dataset IKEA Furniture sehingga dapat merekomendasikan harga produk yang tepat yang dapat dijual oleh Manajemen IKEA kepada masyarakat. (Bagaimana caranya untuk menentukan harga yang tepat dari sebuah product?)

## Objective
Penentuan harga produk yang tepat diharapkan dapat meningkatkan sales perusahaan dan secara tidak langsung mengurangi cost penyimpanan produk di gudang.

## Data
- Sumber data : https://www.kaggle.com/ahmedkallam/ikea-sa-furniture-web-scraping 

- Data tersebut merupakan hasil web scrapping dari IKEA Arab Saudi. Harga yang tertera dalam data set berdasarkan mata uang Saudi Riyals sebagaimana tercantum dalam website IKEA pada 4/20/2020.

- Berdasarkan data set yang diberikan, diketahui data-data yang ada dalam kolom data sebagai berikut:

| No | Column | Description |
| -- | ------ | ----------- |
| 1 | item_id | Nomor identitas unik dari setiap produk yang dijual oleh IKEA (sebagai unit analysis) |
| 2 | name | Nama dari sebuah produk |
| 3 | category | Jenis kategori dari produk |
| 4 | price | Harga produk yang dijual saat ini |
| 5 | old_price | Harga jual produk sebelumnya |
| 6 | sellable_online | Ketersediaan penjualan produk secara daring |
| 7 | link | Tautan alamat web untuk mengetahui penjelasan lebih lanjut terkait produk |
| 8 | other_colors | Ketersediaan pilihan warna pada produk |
| 9 | short_description | Penjelasan singkat mengenai produk, fungsi, dan kegunaannya |
| 10 | designer | Nama desainer yang membuat produk |
| 11 | depth | Kedalaman produk dalam cm |
| 12 | height | Tinggi produk dalam cm |
| 13 | width | Lebar produk dalam cm |


## Step
1. Exploratory Data Analysis (EDA)     [link to file](https://github.com/PurwadhikaDev/InsightEngineer_JC_DS_VL_01_FinalProject/blob/main/1_IE_IKEA_Product_Problem_Statement_Data_Understanding_EDA_dan_narasi.ipynb)
<br /> A. Check linearity
<br /> B. Check data correlation
<br /> C. Check data type, etc

2. Preprocessing (Data cleaning)     [link to file](https://github.com/PurwadhikaDev/InsightEngineer_JC_DS_VL_01_FinalProject/blob/main/2_IE_IKEA_Preprocessing_and_Methodology_Data_Analysis.ipynb)
<br /> A. Handle duplicates data
<br /> B. Handle inconsistent data
<br /> C. Hanlde missing data
<br /> D. Add/drop column, etc

3. Modelling & Conclusion   [link to file](https://github.com/PurwadhikaDev/InsightEngineer_JC_DS_VL_01_FinalProject/blob/main/3_IE_IKEA_Machine%20Learning%20Model_Conclusin%20dan%20Recommendation.ipynb)
<br /> A. Further data preparation (Binary encoding, handle outliers, etc)
<br /> B. Decide model benchmark
<br /> C. Model benchmark selection using performance evaluation
<br /> D. Hyperparameter tuning from selected benchmark model
<br /> E. Model comparison (model before & after tuning)
<br /> F. Selected final model

4. Result Analytics & Recommendation     [link to file](https://github.com/PurwadhikaDev/InsightEngineer_JC_DS_VL_01_FinalProject/blob/main/4_IE_IKEA_Result_Analytics.ipynb)

## Conclusion & Recommendation
Terdapat korelasi kuat antara dimensi besaran produk seperti depth (0,4), height (0,53), dan width (0,73) dengan harga. Jika 3 dimensi itu digabungkan menjadi volume, volume memiliki korelasi paling kuat dengan harga (0,78) berbanding dengan 3 dimensi lainnya. 
<p align="center"> <img src="https://user-images.githubusercontent.com/92136872/136909964-d270e69a-2474-40a2-b3a6-77baabbb7cc4.png"/>
</p>
<br/> Produk-produk yang memiliki volume besar dan rata-rata harga yang tinggi adalah produk berkategori Wardrobes, beds, sofas & armchairs. Selain itu, designer juga turut andil dalam mempengaruhi harga produk. Produk yang di desain oleh Niels Gammelgaard, S Lanneskog rata-rata berharga 4000-6000 SR.
<p align="center"> <img src="https://user-images.githubusercontent.com/92136872/136911266-7c2da24b-7e85-4cde-8e02-59a370aff2e5.png"/></p>
<p align="center"> <img src="https://user-images.githubusercontent.com/92136872/136912441-fdc7e68a-1103-4237-a1ef-134151426e08.png"/></p>

<br /> Keterjualan produk dengan harga yang tinggi juga lebih besar terdapat pada produk yang dijual secara online dan produk yang memiliki pilihan warna. Dimana rata-rata harga produk yang dijual secara online dan terdapat pilihan warna adalah 1500 SR, sedangkan produk yang tidak dijual online dan hanya ada pilihan satu warna memiliki harga rata-rata 1300 SR. **Oleh itu kami menyarankan kepada manajemen agar dapat menampilkan harga produk yang dijual dengan memperhatikan volume (depth, height, width) produk, kategori produk, keterjualan online dan ketersediaan pilihan warna, serta designer produk**. Harga produk yang ditampilkan dapat diberikan setelah dikurangi diskon atau dimarkup sesuai dengan karakteristik produk tersebut.
<br/><br/> Setelah dilakukan test terhadap model benchmark Mechine Learning untuk penentuan harga, Kneighbors Regressor & Random Forest Regressor menghasilkan nilai terbaik dibanding dengan model lainnya.
<p align="center"> <img src="https://user-images.githubusercontent.com/92136872/136913690-274528e3-10ad-4173-80a9-9a38dae69636.png"/></p>

<br/> Kemudian dilakukan proses hyperparamter tuning terhadap 2 model tersebut dan didapat hasil bahwa model Random Forest Regressor dengan parameter criterion = 'mse', n_estimators = 100, max_depth = 15, random_state = 42 menunjukan peningkatan yang cukup signifikan.
<p align="center"> <img src="https://user-images.githubusercontent.com/92136872/136915693-091fd0bd-9fe5-4c22-8f2d-88f27908a929.png"/></p>
<br/> Maka, model inilah yang kami jadikan sebagai "Selected Model".
<p align="center"> <img src="https://user-images.githubusercontent.com/92136872/136917571-2f3c0ab5-f66b-4105-8401-a5c218ca4457.png"/></p>

Model machine learning yang terpilih dapat menentukan perkiraan harga yang tepat atas suatu produk. Perkiraan harga tersebut dapat digunakan sebagai manajemen IKEA untuk menetapkan harga dan diskon produk sehingga pembeli dapat merasa diuntungkan ketika membeli produk IKEA. Namun, hasil akan lebih baik jika terdapat data yang berkaitan dengan penjualan tiap produk agar dapat dilakukan analisa lebih lanjut.

## Business Insight
Perusahaan harus lebih berhati-hati dalam menentukan harga terhadap product yang mempunyai karakteristik berikut:
1. Product yang termasuk dalam category Sofa & armchairs, Bookcases & shelving units, Beds dan Wardobes
2. Product yang tidak diketahui designernya
3. Product dengan ukuran kedalaman 40 - 55 cm
4. Product dengantinggi 74 - 83 cm, dan
5. Product dengan lebar 80 cm

<br/> Product dengan karakteristik diatas berpengaruh terhadap besarnya error dalam prediksi harga. Karena jika error prediksi harga besar (terlalu over price/under price), maka perusahaan akan mengalami kerugian.


## References
1. https://www.analyticsvidhya.com/blog/2021/05/feature-engineering-how-to-detect-and-remove-outliers-with-python-code/
2. https://www.analyticsvidhya.com/blog/2021/04/how-to-handle-missing-values-of-categorical-variables/
3. https://www.analyticsvidhya.com/blog/2018/08/k-nearest-neighbor-introduction-regression-python/
4. https://humansofdata.atlan.com/2018/03/when-delete-outliers-dataset/
5. https://www.pluralsight.com/guides/non-linear-regression-trees-scikit-learn
6. https://medium.com/@harsha_vardhan/price-prediction-challenge-a-real-world-case-study-using-machine-learning-ce8a0697b795
7. https://www.kaggle.com/lucchi/investigating-and-predicting-ikea-furniture
