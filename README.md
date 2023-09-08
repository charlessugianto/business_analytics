# business_analytics
Link tableau: https://public.tableau.com/views/Dashboard_CharlesSugianto/Dashboard?:language=en-US&:display_count=n&:origin=viz_share_link

Link youtube: abc.com

# 1. Background dan Tujuan Analisa
Sebuah perusahaan Shopping Mall menjalankan berbagai iklan dari Juli hingga November 2021. Mereka ingin mengurangi biaya iklan tanpa mengurangi hasilnya, jadi mereka perlu lebih pintar dalam iklan mereka. Mereka juga ingin tahu apakah iklan-iklan yang mereka jalankan menghasilkan keuntungan dan jenis iklan yang paling efektif. Terdapat 4 tujuan Analisa, yaitu sebagai berikut:
1.	Apakah campaign ini menghasilkan keuntungan?
2.	Di bulan mana perusahaan menghasilkan profit?
3.	Bagaimana performa iklan dalam meningkatkan produktivitas perusahaan di bulan yang profitable?

# 2. User Story Line dan User Flow
Pengguna dari dashboard ini adalah seorang manajer pemasaran. Pengguna ingin menilai kinerja setiap kampanye iklan yang diluncurkan dan menentukan apakah model kampanye tersebut berhasil, menguntungkan, dan perlu dipertahankan atau harus dievaluasi lebih lanjut.
Dashboard akan dibuat dengan menyajikan berbagai data seperti impresi, jumlah klik, tingkat klik (CTR), tingkat konversi, biaya iklan, pendapatan dari iklan, dan sebagainya. Dengan data ini, manajer dapat mengevaluasi efektivitas iklan dalam menarik perhatian calon pelanggan, mendorong kunjungan ke situs web perusahaan, dan menilai kinerja iklan tersebut
 
# 3. Dataset,Tools, dan Metrics
A.	Dataset: https://www.kaggle.com/datasets/marceaxl82/shopping-mall-paid-search-campaign-dataset
B.	Tools data cleaning: Jupyter Notebook
C.	Tools visualisasi: Tableau
Dataset tersebut memiliki 190 baris iklan yang ditampilkan dalam mesin pencari dengan tujuan untuk mengarahkan pengunjung ke situs web berdasarkan kata kunci yang dicari oleh pengguna. Rentang waktu kampanye ini adalah dari bulan Juli hingga November 2021. 

•	Ad Group: Kategori iklan.
•	Month: Bulan kampanye.
•	Impressions: Jumlah tampilan iklan kepada calon pengunjung.
•	Clicks: Jumlah klik yang diterima oleh iklan dari calon pengunjung.
•	CTR: Tingkat Klik, yaitu rasio klik dibandingkan dengan jumlah tampilan 
•	Conversions: Jumlah tindakan pembelian yang diambil oleh pengunjung.
•	Conv Rate: Tingkat Konversi, persentase pengunjung yang melakukan pembelian setelah mengklik iklan.
•	Cost: Biaya yang dikeluarkan oleh perusahaan untuk ad group tertentu.
•	CPC: Biaya Per Klik untuk mengevaluasi efektivitas kampanye dalam hal Return on Investment.
•	Revenue: Total pendapatan yang diperoleh dari iklan.
•	Sale Amount: Jumlah penjualan yang berasal dari suatu kelompok iklan.
•	P&L: Keuntungan atau kerugian yang dihasilkan dari kelompok iklan tertentu.

D.	Metrics
1.	Conversion Rate (Tingkat Konversi): Ini mengukur persentase pengunjung atau pelanggan potensial yang berubah menjadi pelanggan yang sebenarnya atau melakukan tindakan yang diinginkan, seperti membuat pembelian atau mengisi formulir.
2.	Cost Per Click (Biaya Per Klik): Ini adalah biaya yang dibayar oleh pengiklan setiap kali seseorang mengklik iklan mereka. Ini adalah salah satu cara pengukuran efisiensi kampanye periklanan.
3.	Revenue (Pendapatan): Ini adalah total uang yang diperoleh dari penjualan produk atau layanan. Revenue sangat penting dalam menilai keberhasilan bisnis.
4.	Cost Per Mile (Biaya Per Seribu Tampilan): Ini adalah biaya yang dibayar oleh pengiklan untuk menampilkan iklan mereka kepada seribu pemirsa potensial, terlepas dari apakah pemirsa mengklik iklan atau tidak.
5.	Impression (Tampilan): Ini mengacu pada jumlah kali iklan ditampilkan kepada pemirsa potensial. Ini dapat membantu pengiklan mengukur seberapa sering iklan mereka terlihat.
6.	Clicks (Klik): Ini adalah jumlah total kali pengguna mengklik iklan. Ini adalah metrik penting dalam mengukur seberapa menarik iklan bagi pemirsa.
7.	Conversion (Konversi): Ini merujuk pada tindakan yang diinginkan yang diambil oleh pengguna, seperti melakukan pembelian atau berlangganan newsletter, sebagai hasil dari interaksi dengan iklan atau situs web.
8.	Click Through Rate (Tingkat Klik): Ini adalah persentase pengguna yang mengklik iklan setelah melihatnya. Ini dihitung dengan membagi jumlah klik oleh jumlah tampilan, kemudian mengalikan dengan 100 untuk mendapatkan persentasenya.

