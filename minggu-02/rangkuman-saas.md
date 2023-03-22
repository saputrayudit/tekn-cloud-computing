# Praktikum Teknologi Cloud Computing - Minggu 2

## 1. Perbedaan antara IaaS, SaaS, dan Paas

* **IaaS (infrastructure as a service)** ialah yang termudah dari semua kategori. Ini mengacu pada layanan berbasis cloud, seperti penyimpanan pay-as-you-go, jaringan, dan virtualisasi. Model ini menyediakan teknologi dan ruang lingkup yang sama dengan pusat data tradisional. Perbedaannya adalah kita tidak dapat secara fisik memelihara atau mengelolanya menggunakan solusi offline. IaaS membantu perusahaan membuat dan mengelola data mereka saat mereka berskala, membayar ruang server yang mereka gunakan untuk mengembangkan perangkat keras atau perangkat lunak. Contoh IaaS yaitu Amazon Web Services , Microsoft Azure dll.

* **SaaS (software-as-a-service)** merupakan perangkat lunak berbasis cloud yang tersedia untuk pembelian secara berlangganan. Ini sebagian besar digunakan untuk aplikasi yang membutuhkan akses web dan seluler. Produk SaaS tidak perlu diunduh dan diinstal pada perangkat individu. Sebagian besar dapat dijalankan langsung dari browser web. Harus diperhitungkan bahwa pelanggan tidak bertanggung jawab atas pembaruan perangkat keras dan perangkat lunak. Selain itu, dengan SaaS, vendor mengelola semua masalah teknis potensial, seperti data, middleware, server, dan penyimpanan. Ini memungkinkan bisnis untuk merasionalisasi pemeliharaan dan dukungan mereka. Contoh SaaS yaitu Google App Engine , Dropbox , JIRA dll.

