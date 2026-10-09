# Bank Transactions Clustering and Classification

## 📌 Deskripsi Proyek
Proyek ini mengimplementasikan teknik *machine learning* berbasis klasterisasi (*clustering*) dan klasifikasi (*classification*) untuk menganalisis data transaksi perbankan. Tujuan utamanya adalah mengeksplorasi aktivitas keuangan nasabah guna mendeteksi pola transaksi ganjil (anomali) dan mengidentifikasi indikasi kecurangan (*fraud detection*). Melalui pemetaan profil perilaku transaksi yang terukur, proyek ini diharapkan mampu memberikan kontribusi nyata dalam memperkuat sistem keamanan finansial serta mengoptimalkan proses evaluasi risiko secara berkala.

## 💾 Informasi Dataset
Repository ini menggunakan dataset historis transaksi perbankan yang terdiri dari **2.512 sampel data**. Dataset ini menyediakan informasi komprehensif mengenai demografi nasabah serta kebiasaan finansial mereka. 

Atribut data yang dianalisis mencakup:
* **Informasi Identitas & Akses:** ID transaksi, ID akun perbankan, ID perangkat (*DeviceID*), alamat IP, durasi sesi transaksi, serta jumlah percobaan *login* sebelum transaksi berhasil.
* **Detail Finansial:** Nilai nominal transaksi, saldo akhir akun, jenis transaksi (Debit/Kredit), kanal transaksi yang digunakan (Online, ATM, Cabang), serta riwayat frekuensi transaksi harian.
* **Profil Demografi:** Usia, profesi, dan lokasi geografis nasabah (nama kota di Amerika Serikat).

## Fitur Utama
- TransactionID: Pengidentifikasi unik alfanumerik untuk setiap transaksi.
- AccountID: ID unik untuk setiap akun, dapat memiliki banyak transaksi.
- TransactionAmount: Nilai transaksi dalam mata uang, mulai dari pengeluaran kecil hingga pembelian besar.
- TransactionDate: Tanggal dan waktu transaksi terjadi.
- TransactionType: Tipe transaksi berupa 'Credit' atau 'Debit'.
- Location: Lokasi geografis transaksi (nama kota di Amerika Serikat).
- DeviceID: ID perangkat yang digunakan dalam transaksi.
- IP Address: Alamat IPv4 yang digunakan saat transaksi, dapat berubah untuk beberapa akun.
- MerchantID: ID unik merchant, menunjukkan merchant utama dan anomali transaksi.
- AccountBalance: Saldo akun setelah transaksi berlangsung.
- PreviousTransactionDate: Tanggal transaksi terakhir pada akun, berguna untuk menghitung frekuensi transaksi.
- Channel: Kanal transaksi seperti Online, ATM, atau Branch.
- CustomerAge: Usia pemilik akun.
- CustomerOccupation: Profesi pengguna seperti Dokter, Insinyur, Mahasiswa, atau Pensiunan.
- TransactionDuration: Lama waktu transaksi (dalam detik).
- LoginAttempts: Jumlah upaya login sebelum transaksi—jumlah tinggi bisa mengindikasikan anomali.

Seluruh variabel ini diolah sebagai parameter input utama untuk mengenali karakteristik transaksi normal versus aktivitas mencurigakan.

## 🛠️ Tech Stack

| Kategori | Teknologi yang Digunakan |
| :--- | :--- |
| **🌐 Bahasa Pemrograman** | Python |
| **🌱 Environment** | Jupyter Notebook |
| **⚛️ Library Utama** | NumPy, pandas, matplotlib, seaborn, scikit-learn, Yellowbrick, Joblib |
| **⚡ Tool Pengembangan** | Google Colab |

---

## ⚙️ Panduan Instalasi & Pengaturan

### Prasyarat
Sebelum memulai, pastikan perangkat Anda telah memenuhi spesifikasi berikut:
* **Python** versi 3.11 atau yang lebih baru.
* **Git** sudah terpasang di sistem operasi Anda.

### Kloning Repositori
Jalankan perintah berikut pada terminal atau command prompt untuk menyalin proyek ini ke direktori lokal Anda:

```bash
git clone https://github.com/Fikri-Rouzan/clustering-and-classification-bank-transactions.git
cd clustering-and-classification-bank-transactions
```
