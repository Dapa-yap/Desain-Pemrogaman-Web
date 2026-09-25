+--------------------------------------------------+
|                   SIMPUS-Mini                    |
+--------------------------------------------------+
|                                                  |
|  [ < Kembali ke Daftar Buku ]                    |
|                                                  |
|  ===============================                 |
|  | Judul   : Bumi Manusia      |                 |
|  | Penulis : Pramoedya A. Toer |                 |
|  | Tahun   : 1980              |                 |
|  | Kategori: Fiksi Sejarah     |                 |
|  | Stok    : 5                 |                 |
|  ===============================                 |
|                                                  |
|  Sinopsis:                                       |
|  Buku ini menceritakan kisah Minke, seorang      |
|  pemuda pribumi yang berjuang di masa kolonial...|
|                                                  |
+--------------------------------------------------+
[Petugas Login] -> [Dashboard] -> [Pilih menu "Buku"] -> [Cari judul buku yang ingin dihapus] -> [Klik tombol "Hapus"] -> [Sistem memunculkan Pop-up Peringatan: "Yakin ingin menghapus buku ini?"] -> [Petugas Klik "Ya"] -> [Data buku terhapus] -> [Sistem mengembalikan Petugas ke halaman Daftar Buku]  
Identifikasi edge case tambahan yang mungkin belum tercatat, contoh: apa yang terjadi kalua petugas mencoba meminjamkan buku yang sama ke anggota yang sama dua kali berturut-turut?
-Kasus Hapus Buku yang Sedang Dipinjam: Bagaimana jika Petugas mencoba menghapus data sebuah buku (seperti pada alur di atas), tetapi sistem mendeteksi buku tersebut statusnya sedang dipinjam oleh anggota? Sistem harusnya mencegah penghapusan ini dan mengeluarkan pesan error ("Buku tidak dapat dihapus karena sedang dalam masa peminjaman").
-Kasus Input Angka Minus: Saat petugas menambahkan buku baru atau memperbarui data, bagaimana jika petugas tidak sengaja mengetik angka negatif untuk stok buku (misalnya: -5)? Sistem harus memvalidasi form agar stok minimal adalah 0.

