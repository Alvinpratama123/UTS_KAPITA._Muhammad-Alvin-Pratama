# JAWABAN ESSAY UTS KAPITA
## Aspek Hukum Digital, Etika Profesi, dan Integritas Akademik

### A1. Hukum Digital dan Etika Profesi

Dalam pengembangan aplikasi antrean layanan fasilitas publik, terdapat dua permasalahan yang perlu diperhatikan, yaitu pengumpulan data identitas dan riwayat kunjungan pengguna untuk dianalisis serta penggunaan modul perangkat lunak dari repositori terbuka tanpa mencantumkan informasi lisensinya.

**1. Ketentuan hukum digital yang relevan**

a. **Undang-Undang Nomor 27 Tahun 2022 tentang Pelindungan Data Pribadi (UU PDP).**

UU PDP mengatur perlindungan data pribadi dalam proses pengumpulan, penggunaan, penyimpanan, dan pengelolaan informasi individu. Dalam kasus ini, tim wajib memastikan bahwa pengumpulan data identitas dan riwayat kunjungan memiliki dasar pemrosesan yang sah, tujuan yang jelas, serta perlindungan keamanan yang memadai. Data pengguna tidak boleh digunakan di luar tujuan yang telah ditentukan tanpa dasar yang sah.

b. **Undang-Undang Nomor 28 Tahun 2014 tentang Hak Cipta.**

Undang-undang ini memberikan perlindungan terhadap karya cipta, termasuk program komputer. Penggunaan modul dari repositori perangkat lunak terbuka tetap harus mengikuti ketentuan lisensi yang diberikan oleh pemiliknya. Oleh karena itu, tim tidak boleh menganggap bahwa seluruh kode open source bebas disalin tanpa kewajiban atribusi atau ketentuan lainnya.

**2. Prinsip etika profesi yang relevan**

a. **Kerahasiaan (Confidentiality).**

Pengembang harus menjaga kerahasiaan data identitas dan riwayat kunjungan pengguna. Informasi tersebut hanya boleh diakses oleh pihak yang memiliki kewenangan sesuai kebutuhan pekerjaan.

b. **Tanggung jawab profesional (Professional Responsibility).**

Setiap pengembang bertanggung jawab terhadap hasil pekerjaannya, termasuk memastikan keamanan sistem, menghormati hak kekayaan intelektual, dan mematuhi ketentuan penggunaan perangkat lunak pihak ketiga.

**3. Hubungan hukum dan etika dengan tindakan tim**

Pengumpulan data tanpa memperhatikan dasar pemrosesan dan perlindungan data dapat menimbulkan pelanggaran terhadap ketentuan UU PDP serta bertentangan dengan prinsip kerahasiaan. Sementara itu, penggunaan kode pihak ketiga tanpa memenuhi ketentuan lisensi dapat melanggar hak cipta dan menunjukkan kurangnya tanggung jawab profesional.

**4. Solusi**

Tim perlu menjelaskan tujuan pengumpulan data, memastikan dasar pemrosesan yang sah, menerapkan pembatasan akses, dan menjaga keamanan penyimpanan data. Selain itu, tim harus memeriksa lisensi setiap modul yang digunakan, mencantumkan atribusi sesuai ketentuan, serta menyimpan informasi lisensi dalam dokumentasi proyek.

---

### A2. Hak Akses Informasi, Privasi Data, dan Lisensi

Pada soal ini terdapat dua kasus yang memiliki permasalahan berbeda, yaitu kelemahan pengendalian akses pada sistem informasi kelurahan dan penggunaan dataset publik yang memiliki batasan lisensi nonkomersial untuk melatih model kecerdasan buatan komersial.

**1. Kasus pertama: Akses data warga melalui perubahan parameter URL**

Permasalahan terjadi ketika warga dapat melihat data warga lain hanya dengan mengubah parameter pada alamat halaman web. Kondisi tersebut menunjukkan adanya kelemahan pengendalian akses pada aplikasi.

