# Week-13_Stage-1_Group-3_Finest-Professionals
**Summary Insight dari EDA**

**Univariate Analysis**
- Mayoritas pelanggan berada di rentang usia 30-40 tahun.
- Sebagian besar pelanggan memiliki saldo yang rendah.
- Pelanggan terakhir dikontak dipertengahan bulan.
- Pelanggan yang dikontak sebagian besar memiliki durasi singkat.
- Sebagian besar pelanggan dihubungi hanya beberapa kali selama periode kampanye.
- Mayoritas pelanggan belum pernah dihubungi sebelumnya.
- Pelanggan sebagian besar belum pernah dihubungi sebelum kampanye ini.
- Sebagian besar pelanggan memiliki pekerjaan di bidang blue-collar, manajemen, dan teknisi.
- Sebagian pelanggan sudah menikah.
- Mayoritas pelanggan memiliki pendidikan tingkat sekunder.
- Mayoritas pelanggan tidak memiliki catatan gagal pembayaran (default).
- Mayoritas pelanggan memiliki pinjaman rumah (housing loan) dan mayoritas juga tidak memiliki pinjaman (loan).
- Komunikasi dengan pelanggan sebagian besar dilakukan melalui telepon seluler (celular).
- Waktu pelaksanaan kampanye pemasaran terpusat di bulan Mei, dengan penyebaran yang signifikan pada bulan Juli dan Agustus.
- Mayoritas hasil dari kampanye pemasaran sebelumnya tidak diketahui.
- Mayoritas pelanggan tidak berlangganan produk/jasa yang ditawarkan dalam kampanye pemasaran tersebut.

**Multivariate Analysis**
- Mayoritas korelasi antar feature termasuk lemah (nilai korelasi kurang dari 0.3) kecuali pada feature previous dan pdays yang memiliki korelasi linear positif yang kuat.
- Semakin lama durasi kontak, semakin besar kemungkinan klien akan berlangganan deposito.
- Pada feature pdays dan previous salah satunya harus dihilangkan karena terdapat korelasi kuat diantara keduanya.
- Pelanggan paling banyak memiliki pekerjaan management.
- Pelanggan yang sudah menikah lebih banyak berlangganan deposito.
- Pelanggan dengan secondary education paling banyak berlangganan deposito.
- Pelanggan yang berlangganan deposito tidak memiliki kredit macet.
- Deposito paling banyak oleh pelanggan yang tidak memiliki pinjaman rumah.
- Pelanggan yang berlangganan deposito tidak memiliki pinjaman pribadi.
- Pelanggan lebih banyak menggunakan tipe cellular.
- Kontak paling banyak terjadi pada bulan Mei, yang juga menghasilkan jumlah pelanggan berlangganan deposito berjangka tertinggi dalam setahun.
- Hasil kampanye yang sukses memiliki tingkat rasio yang paling baik.

**Business Insight**
- Hanya 11,6% nasabah yang sudah membuka deposito berjangka. Artinya hanya ada 5.300 nasabah yang berlangganan, dan 40.055 lainnya belum berlangganan deposito.
- Rata-rata usia pelanggan/nasabah ialah berusia sekitar 30 sampai 40 tahun.
- Nasabah yang paling banyak membuka deposito berjangka berusia sekitar 30-40 tahun dan sudah menikah.
- Nasabah yang belum membuka deposit rata-rata berusia 30-40 tahun.
- Pelanggan yang memiliki housing loan (pinjaman rumah) cenderung tidak memilih untuk membuka deposito.
- Pelanggan yang tidak memiliki loan (pinjaman pribadi) lebih banyak yang mengambil deposito berjangka dibandingkan dengan pelanggan yang memiliki loan.

**Business Recomendation**
- **Segmentasi target**<br>
Data menunjukan bahwa pelanggan dalam rentang usia 30-40 tahun cenderung memiliki minat yang tinggi terhadap produk deposito. Kami merekomendasikan untuk melakukan segmentasi target yang lebih spesifik pada kelompok usia ini demi meningkatkan efektivitas kampanye pemasaran.
- **Fokus pada pelanggan yang tidak memiliki loan**<br>
Pelanggan yang tidak memiliki loan cenderung memiliki minat yang tinggi terhadap produk deposito. Hal tersebut bisa jadi karena mereka tidak memiliki beban keuangan, sehingga mereka bisa mengalokasikan dana pribadi mereka ke investasi, salah satunya deposito berjangka.
- **Fokus pada pelanggan yang tidak memiliki housing loan**<br>
Sama seperti pelanggan yang tidak memiliki pinjaman pribadi, kita dapat memberikan campaign terkait manfaat investasi sejak dini kepada pelanggan yang tidak memiliki housing loan. Harapannya, mereka bisa mengalokasikan uang yang mereka punya untuk berlangganan deposito berjangka di bank kita.
- **Personalisasi komunikasi**<br>
Jika dipetakan kembali, nasabah yang cenderung memiliki minat berlangganan deposito berjangka ialah mereka yang berusia 30-40 tahun, sudah menikah, tidak memiliki beban pinjaman. Untuk itu, kita dapat membuat campaign yang lebih personal, seperti:
<ol>
  - Campaign untuk memberikan awareness tentang pentingnya investasi sejak ini untuk mempersiapkan dana pendidikan untuk anak.<br>
  - Merekomendasikan deposito dengan bunga tinggi sebagai tabungan membeli rumah<br>
  - Menampilkan keunggulan deposito dibanding investasi lain
</ol>
