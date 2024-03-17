<h1>Week-13_Stage-1_Group-3_Finest-Professionals</h1>
<h2>Summary Insight dari EDA**</h2>

<h3>I. Descriptive Statistics</h3>
<h4>A. Terdapat tipe data atau nama kolom dan isinya yang sesuai dan kurang kurang sesuai:</h4>
<ul>
  <li>Tipe data untuk kolom yang sudah sesuai (age, balance, day : tipe data int64 atau float64; job, marital, education, default, housing, loan, contact, month, poutcome, y : tipe data object).</li>
  <li>Tipe data pada kolom duration, campaign, pdays, dan previous dapat diubah dari float64 menjadi int64 karena kolom-kolom tersebut seharusnya berisi nilai-nilai bilangan bulat, bukan bilangan desimal.</li>
</ul>

<h4>B. Terdapat kolom yang memiliki nilai kosong:</h4>
<ul>
  <li>duration: Kolom ini memiliki 346 nilai null.</li>
  <li>campaign: Kolom ini memiliki 382 nilai null.</li>
  <li>pdays   : Kolom ini memiliki 217 nilai null.</li>
  <li>previous: Kolom ini memiliki 268 nilai null.</li>
  <li>y       : Kolom ini memiliki 308 nilai null.</li>
</ul>
<h4>C. Terdapat kolom yang memiliki nilai summary agak aneh:</h4>
<ul>
  <li>Nilai minimum pada pdays -1, yang menunjukkan bahwa beberapa nasabah mungkin belum pernah dihubungi sebelumnya.</li>
  <li>Dengan menghapus baris yang memiliki nilai kolom "pdays" -1, kami dapat memfokuskan analisis pada subset data yang lebih spesifik pada nasabah yang telah dihubungi sebelumnya.</li>
  <li>Beberapa kolom numerik skew (dilihat dari perbedaan yang besar antara mean dan median) seperti balance, duration, campaign, pdays dan previous</li>
  <li>Terdapat indikasi outlier pada kolom balance, duration, campaign, pdays dan previous</li>
</ul>

<h3><strong>Univariate Analysis</strong></h3>
<ul>
  <li>Mayoritas pelanggan berada di rentang usia 30-40 tahun.</li>
  <li>Sebagian besar pelanggan memiliki saldo yang rendah.</li>
  <li>Pelanggan terakhir dikontak dipertengahan bulan.</li>
  <li>Pelanggan yang dikontak sebagian besar memiliki durasi singkat.</li>
  <li>Sebagian besar pelanggan dihubungi hanya beberapa kali selama periode kampanye.</li>
  <li>Mayoritas pelanggan belum pernah dihubungi sebelumnya.</li>
  <li>Pelanggan sebagian besar belum pernah dihubungi sebelum kampanye ini.</li>
  <li>Sebagian besar pelanggan memiliki pekerjaan di bidang blue-collar, manajemen, dan teknisi.</li>
  <li>Sebagian pelanggan sudah menikah.</li>
  <li>Mayoritas pelanggan memiliki pendidikan tingkat sekunder.</li>
  <li>Mayoritas pelanggan tidak memiliki catatan gagal pembayaran (default).</li>
  <li>Mayoritas pelanggan memiliki pinjaman rumah (housing loan) dan mayoritas juga tidak memiliki pinjaman (loan).</li>
  <li>Komunikasi dengan pelanggan sebagian besar dilakukan melalui telepon seluler (celular).</li>
  <li>Waktu pelaksanaan kampanye pemasaran terpusat di bulan Mei, dengan penyebaran yang signifikan pada bulan Juli dan Agustus.</li>
  <li>Mayoritas hasil dari kampanye pemasaran sebelumnya tidak diketahui.</li>
  <li>Mayoritas pelanggan tidak berlangganan produk/jasa yang ditawarkan dalam kampanye pemasaran tersebut.</li>
</ul>