Potensi pelanggaran yang terjadi meliputi:

- **Hak akses informasi:** pengguna dapat mengakses informasi yang sebenarnya bukan menjadi hak atau kewenangannya.
- **Privasi data:** data pribadi warga berpotensi diketahui atau digunakan oleh pihak yang tidak berwenang.
- **Keamanan informasi:** sistem tidak melakukan pemeriksaan otorisasi secara memadai pada setiap permintaan data.

Penyebab teknisnya kemungkinan adalah aplikasi hanya melakukan pemeriksaan akses pada tampilan antarmuka, tetapi tidak memvalidasi hak akses pengguna pada sisi server. Kondisi ini dapat berkaitan dengan kerentanan Insecure Direct Object Reference (IDOR).

Usulan mitigasi:

a. Menerapkan autentikasi dan otorisasi pada setiap permintaan data.

b. Menggunakan Role-Based Access Control (RBAC) untuk membatasi akses berdasarkan peran pengguna.

c. Melakukan validasi kepemilikan data pada sisi server sehingga pengguna hanya dapat mengakses data yang menjadi kewenangannya.

d. Menerapkan pencatatan aktivitas akses (audit log) untuk membantu mendeteksi aktivitas mencurigakan.

e. Melakukan pengujian keamanan secara berkala untuk menemukan kelemahan akses informasi.

**2. Kasus kedua: Penggunaan dataset nonkomersial untuk AI komersial**

Permasalahan terjadi ketika tim menggunakan dataset publik untuk melatih model kecerdasan buatan yang akan dikembangkan secara komersial, padahal lisensi dataset hanya mengizinkan penggunaan nonkomersial.

Potensi pelanggarannya adalah penggunaan dataset yang tidak sesuai dengan ketentuan lisensi. Walaupun dataset dapat diakses secara publik, bukan berarti seluruh penggunaannya diperbolehkan untuk tujuan komersial.

Penyebabnya dapat berupa kurangnya pemeriksaan terhadap ketentuan lisensi, kurangnya dokumentasi sumber dataset, serta ketidaktahuan tim mengenai perbedaan penggunaan komersial dan nonkomersial.

Usulan mitigasi:

a. Memeriksa ketentuan lisensi sebelum menggunakan dataset.

b. Menghentikan penggunaan dataset untuk tujuan komersial apabila lisensinya tidak mengizinkan.

c. Meminta izin kepada pemilik dataset apabila penggunaan komersial memerlukan persetujuan tambahan.

d. Mengganti dataset dengan sumber lain yang memiliki lisensi yang mengizinkan penggunaan komersial.

e. Mendokumentasikan sumber, pemilik, dan ketentuan lisensi setiap dataset yang digunakan.

**Kesimpulan A2:** Kedua kasus menunjukkan bahwa akses terhadap informasi dan dataset tidak berarti seseorang bebas menggunakannya tanpa batas. Pengembang harus memperhatikan hak akses, privasi data, keamanan sistem, dan ketentuan lisensi yang berlaku.

---

### A3. Pengelolaan Data dan Lisensi dalam Proyek Aplikasi Kesehatan

Dalam proyek kelompok yang mengembangkan aplikasi pendataan layanan kesehatan di tingkat komunitas, tim harus memperhatikan perlindungan data pribadi karena sistem mengelola informasi identitas dan data kesehatan pengguna. Selain itu, penggunaan beberapa pustaka pihak ketiga dengan lisensi berbeda juga harus dikelola secara bertanggung jawab.

Rancangan penanganan data dan lisensi dapat dilakukan melalui beberapa tahapan berikut.

**1. Klasifikasi data**

Tim perlu mengelompokkan data berdasarkan tingkat kerahasiaan dan risiko penyalahgunaannya.

- Data identitas: nama, alamat, dan informasi identitas pengguna.
- Data kesehatan: riwayat kesehatan, hasil survei kesehatan, dan informasi kondisi kesehatan pengguna.
- Data operasional: informasi aktivitas aplikasi dan riwayat penggunaan sistem.

