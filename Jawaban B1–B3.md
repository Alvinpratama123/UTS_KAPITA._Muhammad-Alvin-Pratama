# JAWABAN STUDI KASUS B1–B3
## UTS KAPITA – Integritas Akademik dan Akuntabilitas Kerja Kelompok

### B1. Kaidah Pengakuan Sumber Kode dari Repositori Terbuka

Dalam kasus pengembangan aplikasi pencatatan persediaan koperasi mahasiswa, salah satu anggota kelompok menyalin potongan kode untuk modul autentikasi pengguna dari repositori terbuka tanpa mencantumkan asal kode dan informasi lisensinya. Tindakan tersebut tidak sesuai dengan prinsip integritas akademik karena menggunakan hasil karya pihak lain tanpa memberikan pengakuan yang semestinya.

Penggunaan kode dari repositori terbuka pada dasarnya diperbolehkan selama mengikuti ketentuan lisensi yang berlaku. Namun, kode yang tersedia secara publik tidak selalu berarti bebas digunakan tanpa persyaratan.

Kaidah pengakuan sumber yang harus diterapkan adalah:

1. **Mencantumkan sumber asli kode.** Tim harus menyebutkan asal kode yang digunakan agar dapat diketahui bahwa kode tersebut bukan sepenuhnya hasil pengembangan kelompok.
2. **Menghormati hak cipta dan lisensi.** Tim wajib memeriksa ketentuan lisensi repositori sebelum menggunakan atau memodifikasi kode.
3. **Memberikan atribusi secara jelas.** Pengakuan sumber dapat dicantumkan pada dokumentasi proyek, laporan, atau komentar kode yang relevan.
4. **Membedakan kode asli dan kode pihak ketiga.** Tim harus menjelaskan bagian kode yang dikembangkan sendiri dan bagian yang diambil atau dimodifikasi dari sumber luar.
5. **Menjaga transparansi.** Setiap penggunaan sumber eksternal harus dapat ditelusuri dan diverifikasi.

Informasi yang perlu dicantumkan dalam pengakuan sumber meliputi:

- Nama pembuat atau pemilik repositori.
- Nama proyek atau repositori asal.
- Alamat URL repositori.
- Jenis lisensi yang digunakan.
- Versi atau commit kode yang digunakan, apabila tersedia.
- Bagian kode yang diambil atau dimodifikasi.
- Tanggal akses sumber, jika diperlukan dalam format sitasi yang digunakan.

Apabila repositori tidak mencantumkan lisensi, tim tidak boleh langsung menganggap kode tersebut bebas digunakan. Tim perlu meminta izin kepada pemilik kode atau menggunakan sumber lain yang memiliki izin penggunaan yang jelas.

Dengan demikian, penggunaan kode pihak ketiga harus dilakukan secara transparan dan mengikuti ketentuan lisensi agar tidak menimbulkan pelanggaran hak cipta maupun integritas akademik.

---

### B2. Peran Pembagian Tugas sebagai Dasar Akuntabilitas Kontribusi

Pembagian tugas yang tercatat merupakan bagian penting dalam kerja kelompok karena menjadi dasar untuk mengetahui tanggung jawab dan kontribusi setiap anggota. Dalam kasus ini, catatan kerja tim hanya memuat nama anggota tanpa menjelaskan tugas yang dikerjakan. Akibatnya, muncul perbedaan pendapat mengenai siapa yang sebenarnya mengembangkan modul autentikasi pengguna.

Pembagian tugas yang jelas dapat membantu kelompok menentukan tanggung jawab masing-masing anggota, memantau perkembangan pekerjaan, dan melakukan evaluasi berdasarkan bukti yang tersedia.

Beberapa manfaat pencatatan pembagian tugas adalah:

1. **Memperjelas tanggung jawab.** Setiap anggota mengetahui pekerjaan yang harus diselesaikan.
2. **Meningkatkan akuntabilitas.** Kontribusi anggota dapat diperiksa berdasarkan tugas dan hasil pekerjaannya.
3. **Mencegah konflik.** Catatan pekerjaan dapat digunakan sebagai bukti ketika terjadi perbedaan pendapat.
4. **Mempermudah evaluasi.** Dosen dapat menilai kontribusi berdasarkan hasil pekerjaan yang dapat diverifikasi.
5. **Meningkatkan transparansi.** Seluruh anggota dapat mengetahui perkembangan proyek dan pembagian pekerjaan.

Dalam pengembangan aplikasi koperasi mahasiswa, pembagian tugas dapat dibuat sebagai berikut:

| Peran | Tanggung jawab | Bukti kontribusi |
|---|---|---|
| Pengembang frontend | Membuat antarmuka aplikasi | Kode antarmuka dan riwayat commit |
| Pengembang backend | Mengembangkan autentikasi dan logika sistem | Kode backend dan pull request |
| Pengelola database | Merancang struktur dan relasi database | Skema database dan dokumentasi |
| Penguji dan dokumentator | Menguji fitur serta menyusun laporan | Test case dan riwayat revisi laporan |

Tabel tersebut merupakan contoh pembagian tugas yang dapat diterapkan, bukan bukti bahwa pembagian tugas tersebut sudah dilakukan oleh tim dalam kasus.

Apabila pembagian peran tidak tercatat, dampaknya adalah sulit menentukan siapa yang bertanggung jawab terhadap suatu pekerjaan, munculnya klaim kontribusi yang tidak dapat dibuktikan, serta risiko penilaian yang tidak adil.

Oleh karena itu, tim perlu menggunakan catatan tugas, riwayat Git commit, pull request, dokumentasi, dan laporan perkembangan pekerjaan. Bukti tersebut perlu diperiksa bersama karena jumlah commit saja tidak selalu menggambarkan besarnya kontribusi seseorang.