<h3><strong>Multivariate Analysis</strong></h3>
<ul>
  <li>Mayoritas korelasi antar feature termasuk lemah (nilai korelasi kurang dari 0.3) kecuali pada feature previous dan pdays yang memiliki korelasi linear positif yang kuat.</li>
  <li>Semakin lama durasi kontak, semakin besar kemungkinan klien akan berlangganan deposito.</li>
  <li>Pada feature pdays dan previous salah satunya harus dihilangkan karena terdapat korelasi kuat diantara keduanya.</li>
  <li>Pelanggan paling banyak memiliki pekerjaan management.</li>
  <li>Pelanggan yang sudah menikah lebih banyak berlangganan deposito.</li>
  <li>Pelanggan dengan secondary education paling banyak berlangganan deposito.</li>
  <li>Pelanggan yang berlangganan deposito tidak memiliki kredit macet.</li>
  <li>Deposito paling banyak oleh pelanggan yang tidak memiliki pinjaman rumah.</li>
  <li>Pelanggan yang berlangganan deposito tidak memiliki pinjaman pribadi.</li>
  <li>Pelanggan lebih banyak menggunakan tipe cellular.</li>
  <li>Kontak paling banyak terjadi pada bulan Mei, yang juga menghasilkan jumlah pelanggan berlangganan deposito berjangka tertinggi dalam setahun.</li>
  <li>Hasil kampanye yang sukses memiliki tingkat rasio yang paling baik.</li>
</ul>

<h3><strong>Business Insight</strong></h3>
<ul>
  <li>Hanya 11,6% nasabah yang sudah membuka deposito berjangka. Artinya hanya ada 5.300 nasabah yang berlangganan, dan 40.055 lainnya belum berlangganan deposito.</li>
  <li>Rata-rata usia pelanggan/nasabah ialah berusia sekitar 30 sampai 40 tahun.</li>
  <li>Nasabah yang paling banyak membuka deposito berjangka berusia sekitar 30-40 tahun dan sudah menikah.</li>
  <li>Nasabah yang belum membuka deposit rata-rata berusia 30-40 tahun.</li>
  <li>Pelanggan yang memiliki housing loan (pinjaman rumah) cenderung tidak memilih untuk membuka deposito.</li>
  <li>Pelanggan yang tidak memiliki loan (pinjaman pribadi) lebih banyak yang mengambil deposito berjangka dibandingkan dengan pelanggan yang memiliki loan.</li>
</ul>

<h3><strong>Business Recommendation</strong></h3>
<ul>
  <li>
    <strong>Segmentasi target</strong><br>
    Data menunjukan bahwa pelanggan dalam rentang usia 30-40 tahun cenderung memiliki minat yang tinggi terhadap produk deposito. Kami merekomendasikan untuk melakukan segmentasi target yang lebih spesifik pada kelompok usia ini demi meningkatkan efektivitas kampanye pemasaran.
  </li>
  <li>
    <strong>Fokus pada pelanggan yang tidak memiliki loan</strong><br>
    Pelanggan yang tidak memiliki loan cenderung memiliki minat yang tinggi terhadap produk deposito. Hal tersebut bisa jadi karena mereka tidak memiliki beban keuangan, sehingga mereka bisa mengalokasikan dana pribadi mereka ke investasi, salah satunya deposito berjangka.
  </li>
  <li>
    <strong>Fokus pada pelanggan yang tidak memiliki housing loan</strong><br>
    Sama seperti pelanggan yang tidak memiliki pinjaman pribadi, kita dapat memberikan campaign terkait manfaat investasi sejak dini kepada pelanggan yang tidak memiliki housing loan. Harapannya, mereka bisa mengalokasikan uang yang mereka punya untuk berlangganan deposito berjangka di bank kita.
  </li>
  <li>
    <strong>Personalisasi komunikasi</strong><br>
    Jika dipetakan kembali, nasabah yang cenderung memiliki minat berlangganan deposito berjangka ialah mereka yang berusia 30-40 tahun, sudah menikah, tidak memiliki beban pinjaman. Untuk itu, kita dapat membuat campaign yang lebih personal, seperti:
    <ul>
      <li>Campaign untuk memberikan awareness tentang pentingnya investasi sejak ini untuk mempersiapkan dana pendidikan untuk anak.</li>
      <li>Merekomendasikan deposito dengan bunga tinggi sebagai tabungan membeli rumah.</li>
      <li>Menampilkan keunggulan deposito dibanding investasi lain.</li>
    </ul>
  </li>
</ul>
