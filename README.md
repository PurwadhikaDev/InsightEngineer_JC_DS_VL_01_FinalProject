# InsightEngineer_JC_DS_VL_01_FinalProject
## Marketing Strategy: Increasing Sales of IKEA by Predicting Price of Products
### by InsightEngineer ( JCDS VL_01 ) 

## Sekilas IKEA
IKEA adalah perusahaan yang bergerak di bidang furniture atau perabot rumah tangga dengan kantor pusat di Swedia. IKEA menjual beragam pilihan produk berkualitas dengan harga yang murah. Konsep penjualan IKEA juga mengusung pengantaran ke rumah atau membeli komponen agar dapat dirakit di rumah. Bahan produk IKEA juga terbuat dari kayu yang ramah lingkungan. Toko IKEA di Indonesia mengusung konsep wholesales seperti gudang sehingga dapat berfungsi menyimpan produk dalam kapasitas besar.
<br />
Prediksi harga produk yang tepat dapat meminimalkan penetapan harga yang terlalu rendah dan tinggi setelah dihitung dengan diskon, karakteristik produk serta volume produknya sehingga dapat memaksimalkan potensi penjualan produk melalui strategi pengaturan harga.
<br />
<p align="center">
<img src="https://user-images.githubusercontent.com/92136872/136832726-dba93177-fa47-47ed-9289-1fb65ab4b8cd.jpg"/>
</p>

## Problem
IKEA mempunyai beragam product untuk dijual. Semakin lama produk disimpan di gudang, semakin besar pula cost yang akan dikeluarkan oleh perusahaan. Sehingga perlu dilakukan strategi pemasaran salah satunya dengan menentukan harga product untuk meningkatkan penjualan IKEA.

## Problem Statement
Di dalam Proyek ini, Tim Insight Engineer akan menganalisis dataset IKEA Furniture sehingga dapat merekomendasikan harga produk yang tepat yang dapat dijual oleh Manajemen IKEA kepada masyarakat. (Bagaimana caranya untuk menentukan harga yang tepat dari sebuah product?)

## Objective
Penentuan harga produk yang tepat diharapakan dapat meningkatkan sales perusahaan dan secara tidak langsung reduce cost penyimpanan produk di gudang.

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
1. Data Cleaning & Exploratory Data Analysis (EDA)
<br /> A. Handle duplicate, inconsistent & missing data, outliers
<br /> B. Add new data
<br /> C. Check linearity
<br /> D. Check data correlation
<br /> E. Check data type, etc
2. Preprocessing
<br /> A. Binary encoding
<br /> B. Data scaling
<br /> C. Data transforming, etc
3. Modelling
<br /> A. Decide model benchmark
<br /> B. Model benchmark selection using performance evaluation
<br /> C. Hyperparameter tuning from selected benchmark model
<br /> D. Model comparison (model before & after tuning)
<br /> E. Slected final model
5. Conclusion & Recommendation
