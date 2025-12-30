# Business Intelligence E-Commerce Analysis
Proyek ini merupakan analisis Business Intelligence berbasis data transaksi e-commerce yang bertujuan untuk mengubah data mentah menjadi insight bisnis yang dapat langsung digunakan untuk pengambilan keputusan.
Fokus utama proyek ini adalah memahami pola penjualan, perilaku pelanggan, profitabilitas produk, serta efektivitas proses pembelian melalui pendekatan analisis data dan visualisasi.

Proyek ini tidak hanya menampilkan grafik, tetapi juga menyajikan interpretasi bisnis dan rekomendasi strategis yang relevan bagi manajemen.

## Alur Kerja Analisis
Proyek ini mengikuti alur kerja Business Intelligence yang sistematis:
1. Data Integration & Cleaning (date formatting, handling missing values)
2. Exploratory Data Analysis (EDA)
3. Feature Engineering (Margin, DOI, Funnel Metrics)
4. Visual Analysis
5. Business Insight Extraction
6. Strategic Recommendation

## Pertanyaan Bisnis
1. Produk mana yang memiliki penjualan tertinggi sepanjang tahun 2024-2025? Adakah lonjakan ekstrem pada produk tertentu?
2. Bagaimana persebaran outlier untuk tiap produk kategori? Apa kaitan outlier dengan performa penjualan?
3. Seperti apa pola pembelian pelanggan dari tahap view hingga purchase?
4. Bagaimana insight terkait distribusi profit margin penjualan?
5. Bagaimana menentukan produk prioritas (unggulan) dan produk yang layak di-_drop_?

## Apa Keunggulan Projek Ini?
1. Visualisasi dalam projek ini dihubungkan langsung dengan masalah bisnis nyata, seperti produk tidak optimal, inefisiensi funnel pembelian, risiko _overstock_ / _understock_. Sehingga, perusahaan dapat menentukan strategi bisnis yang tepat dan _data-driven_.
2. Menghasilkan insight yang dapat ditindaklanjuti karena analisis menghasilkan rekomendasi konkret terkait strategi promosi, optimasi stok, prioritas pengelolaan produk.
3. Proyek ini berfokus pada impact bisnis, bukan hanya eksplorasi data.

## Tech Stack
+ Python (Pandas, NumPy)
+ Data Visualization (Matplotlib, Seaborn)
+ Feature Engineering
+ Analytical & Business Storytelling

## Apa Saja Insight yang Diperoleh?
**1. Analisis Sales Spike**
<p align="center">
  <img alt="Top 5 Sales Spike Detection"
       src="https://github.com/user-attachments/assets/66e6cb8b-618f-42f2-bf2c-99a048996328" width = '600'/>
  <br>
  <em>Figure 1. Lonjakan Penjualan pada Top 3 Produk</em>
</p>
Produk Sticky Notes DQLab mengalami lonjakan penjualan sangat signifikan pada September 2024, menjadi puncak tertinggi sepanjang periode pengamatan. Sebelum periode tersebut, penjualannya relatif rendah, kemudian meningkat tajam dan setelahnya tetap berada di level yang lebih tinggi dibandingkan kondisi awal.
Pola ini mengindikasikan keberhasilan suatu aktivitas bisnis seperti promosi besar, kampanye khusus, atau kontrak pembelian dalam jumlah besar. Sebaliknya, empat produk lainnya menunjukkan tren yang lebih stabil tanpa lonjakan ekstrem.

**Implikasi bisnis:** Pola ini menunjukkan bahwa strategi yang diterapkan pada Sticky Notes DQLab sangat efektif dan layak dievaluasi serta direplikasi untuk produk lain.
<br>
<br>

**2. Deteksi Outlier**
<p align="center">
  <img alt="Outlier Analysis by Product Name"
       src="https://github.com/user-attachments/assets/fc21ede2-429a-4c19-9a95-1f2fdf04857e" width = '600'/>
  <br>
  <em>Figure 2. Melihat Outliers dengan Boxplot tiap Kategori Produk</em>
</p>
Boxplot menunjukkan bahwa Earphone Kantor DQLab, Kertas Warna DQLab, dan Sticky Notes DQLab memiliki median penjualan lebih tinggi serta rentang interkuartil yang lebih lebar, menandakan performa yang lebih dinamis dibanding produk lain yang relatif stabil. Hampir semua produk juga memiliki outlier, yang menunjukkan adanya lonjakan penjualan di luar pola normal.

**Implikasi bisnis:** Lonjakan ini berpotensi berasal dari promo atau pembelian besar yang perlu dianalisis lebih lanjut untuk mengidentifikasi faktor pendorong utama performa produk.
<br>
<br>

**3. Analisis Funnel Conversion**
<p align="center">
  <img alt="Profit Margin Distribution"
       src="https://github.com/user-attachments/assets/a8d8398c-7894-4aa5-a01a-2478a260d6b4" width = '600'/>
  <br>
  <em>Figure 3. Funnel Chart tiap Tahap Pembelian</em>
</p>
Dari total 76,5 juta views, sebanyak 79% berhasil menjadi clicks, namun terjadi penurunan tajam pada tahap add_to_cart yang hanya mencapai 15%. Lebih jauh lagi, hanya sekitar 1% dari total views yang akhirnya menjadi purchase. Hal ini mengindikasikan bottleneck kritis antara tahap click dan add_to_cart yang sangat memengaruhi tingkat konversi akhir.