Data kesehatan termasuk data pribadi yang bersifat spesifik menurut UU PDP sehingga memerlukan perlindungan yang lebih ketat.

**2. Dasar persetujuan dan pembatasan akses**

Sebelum mengumpulkan data, tim harus memberikan penjelasan mengenai tujuan pengumpulan, jenis data yang digunakan, dan pihak yang dapat menerima data tersebut.

Pemrosesan data harus memiliki dasar yang sah sesuai ketentuan UU PDP. Apabila menggunakan persetujuan sebagai dasar pemrosesan, persetujuan harus diberikan secara jelas dan dapat dibuktikan.

Pembatasan akses dilakukan berdasarkan tugas dan kewenangan masing-masing pengguna. Contohnya:

- Petugas kesehatan hanya dapat mengakses data yang diperlukan untuk menjalankan tugasnya.
- Administrator bertanggung jawab mengelola akun dan konfigurasi sistem.
- Mitra eksternal hanya dapat menerima data sesuai tujuan dan kewenangan yang telah ditetapkan.

Tim juga perlu menerapkan autentikasi, otorisasi, enkripsi, dan pencatatan aktivitas akses.

**3. Pengelolaan lisensi kode pihak ketiga**

Setiap pustaka atau kode program pihak ketiga yang digunakan harus diperiksa lisensinya sebelum diintegrasikan ke dalam aplikasi.

Tim perlu membuat daftar inventaris yang berisi:

- Nama pustaka atau library.
- Sumber atau pemilik perangkat lunak.
- Jenis lisensi.
- Ketentuan penggunaan dan distribusi.
- Kewajiban atribusi atau pemberitahuan lisensi.

Contohnya, apabila tim menggunakan library dengan lisensi MIT, tim harus memenuhi ketentuan lisensi tersebut, termasuk mempertahankan pemberitahuan hak cipta dan teks lisensi yang diwajibkan.

**4. Prosedur penanganan insiden kebocoran data**

Apabila terjadi kebocoran data, tim harus melakukan langkah-langkah berikut:

a. Mengidentifikasi sumber kebocoran dan jenis data yang terdampak.

b. Membatasi akses yang tidak sah dan mengamankan sistem yang mengalami gangguan.

c. Mengamankan bukti digital seperti log aktivitas dan catatan akses untuk keperluan investigasi.

d. Melaporkan insiden kepada pihak yang berwenang dan memberikan pemberitahuan tertulis kepada subjek data serta pihak terkait sesuai ketentuan UU PDP. UU PDP mengatur pemberitahuan kegagalan pelindungan data pribadi paling lambat 3 x 24 jam dalam kondisi yang diatur undang-undang.

e. Melakukan evaluasi penyebab kebocoran dan memperbaiki kelemahan keamanan.

f. Meningkatkan prosedur pengamanan agar insiden serupa tidak terulang.

**Kesimpulan A3:** Pengelolaan data kesehatan harus dilakukan secara hati-hati melalui klasifikasi data, dasar pemrosesan yang sah, pembatasan akses, dan prosedur penanganan insiden. Penggunaan kode pihak ketiga juga harus mengikuti ketentuan lisensi masing-masing.

---

### A4. Integritas Akademik dalam Kerja Kelompok

Integritas akademik merupakan prinsip kejujuran, tanggung jawab, keadilan, dan penghargaan terhadap hasil karya orang lain dalam kegiatan akademik. Dalam pengembangan solusi informatika secara berkelompok, setiap anggota harus mencantumkan sumber referensi yang digunakan serta memperoleh pengakuan berdasarkan kontribusi pekerjaannya.

**1. Contoh penerapan pengakuan sumber**

Dalam pengembangan aplikasi pemesanan tiket bus, kelompok menggunakan dokumentasi resmi Laravel dan React Native sebagai referensi dalam proses pengembangan sistem.