Dengan pencatatan yang baik, kontribusi setiap anggota dapat dipertanggungjawabkan secara objektif dan proses penilaian menjadi lebih adil.

---

### B3. Langkah Menjaga Integritas Akademik dalam Laporan Akhir

Dalam kasus ini, ketua tim mengusulkan agar bagian kode yang berasal dari sumber luar dihapus dari laporan supaya terlihat bahwa seluruh kode merupakan hasil karya kelompok. Ketua tim juga mengusulkan agar kontribusi seluruh anggota dinyatakan sama rata, meskipun terdapat perbedaan pekerjaan yang dilakukan.

Usulan tersebut tidak sesuai dengan prinsip integritas akademik karena dapat menimbulkan informasi yang tidak benar mengenai sumber kode dan kontribusi anggota kelompok.

Sebagai anggota tim, tindakan yang seharusnya dilakukan adalah sebagai berikut.

**1. Menolak penyembunyian sumber kode pihak ketiga**

Tim harus menolak usulan menghilangkan informasi sumber kode dengan tujuan membuatnya terlihat sebagai karya sendiri. Kode yang berasal dari repositori terbuka harus tetap diakui dan dicantumkan sumber serta lisensinya.

Apabila penggunaan kode tidak sesuai dengan ketentuan lisensi, tim harus memperbaiki kepatuhan lisensi, meminta izin, atau mengganti kode dengan implementasi yang memiliki izin penggunaan yang sesuai.

**2. Melakukan pemeriksaan terhadap kode yang digunakan**

Tim perlu meninjau kembali seluruh kode program untuk mengetahui bagian yang dibuat sendiri dan bagian yang berasal dari pihak ketiga.

Pemeriksaan dapat dilakukan melalui riwayat Git, dokumentasi, dan perbandingan dengan repositori sumber.

Hasil pemeriksaan tersebut kemudian dicatat agar asal kode dapat ditelusuri.

**3. Membuat laporan kontribusi berdasarkan bukti**

Setiap anggota harus menyerahkan catatan pekerjaan yang benar-benar dilakukan.

Bukti kontribusi dapat berupa:

- Riwayat Git commit dan pull request.
- Dokumentasi fitur yang dikembangkan.
- Riwayat revisi laporan.
- Hasil pengujian sistem.
- Catatan rapat dan pembagian tugas.

Apabila terdapat anggota yang tidak memiliki bukti kontribusi, tim perlu meminta klarifikasi sebelum melakukan penilaian.

**4. Menolak pernyataan kontribusi sama rata apabila tidak sesuai fakta**

Kontribusi anggota tidak boleh dinyatakan sama rata hanya untuk menghindari konflik atau menjaga nilai kelompok.

Setiap anggota harus memperoleh pengakuan sesuai pekerjaan yang benar-benar dilakukan dan dapat dibuktikan.

Jika terdapat perbedaan pendapat, tim dapat melakukan diskusi bersama dan meminta arahan dosen agar penilaian tetap objektif.

**5. Memperbaiki laporan akhir secara transparan**

Laporan akhir harus mencantumkan sumber kode pihak ketiga, informasi lisensi, pembagian tugas, dan kontribusi masing-masing anggota secara benar.

Dokumentasi juga harus menjelaskan proses pengembangan dan hasil pekerjaan secara jujur agar laporan dapat diperiksa oleh dosen.

**6. Menerapkan prinsip yang sama dalam proposal Tugas Akhir**

Hasil evaluasi kasus ini dapat dijadikan pedoman dalam penyusunan proposal Tugas Akhir. Setiap referensi jurnal, dokumentasi teknologi, dan kode pihak ketiga yang digunakan harus diakui sumbernya.

Sebagai contoh, dalam pengembangan aplikasi pemesanan dan validasi tiket Bus Trans Citra Raya berbasis QR Code, penggunaan teknologi seperti React Native dan Laravel harus disertai dokumentasi sumber yang relevan serta kepatuhan terhadap lisensi perangkat lunak yang digunakan.

Hasil pengembangan dan pengujian juga harus dilaporkan berdasarkan bukti yang benar-benar diperoleh, bukan berdasarkan hasil yang dibuat-buat.

**Kesimpulan B3**

Tim harus mengutamakan kejujuran, transparansi, dan tanggung jawab dalam menyusun laporan akhir. Usulan menyembunyikan sumber kode dan menyatakan kontribusi sama rata tanpa dasar yang benar harus ditolak.

Setiap sumber kode perlu diakui sesuai ketentuan lisensi, sedangkan kontribusi anggota harus dilaporkan berdasarkan bukti pekerjaan yang dapat diverifikasi. Dengan demikian, laporan akhir dapat memenuhi prinsip integritas akademik dan dipertanggungjawabkan kepada dosen.

---

## Kesimpulan Umum Studi Kasus B1–B3

Berdasarkan studi kasus pengembangan aplikasi pencatatan persediaan koperasi mahasiswa, dapat disimpulkan bahwa integritas akademik memiliki peran penting dalam proses pengembangan perangkat lunak secara berkelompok.

Penggunaan kode dari repositori terbuka harus disertai pengakuan sumber dan kepatuhan terhadap lisensi. Pembagian tugas harus dicatat secara jelas agar kontribusi setiap anggota dapat diperiksa. Selain itu, laporan akhir harus disusun berdasarkan fakta dan bukti yang dapat diverifikasi.

Penerapan prinsip tersebut dapat mencegah plagiarisme, mengurangi konflik antarangggota, dan meningkatkan akuntabilitas kerja kelompok. Prinsip yang sama juga perlu diterapkan dalam penyusunan proposal Tugas Akhir agar proses penelitian dan pengembangan sistem dilakukan secara jujur, transparan, dan bertanggung jawab.