**Implikasi bisnis:** Optimalisasi pengalaman pengguna pada tahap ini berpotensi memberikan dampak besar terhadap peningkatan penjualan.
<br>
<br>

**4. Distribusi Profit Margin (%)**
<p align="center">
  <img alt="SKU Priority Classification Matrix"
       src="https://github.com/user-attachments/assets/09867194-0e8a-4174-a558-71a403cc61a4" width = '600'/>
  <br>
  <em>Figure 4. Distribusi Profit Margin (%)</em>
</p>
Distribusi profit margin menunjukkan variasi yang luas dengan konsentrasi utama di kisaran 10–25% dan sekitar 50%, serta beberapa kelompok produk di rentang 30–35% dan 60–70%. Kurva distribusi yang tidak simetris menunjukkan bahwa perusahaan memiliki beberapa segmen produk dengan tingkat profitabilitas yang berbeda.

**Implikasi bisnis:** Segmentasi produk berdasarkan margin menjadi penting untuk menyusun strategi harga, promosi, dan prioritas pengelolaan produk.
<br>
<br>

**5. Klasifikasi SKU Berdasarkan Margin dan DOI (khusus Bulan Oktober)**
<p align="center">
  <img alt="Customer Conversion Funnel"
       src="https://github.com/user-attachments/assets/6ce3282a-08f0-4a0a-9ccc-96c191c9890f" width = '600'/>
  <br>
  <em>Figure 5. Matriks Prioritas SKU Berdasarkan Margin dan DOI</em>
</p>
Matriks SKU menunjukkan bahwa Sticky Notes DQLab dan Earphone Kantor DQLab merupakan produk paling sehat secara bisnis karena memiliki margin tinggi dan Days of Inventory rendah, sehingga menghasilkan profit cepat tanpa membebani biaya penyimpanan. Sebaliknya, produk seperti Kartu Ucapan DQLab dan Tempat Kartu DQLab memang memiliki margin tinggi, namun tertahan pada Days of Inventory yang sangat besar, yang berarti modal tersimpan lama di gudang dan meningkatkan risiko biaya operasional. Temuan ini menunjukkan bahwa tidak semua produk bermargin tinggi layak menjadi prioritas, karena kecepatan perputaran stok (DOI) sama pentingnya dengan margin dalam menentukan profitabilitas nyata.
<br>
<br>

## Kesimpulan
**1. Produk dengan performa penjualan tertinggi**

Penjualan didominasi oleh sedikit produk utama, dengan Sticky Notes DQLab mengalami lonjakan ekstrem pada September 2024. Setelah puncak, performanya tetap lebih tinggi dibanding periode awal, menunjukkan potensi sebagai key revenue driver.

**2. Outlier & performa produk**

Hampir semua kategori produk memiliki outlier, yang mengindikasikan adanya event penjualan tidak normal seperti promo besar atau pesanan massal. Produk dengan median tinggi dan outlier ekstrem cenderung memiliki kontribusi penjualan yang lebih dinamis.

**3. Pola perilaku pelanggan (Funnel)**

Dari seluruh view, hanya 1% yang berakhir menjadi purchase. Drop-off terbesar terjadi pada tahap click → add_to_cart, menjadikannya titik kritis utama untuk optimasi konversi.

**4. Distribusi profit margin**

Profit margin tidak terdistribusi normal dan membentuk beberapa klaster nilai, menandakan adanya kelompok produk dengan struktur profitabilitas yang sangat berbeda. Ini menunjukkan bahwa pendekatan harga dan stok tidak bisa disamaratakan.

**5. Penentuan produk prioritas & kandidat drop**

Matriks Margin–DOI menunjukkan bahwa produk dengan margin tinggi & DOI rendah merupakan kandidat utama untuk produk unggulan. Sebaliknya, produk dengan DOI tinggi & margin rendah berpotensi menjadi beban inventory dan layak untuk dievaluasi atau dikurangi.

## Rekomendasi Bisnis
**1. Leverage momentum produk dengan lonjakan penjualan**

Produk seperti Sticky Notes DQLab yang menunjukkan spike penjualan ekstrem perlu diperlakukan sebagai growth driver, melalui strategi bundling, promo lanjutan, dan penempatan prioritas dalam campaign pemasaran agar performa pasca-puncak tetap terjaga.

**2. Optimalkan tahap add-to-cart dalam funnel konversi**

Penurunan tajam dari tahap click ke add-to-cart menunjukkan peluang besar untuk peningkatan revenue. Disarankan melakukan perbaikan UX halaman produk, pemberian promo kontekstual di keranjang, serta personalisasi rekomendasi produk.

**3. Reformulasi strategi portofolio produk berbasis Margin–DOI Matrix**

Fokuskan investasi stok dan promosi pada produk dengan kombinasi margin tinggi dan DOI relatif rendah, karena kelompok ini memberikan keseimbangan terbaik antara profitabilitas dan kecepatan perputaran inventori.

**4. Evaluasi produk dengan DOI ekstrem**

Produk dengan DOI sangat tinggi berpotensi mengikat modal terlalu lama. Untuk kategori ini diperlukan strategi diskon selektif, reposisi harga, atau penyesuaian volume produksi.

**5. Segmentasi strategi harga & inventory, bukan berbasis rata-rata umum**

Setiap kelompok produk memerlukan kebijakan yang berbeda. Pendekatan dapat dilakukan dengan melakukan segmentasi strategi harga berdasarkan cluster margin, bukan rata-rata umum, supaya tiap produk dapat strategi profitabilitas yang lebih tepat.