Penerapan pengakuan sumber dilakukan dengan mencantumkan referensi dokumentasi tersebut pada laporan atau daftar referensi. Apabila kelompok menggunakan kode program dari repositori pihak ketiga, kelompok juga harus mencantumkan atribusi dan memenuhi ketentuan lisensi yang berlaku.

Dengan demikian, penggunaan sumber dari pihak lain tidak dianggap sebagai hasil karya asli kelompok tanpa pengakuan.

**2. Contoh pembagian peran yang tepat**

Dalam suatu proyek pengembangan aplikasi, pembagian tugas dapat dilakukan sebagai berikut:

- Anggota pertama: bertanggung jawab terhadap pengembangan frontend aplikasi.
- Anggota kedua: bertanggung jawab terhadap pengembangan backend dan integrasi API.
- Anggota ketiga: bertanggung jawab terhadap perancangan database dan pengelolaan data.
- Anggota keempat: bertanggung jawab terhadap pengujian sistem dan dokumentasi hasil pengujian.

Setiap anggota harus menyelesaikan tugas sesuai tanggung jawabnya dan mendokumentasikan hasil pekerjaan agar kontribusinya dapat diperiksa.

**3. Contoh pelanggaran integritas akademik**

Contoh pelanggaran adalah seorang anggota kelompok menyalin kode program atau isi laporan dari internet tanpa mencantumkan sumber, kemudian mengakuinya sebagai hasil pekerjaan sendiri.

Tindakan tersebut termasuk plagiarisme karena menggunakan karya orang lain tanpa memberikan pengakuan yang semestinya.

Pelanggaran lainnya adalah mengakui pekerjaan anggota lain sebagai hasil pekerjaan pribadi atau memalsukan laporan kontribusi kelompok.

**4. Cara penanganan**

Penanganan dilakukan dengan memeriksa sumber kode dan dokumen yang digunakan, meminta klarifikasi kepada anggota yang bersangkutan, serta memperbaiki atribusi atau sitasi yang belum dicantumkan.

Jika pelanggaran terbukti, kelompok perlu melakukan evaluasi dan melaporkannya kepada dosen apabila diperlukan. Pembagian tugas dan riwayat pekerjaan juga harus didokumentasikan agar setiap kontribusi dapat dipertanggungjawabkan.

**Kesimpulan A4:** Integritas akademik dalam kerja kelompok dapat diwujudkan melalui kejujuran dalam penggunaan sumber, penghargaan terhadap hak cipta, pembagian peran yang jelas, serta tanggung jawab terhadap hasil pekerjaan masing-masing anggota.

---

### A5. Penilaian Kontribusi Anggota Kelompok

Penilaian kontribusi anggota dalam proyek kelompok harus dilakukan secara objektif berdasarkan catatan pekerjaan dan bukti hasil yang dapat diverifikasi. Penilaian tidak boleh hanya berdasarkan pendapat pribadi atau kedekatan antaranggota.

Berdasarkan kasus, terdapat tiga kondisi anggota kelompok, yaitu satu anggota mengerjakan sebagian besar kode program, anggota lainnya menyusun dokumentasi, dan satu anggota tidak tercatat memberikan kontribusi dalam riwayat kerja maupun artefak proyek.

**1. Kerangka penilaian kontribusi**

Penilaian dapat dilakukan menggunakan beberapa aspek berikut:

a. **Kontribusi pengembangan kode**

Bukti yang diperiksa meliputi riwayat Git commit, pull request, perubahan kode, dan hasil implementasi fitur.

b. **Kontribusi dokumentasi**

Bukti yang diperiksa meliputi riwayat revisi dokumen, penyusunan laporan, dokumentasi teknis, dan hasil penulisan.

c. **Kontribusi pengujian**

Bukti yang diperiksa meliputi test case, hasil pengujian, laporan kesalahan, dan dokumentasi perbaikan sistem.

