# SALES PERFORMANCE DASHBOARD USING EXCEL
## Problem Statement
Sebuah perusahaan retail skala menengah memiliki data penjualan bulanan yang berantakan dari berbagai platform dan data master produk yang terpisah. Jajaran manajemen ingin melihat laporan performa bisnis selama tahun 2025.

## Dataset & Formulas Used
### Dataset
Dataset yang digunakan adalah dataset dummy yang dibuat menggunakan Python menggunakan google colab(berkas ipynb tersedia). Dataset terdiri dari Data Transaksi sebanyak 1.000 data, Master Produk berisikan SKU (code barang), nama produk, kategori, cost dan harga. Terakhir Master Target berisikan target penjualan per produk setiap bulannya selama tahun 2025.

**Data Transaksi**

<img width="1032" height="447" alt="data transaksi" src="https://github.com/user-attachments/assets/985e316d-fd10-49fd-b607-9fbacc905d8b" />

**Master Product**

<img width="394" height="235" alt="master produk" src="https://github.com/user-attachments/assets/8b409bae-b070-4258-8101-814c631c2eb4" />

**Master Target**

<img width="870" height="96" alt="master target" src="https://github.com/user-attachments/assets/eba42b47-6f6e-4601-80b7-a04b980ac6ba" />

### Formulas
Menggunakan ```TRIM()``` dan ```PROPER()``` untuk menghilangan spasi berlebih dan mengubah huruf pertama pada setiap kata yang ada dalam tabel **nama pelanggan** menjadi huruf kapital.

Menggunakan ```MONTH()``` untuk mengambil data bulan pada tabel **tanggal** dan mengubahnya menjadi format **text** menggunakan ```TEXT()```

Menggunakan ```INDEX MATCH``` untuk menentukkan **kategori** dan **harga jual** berdasarkan **SKU** yang ada dalam **data transaksi dan master produk**. Selain itu, ```INDEX MATCH``` digunakan untuk mencari target bulanan per kategori berdasarkan **nama bulan** yang ada dalam data transaksi dan di master target.

Membuat **Pivot Table** sebelum membuat **Dashboard**

**Pivot Table**

<img width="822" height="339" alt="pivot tabel" src="https://github.com/user-attachments/assets/aac878ed-8a21-4a73-8661-fd332e72a575" />

**Dashboard**

<img width="781" height="414" alt="dashboard" src="https://github.com/user-attachments/assets/990d6834-e114-4752-896e-70053d276176" />

## Business Recomendations
1. Memberlakukan strategi kolaborasi dilini pakaian dengan KOL/IP:
   Kategori pakaian saat ini hanya menyumbang 5.08% dari total revenue. Disarankan melakukan kolaborasi ekslusif seperti official merchandise anime/KOL untuk meningkatkan nilai jual produk.
2. Melakukan program bundling dan promosi untuk kategori furnitur:
   Kategori furnitur berpotensi besar naik kelas dari kontribusi 16.9%. Skema promo berjangka (seperti paket bundling ruang kerja/diskon ongkir) dapat mempercepat pembeli mengambil keputusan.
3. Memberlakukan promo awal tahun untuk mencegah drop penjual dikuartal 1 (Q1):
   Data historis menunjukkan Q1 merupakan periode penjualan terendah (hanya Rp 711 Juta), dengan penurunan drastis di bulan Maret pada hampir seluruh wilayah. 