* **PaaS (platform as a service)** mengacu pada layanan platform berbasis cloud yang memberi para pengembang kerangka kerja yang dapat mereka gunakan untuk membuat aplikasi khusus. Model ini menyediakan programmer dengan platform yang digunakan untuk membuat perangkat lunak yang dikirimkan melalui Internet. Semua server, penyimpanan, dan jaringan dapat dikontrol oleh bisnis atau penyedia pihak ketiga. PaaS membuat proses pengembangan, pengujian, dan penyebaran cepat, mudah, dan hemat biaya. Dibandingkan dengan SaaS, PaaS menyediakan platform untuk pembuatan perangkat lunak, bukan perangkat lunaknya. Contoh PaaS ialah Windows Azure & Google App Engine.
* perbedaan menurut gambar **Iaas** **SaaS** **PaaS**
![image](https://user-images.githubusercontent.com/79730184/225207295-056cb338-cff5-4f46-b623-4f086042e9ca.png)

## 2. SAAS (Software as a Service) Platform Architecture
![image](https://user-images.githubusercontent.com/79730184/225284115-8d065d18-e320-44d5-8e9e-1dd290f5c7d5.png)

SAAS (Software as a Service) atau dalam bahasa Indonesia dapat dikatakan sebagai Perangkat Lunak sebagai layanan adalah konsep model bisnis di mana suatu perusahaan menyediakan akses ke aplikasi perangkat lunak melalui internet sebagai layanan kepada pelanggan mereka. Dalam model ini, perusahaan penyedia perangkat lunak menangani semua hal yang terkait dengan pengembangan, pemeliharaan, dan pengoperasian aplikasi, sementara pelanggan hanya perlu membayar biaya berlangganan untuk menggunakan aplikasi tersebut.

Dalam konsep ini, pelanggan tidak perlu lagi membeli dan menginstal perangkat lunak pada komputer atau server mereka sendiri, karena semua pengolahan dan penyimpanan data dilakukan di server penyedia perangkat lunak. Ini memungkinkan pelanggan untuk mengakses aplikasi dari mana saja, selama mereka memiliki koneksi internet.

Contoh SaaS yang populer termasuk Dropbox, Google Apps, Salesforce, dan Slack. Konsep SaaS telah mengubah cara banyak perusahaan memanfaatkan perangkat lunak dan memberikan solusi yang lebih fleksibel dan hemat biaya untuk kebutuhan teknologi informasi mereka.
Ada dua varietas utama SaaS:
1. SaaS Vertikal
Perangkat Lunak yang menjawab kebutuhan industri tertentu (misalnya, perangkat lunak untuk industri kesehatan, pertanian, real estat, keuangan)
2. SaaS Horisontal
Produk yang berfokus pada kategori perangkat lunak (pemasaran, penjualan, alat pengembang, SDM) tetapi agnostik industri.
* ilustrasi pada bentuk gambar

![image](https://user-images.githubusercontent.com/79730184/225326824-6bc5962a-3bdb-46e6-a52e-62543560e981.png)

* Manfaat SAAS <br>
Perangkat lunak skala besar sebelumnya membutuhkan biaya, waktu, staf, dan anggaran yang signifikan untuk diterapkan di perusahaan besar, sehingga banyak organisasi kecil tidak dapat memanfaatkannya. Namun, model pengiriman perangkat lunak sebagai layanan (SaaS) telah mengubah hal ini dengan menghilangkan atau mengurangi komitmen sumber daya di muka. Integrasi dapat direncanakan dan dilaksanakan dengan upaya minimal, menciptakan interval waktu tersingkat untuk investasi TI yang besar. Vendor SaaS juga menawarkan "test drive" perangkat lunak mereka yang bebas risiko (dan seringkali gratis) selama jangka waktu tertentu sehingga memberikan pelanggan kesempatan untuk mencoba perangkat lunak sebelum membelinya. Hal ini membantu menghilangkan banyak risiko seputar pembelian perangkat lunak dan menawarkan peluang bagi organisasi dari semua ukuran untuk mengalihkan risiko akuisisi perangkat lunak serta memindahkan TI dari pusat biaya reaktif menjadi bagian perusahaan yang proaktif dan menghasilkan nilai.

* kesimpulan <br>
Dalam kesimpulannya, SaaS (Software as a Service) adalah model bisnis di mana suatu perusahaan menyediakan akses ke aplikasi perangkat lunak melalui internet sebagai layanan kepada pelanggan mereka. Model ini memungkinkan pelanggan untuk mengakses aplikasi dari mana saja dengan koneksi internet, tanpa harus membeli atau menginstal perangkat lunak pada komputer mereka sendiri. Perusahaan penyedia perangkat lunak bertanggung jawab atas pengembangan, pemeliharaan, dan pengoperasian aplikasi, sementara pelanggan hanya membayar biaya berlangganan untuk menggunakan aplikasi tersebut. Konsep SaaS telah mengubah cara banyak perusahaan memanfaatkan perangkat lunak dan memberikan solusi yang lebih fleksibel dan hemat biaya untuk kebutuhan teknologi informasi mereka.
## 3. SaaS (Software as a Service) Platform itecture.
![image](https://user-images.githubusercontent.com/79730184/226768160-c390a11f-dc13-45fe-aa6e-087b8da3e6ee.png)

**Kesederhanaan Aplikasi Arsitektur SaaS**

* Nilai Ekonomis
Model pembayaran biaya berlangganan bulanan atau tahunan memudahkan bisnis untuk menganggarkan, memasangkannya dengan nol biaya penyiapan infrastruktur, dan mudah untuk melihat bagaimana memilih menggunakan solusi SaaS dapat menghemat uang bisnis.

* Keamanan
Keamanan merupakan aspek penting dari solusi pengembangan perangkat lunak dan platform SaaS tidak berbeda. Sebagai konsumen aplikasi yang dirancang menggunakan SaaS, Anda tidak perlu mengkhawatirkan bagaimana data Anda dikunci. Itu disimpan dengan aman di cloud!
* Kesesuaian
Dengan penginstalan perangkat lunak tradisional, pembaruan dan tambalan terkadang membutuhkan banyak waktu dan uang. Ini terutama berlaku di perusahaan.

* Kemampuan Solusi SaaS
Platform SaaS memiliki beragam kemampuan. Apalagi jika digabungkan dengan penawaran cloud lainnya seperti IaaS (Infrastruktur sebagai Layanan) dan PaaS (Platform sebagai Layanan).

Teknologi cloud seperti Microsoft Azure memungkinkan Anda menyediakan server yang dapat menghosting situs web, database, dan banyak lagi.
Infrastruktur yang secara historis dipasang secara fisik di lokasi bisnis dan dijalankan oleh tim TI internal, kini dapat disediakan dari dasbor online hanya dengan beberapa klik mouse.
Solusi SaaS dapat digunakan untuk lingkungan ini dan, secara teori, menawarkan segala jenis layanan yang dapat dikembangkan sebagai aplikasi perangkat lunak yang dapat mencakup, namun tidak terbatas pada:

* Aplikasi kantor
* Email dan pesan instan
* Media sosial
* layanan Fintech
* Mengekspos API Pihak ke-3
* Keamanan dan otentikasi
* Pembelajaran mesin
* Kecerdasan buatan
* Layanan Lokasi
* Streaming data dan layanan pencarian

* Kurangnya kontrol dalam platform Arsitektur SaaS
Karena aplikasi SaaS dihosting di lingkungan SaaS vendor, Anda memiliki sedikit atau tidak ada kendali atas perangkat lunak yang Anda gunakan.Aplikasi internal atau lokal akan memberi bisnis Anda lebih banyak kontrol atas perilakunya, misalnya, aplikasi berbasis Windows mungkin memiliki lebih banyak opsi konfigurasi daripada aplikasi web biasa yang dikirimkan sebagai aplikasi SaaS.

* Ekosistem terbatas
Tidak dapat disangkal bahwa SaaS menjadi tren yang berkembang sebagai saluran distribusi perangkat lunak. Konon, masih banyak aplikasi yang tidak menawarkan versi yang dihosting.

* Pertunjukan
Aplikasi in-house, thick client, atau on-premise akan selalu berjalan lebih cepat daripada produk yang dikirimkan melalui internet.

* Kekhawatiran Data
Saat memilih produk SaaS, dan misalnya, dengan munculnya GDPR, bisnis harus memberi perhatian khusus dalam hal tempat implementasi SaaS menyimpan data di cloud. Setiap yurisdiksi memiliki kebijakan legislatifnya sendiri dan bertindak ketika data sensitif sedang diproses atau disimpan.

* Komponen Utama Platform SaaS
Bagian penting dalam mengembangkan produk SaaS terbaru Anda adalah menentukan komponen atau fitur utama mana yang diharapkan pengguna sebagai standar. Dapat dipahami bahwa fitur akan didorong oleh permintaan pasar dan komunitas pengguna, tetapi ada beberapa komponen utama yang diharapkan pengguna.

* Keamanan
Melindungi data pelanggan di platform SaaS Anda adalah yang paling penting, karena itu, produk SaaS Anda kemungkinan besar akan melayani ratusan, bahkan ribuan pengguna. Pastikan arsitektur SaaS Anda mempertimbangkan hal ini.

* Pribadi
Sementara keamanan berkaitan dengan penguncian pengguna dan data sensitif, privasi data adalah komponen penting lainnya yang harus dipertimbangkan oleh platform SaaS Anda. Dengan peraturan baru, seperti GDPR, bisnis menjadi lebih akuntabel dari sebelumnya untuk memastikan privasi pengguna dan data tetap terjaga.Dengan temuan dari KPMG yang menyatakan bahwa Privasi Data adalah atribut terpenting kedua, yang mereka cari di penyedia cloud, privasi merupakan komponen penting untuk dipertimbangkan saat merancang produk SaaS Anda sendiri.

* Kustomisasi dan Konfigurasi
Meskipun Anda mungkin dapat memberikan solusi SaaS out-of-the-box untuk sebagian besar konsumen yang dikirimkan dengan serangkaian fitur, antarmuka pengguna, dan fungsionalitas standar, perusahaan sering kali mengharapkan penyesuaian tambahan untuk menangani kasus penggunaan khusus untuk spesifik mereka. domain masalah.Mempertimbangkan ekstensibilitas untuk arsitektur SaaS Anda adalah komponen penting lainnya yang perlu Anda pertimbangkan. Anda dapat melakukannya dengan mengirimkan versi "label putih" dari produk SaaS Anda atau dengan menerapkan mekanisme plugin yang memungkinkan bisnis dan/atau pengembang memperluas solusi SaaS label putih Anda.