d. **Kontribusi perencanaan dan koordinasi**

Bukti yang diperiksa meliputi catatan rapat, pembagian tugas, diskusi kelompok, dan penyelesaian pekerjaan yang telah disepakati.

**2. Contoh matriks penilaian kontribusi**

| Aspek | Bukti yang dapat diverifikasi |
|---|---|
| Pengembangan kode | Git commit, pull request, dan hasil implementasi |
| Dokumentasi | Riwayat revisi dan dokumen laporan |
| Pengujian | Test case dan hasil pengujian |
| Koordinasi | Catatan rapat dan riwayat diskusi |
| Penyelesaian tugas | Daftar pekerjaan dan hasil akhir |

Penilaian dapat menggunakan skala 0–100 berdasarkan rubrik yang disepakati kelompok dan dosen. Bobot setiap aspek harus ditentukan terlebih dahulu agar penilaian dilakukan secara konsisten.

**3. Analisis kontribusi masing-masing anggota**

- Anggota pertama yang mengerjakan sebagian besar kode program harus memperoleh pengakuan berdasarkan hasil implementasi, perubahan kode, dan kualitas pekerjaan yang dapat dibuktikan.
- Anggota kedua yang menyusun dokumentasi harus memperoleh pengakuan berdasarkan hasil penyusunan laporan dan riwayat revisi dokumen.
- Anggota ketiga yang tidak memiliki catatan kontribusi perlu dimintai klarifikasi terlebih dahulu. Kelompok harus memberikan kesempatan untuk menunjukkan bukti pekerjaan yang mungkin belum terdokumentasi.

**4. Cara menangani anggota tanpa bukti kontribusi**

Kelompok tidak boleh langsung memberikan penilaian buruk tanpa melakukan pemeriksaan. Langkah yang perlu dilakukan adalah:

a. Memeriksa seluruh riwayat pekerjaan melalui GitHub, dokumen, dan catatan tugas.

b. Meminta anggota yang bersangkutan menjelaskan pekerjaan yang telah dilakukan.

c. Memberikan kesempatan untuk menunjukkan hasil pekerjaan atau menyelesaikan tugas yang masih diperlukan.

d. Melakukan penilaian berdasarkan bukti yang tersedia dan rubrik yang telah disepakati.

e. Mendokumentasikan hasil evaluasi secara transparan dan melaporkan kondisi tersebut kepada dosen apabila diperlukan.

**Kesimpulan A5:** Penilaian kontribusi anggota kelompok harus didasarkan pada bukti pekerjaan yang nyata dan dapat diverifikasi. Anggota yang mengembangkan kode, menyusun dokumentasi, melakukan pengujian, maupun menjalankan tugas lainnya harus memperoleh pengakuan sesuai kontribusinya. Prinsip keadilan, transparansi, dan tanggung jawab harus diterapkan dalam proses penilaian.

---

## Kesimpulan Umum A1–A5

Berdasarkan pembahasan A1 sampai A5, dapat disimpulkan bahwa pengembangan solusi informatika tidak hanya berfokus pada keberhasilan teknis suatu aplikasi, tetapi juga harus memperhatikan aspek hukum digital, etika profesi, perlindungan data pribadi, kepatuhan lisensi perangkat lunak, dan integritas akademik.

Setiap pengembang memiliki tanggung jawab untuk menjaga kerahasiaan informasi pengguna, membatasi akses data sesuai kewenangan, menghormati hak cipta, serta memastikan penggunaan sumber dan kode pihak ketiga dilakukan sesuai ketentuan.

Selain itu, dalam kerja kelompok diperlukan pembagian peran yang jelas dan penilaian kontribusi berdasarkan bukti pekerjaan yang dapat diverifikasi. Dengan menerapkan prinsip tersebut, proses pengembangan sistem informasi dapat berjalan secara bertanggung jawab, transparan, aman, dan sesuai dengan ketentuan yang berlaku.