# 4	Data Preparation
A.	Missing Value dan Duplicated Data
Hasil: Tidak ditemukan missing value dan duplikasi data
B.	Cek Tipe Data dan Ubah Tipe Data Ad Group
C.	 Group by kolom Ad Group
D.	Keterangan Cost per Mile dan Device
CPM diperhitungkan ke dalam tabel dataset untuk mengevaluasi biaya yang dikeluarkan untuk setiap 1000 tampilan iklan. Kolom "Ad Group" juga terdapat informasi tentang media yang digunakan dalam iklan tersebut.

# 5 Visualisasi
Pengguna dashboard memiliki kemampuan untuk meninjau kinerja iklan secara keseluruhan melalui metrik yang terlihat di bagian paling atas dashboard. Grafik garis akan memperlihatkan tren per bulan. Tambahan lagi, pengguna dapat melakukan analisis yang lebih terperinci terhadap performa masing-masing kelompok iklan, termasuk kesadaran merek, lalu lintas yang dihasilkan, dan penjualan yang dihasilkan. Selain itu, pengguna memiliki opsi untuk menyaring data berdasarkan bulan dan jenis perangkat.
 
# 6. Analisa
1.	Apakah campaign ini menghasilkan keuntungan?
Kampanye iklan yang dijalankan belum menghasilkan keuntungan yang memadai karena pendapatan yang diperoleh lebih kecil dari biaya pemasaran. Dalam berikutnya akan dilihat pada bulan Oktober yang memiliki profit tertinggi.

2.	Di bulan mana perusahaan menghasilkan profit?
Ketika bulan Oktober, perusahaan berhasil meraih keuntungan, maka dilakukan pendalaman terhadap iklan yang menunjukkan kinerja yang baik selama bulan tersebut.

3.	Bagaimana performa iklan dalam meningkatkan produktivitas perusahaan di bulan yang profitable?
Iklan Coupon mendapat impressi tertinggi, lebih signifikan daripada iklan Discount. Namun, jika kita lihat cost per mille-nya, iklan Discount lebih efisien daripada iklan Coupon dengan perbedaannya tidak terlalu jauh. Selain itu, sale akan lebih efesien daripada discount. Tidak hanya memberikan wawasan tentang efisiensi biaya per 1.000 tampilan iklan, tetapi juga membantu perusahaan dalam mengukur efektivitas kampanye mereka dalam mencapai target audiens, baik melalui CPM dan Convertion Rate.

# 7 Kesimpulan
Secara umum, perusahaan belum mendapatkan keuntungan dari kampanye iklan mereka, kecuali pada bulan Oktober. Pada bulan tersebut, iklan tipe Coupon dan Discount tampil sebagai pilihan terbaik dalam meningkatkan kesadaran merek, lalu lintas, dan penjualan. Dengan demikian, berdasarkan analisis saat ini, perusahaan dapat mempertimbangkan untuk lebih fokus pada iklan tipe Coupon dan Discount untuk menjawab kebutuhan Manajer Pemasaran dalam menghemat anggaran pemasaran tanpa mengurangi kinerja iklan. Namun, sebaiknya dilakukan analisis lebih mendalam terutama pada bulan-bulan dengan kerugian.

# 8 Referensi
Farris, P.W., Bendle, N., Pfeifer, P. and Reibstein, D., 2010. Marketing metrics: The definitive guide to measuring marketing performance. Pearson Education.
Ling-Yee, L., 2011. Marketing metrics' usage: Its predictors and implications for customer relationship management. Industrial Marketing Management, 40(1), pp.139-148.
Sampaio, C.H., Simões, C., Perin, M.G. and Almeida, A., 2011. Marketing metrics: Insights from Brazilian managers. Industrial Marketing Management, 40(1), pp.8-16.
