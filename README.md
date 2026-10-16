# 🏪 WarungPintar

**Asisten AI untuk mencatat, memantau, dan mengembangkan usaha warung dan UMKM.**

Catat penjualan semudah ngobrol, stok dan laporan diurus otomatis.

- Tim: [Nama Tim]
- Kompetisi: [Nama Hackathon]
- Demo: [Link demo]

## Latar belakang

Puluhan juta UMKM di Indonesia, terutama warung kecil, masih mencatat transaksi di buku tulis atau mengandalkan ingatan. Akibatnya pemilik usaha sulit mengetahui untung rugi, stok sering kosong saat ramai atau menumpuk sampai kedaluwarsa, dan catatan keuangan tidak cukup rapi untuk mengajukan modal usaha. Aplikasi pembukuan yang ada biasanya terlalu rumit dan memakai istilah akuntansi yang asing bagi pengguna awam.

WarungPintar menjawab masalah itu dengan satu prinsip: pencatatan harus semudah mengirim pesan.

## Fitur

- **Catat dengan bahasa sehari-hari.** Tulis atau ucapkan seperti "tadi laku 5 telur, 2 minyak goreng, 3 indomie". Sistem mengenali barang dan jumlahnya, lalu menampilkan daftar yang bisa dikoreksi sebelum disimpan.
- **Dasbor penjualan.** Omzet hari ini dan 7 hari terakhir, perkiraan laba, grafik harian, dan barang terlaris.
- **Rekomendasi stok.** Perkiraan sisa hari stok berdasarkan rata-rata penjualan harian, lengkap dengan saran jumlah belanja untuk 7 hari.
- **Ringkasan mingguan.** Ringkasan singkat berbahasa Indonesia yang bisa disalin dan dibagikan.

## Cara menjalankan

Prototipe ini berupa satu file HTML tanpa dependensi, jadi tidak perlu instalasi.

1. Unduh atau clone repositori ini.
2. Buka `index.html` di peramban.

Untuk demo online, aktifkan GitHub Pages: **Settings > Pages > Deploy from a branch > main / root**.

## Teknologi

Prototipe saat ini:

- HTML, CSS, dan JavaScript murni
- Penyimpanan data di peramban (`localStorage`)
- Pengenalan suara lewat Web Speech API (jika didukung peramban)

Rencana pengembangan:

- OCR dan model bahasa (LLM) untuk membaca foto nota, tulisan tangan, dan kalimat bebas
- Backend (FastAPI atau Node.js) dengan basis data PostgreSQL atau Firebase
- Model prediksi stok yang lebih akurat

## Cara kerja

1. **Input:** pengguna menulis atau berbicara.
2. **Pemrosesan:** teks dipecah menjadi nama barang dan jumlah, lalu dicocokkan dengan daftar barang warung.
3. **Konfirmasi:** pengguna memeriksa dan mengoreksi hasil sebelum disimpan.
4. **Analisis:** sistem menghitung omzet, laba, barang terlaris, dan kebutuhan stok.
5. **Output:** dasbor, status stok, dan ringkasan mingguan.

## Batasan prototipe

- Pembacaan catatan masih memakai pencocokan kata kunci untuk 7 barang contoh, belum memakai model AI.
- Riwayat penjualan 7 hari dan daftar harga adalah data contoh.
- Fitur scan nota dari foto belum tersedia.
- Data tersimpan di peramban masing-masing dan belum tersinkron antar perangkat.

## Rencana berikutnya

- Scan nota dan tulisan tangan dengan OCR
- Ekstraksi catatan dengan LLM agar memahami istilah dan singkatan lokal
- Integrasi WhatsApp untuk mencatat lewat chat
- Pencatatan otomatis dari pembayaran digital seperti QRIS
- Ekspor laporan keuangan sederhana untuk pengajuan modal

## Tim

| Nama | Peran |
|---|---|
| [Nama 1] | AI dan backend |
| [Nama 2] | Frontend dan pengalaman pengguna |
| [Nama 3] | Riset dan data uji |
| [Nama 4] | Presentasi dan dokumentasi |

## Lisensi

[MIT](LICENSE) atau sesuaikan dengan ketentuan lomba.
