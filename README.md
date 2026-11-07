# Kasir Sahabat Jaya Motor

Aplikasi kasir (POS) dan backoffice untuk toko sparepart sepeda motor **Sahabat Jaya Motor**.
Seluruh aplikasi ada di satu file: `kasir-sparepart.html`. Tidak perlu instalasi.

## Fitur

- **Kasir**: cari produk atau scan barcode, keranjang, diskon (Rp atau %), PPN, harga eceran/grosir, tahan dan lanjutkan transaksi.
- **Pembayaran**: tunai, transfer, QRIS, tempo (piutang), dan **campuran** (misalnya tunai + transfer).
- **Retur sebagian**: kembalikan sebagian barang dari sebuah nota. Stok bertambah, omzet berkurang.
- **Produk**: SKU otomatis, barcode, kategori, merek, kecocokan motor, rak, harga beli, harga eceran dan grosir, stok minimum, impor/ekspor CSV.
- **Stok**: barang masuk dari pemasok (lunas/utang), stok opname, kartu stok per produk, data pemasok.
- **Riwayat**: daftar nota, pelunasan tempo, pembatalan nota (butuh otorisasi), retur.
- **Laporan**: omzet, laba kotor, produk terlaris, metode pembayaran, piutang, nilai persediaan, daftar barang perlu dibeli, ekspor CSV.
- **Peran dan PIN**: Pemilik, Manajer, Kasir. Kunci layar otomatis. Pembatalan nota dan retur butuh PIN manajer atau pemilik.
- **Cetak struk**: kertas thermal 58 mm atau 80 mm lewat file cetak (HTML) atau PDF.
- **Cadangan**: ekspor dan pulihkan data (JSON) dari menu Pengaturan.

## Cara memakai

1. Buka `kasir-sparepart.html` di browser (Chrome disarankan), atau lewat GitHub Pages bila diaktifkan.
2. Buka **Pengaturan**: isi nama toko, alamat, nomor telepon, dan ukuran kertas struk.
3. Buka **Pengaturan > Staf & PIN** untuk membuat akun pemilik dan kasir.
4. Tambahkan produk di menu **Produk** (atau impor CSV), lalu catat stok awal atau barang masuk di menu **Stok**.
5. Mulai berjualan di menu **Kasir**.

## Tentang penyimpanan data

- Saat dibuka sebagai file biasa atau lewat GitHub Pages, data disimpan **di browser perangkat itu saja**. Perangkat lain tidak melihat data yang sama.
- Karena itu, rutin unduh **cadangan JSON** dari menu Pengaturan, terutama sebelum membersihkan data browser.
- Penyimpanan data bersama antar-perangkat hanya aktif saat aplikasi dijalankan sebagai artefak di Claude.

## Mencetak struk thermal

Dari jendela struk, tekan **Cetak** untuk mengunduh file struk. Buka file itu, lalu jendela cetak muncul otomatis. Pilih printer thermal dan ukuran kertas yang sesuai. Alternatifnya, unduh **PDF** dan cetak dari aplikasi printer.
