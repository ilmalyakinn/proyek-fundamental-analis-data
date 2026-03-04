# 📊 E-Commerce Public Data Analysis Dashboard ✨

Ini adalah proyek akhir (submission) untuk kelas **Belajar Analisis Data dengan Python** dari Dicoding. Proyek ini berfokus pada analisis data E-Commerce publik menggunakan bahasa pemrograman Python, di mana data diolah, dieksplorasi, dan kemudian disajikan dalam bentuk dashboard interaktif menggunakan **Streamlit**.

## � Fitur Dashboard
Dashboard ini menyajikan berbagai analisis bisnis penting:
- **Daily Orders Delivered:** Menampilkan pergerakan jumlah pesanan harian yang dikirim dan pendapatan terkait.
- **Customer Spend Money:** Menganalisis tren total pengeluaran pembeli dari waktu ke waktu.
- **Order Items:** Visualisasi jenis produk paling laris dan yang paling sedikit terjual.
- **Review Score:** Distribusi rating kepuasan pelanggan terhadap layanan secara keseluruhan.
- **Customer Demographic:** Demografi berdasarkan lokasi negara bagian (State) pembeli.
- **RFM Analysis:** Analisis tingkat lanjut untuk mengelompokkan pelanggan berdasarkan metrik *Recency* (waktu terakhir transaksi), *Frequency* (seberapa sering transaksi), dan *Monetary* (uang yang dihabiskan). Termasuk visualisasi segmentasi pembeli (Binning / Manual Clustering).
- **Geolocation Analysis:** Pemetaan persebaran lokasi geografis (titik koordinat) pelanggan di peta Brazil.

## 📂 Struktur Proyek
```text
├── dashboard/
│   ├── alldf.csv               # Dataset utama untuk dashboard
│   ├── dashboard.py            # Script utama Streamlit
│   ├── func.py                 # Kumpulan class & fungsi helper
│   └── geolocation.csv         # Dataset khusus untuk peta spasial
├── data/                       # Direktori berisi file raw dataset (*.csv) statis
├── notebook.ipynb              # File Jupyter Notebook (Proses EDA & Data Wrangling)
├── README.md                   # Dokumentasi proyek
├── requirements.txt            # Daftar pustaka / package Python yang dibutuhkan
└── url.txt                     # File referensi tambahan
```

## 🚀 Setup Environment

Jika Anda ingin menjalankan proyek ini secara lokal di komputer Anda, ikuti langkah-langkah instalasi berikut:

### 1. Clone Repository
Pastikan Anda sudah menginstal Git, lalu jalankan:
```bash
git clone https://github.com/ilmalyakinn/proyek-fundamental-analis-data.git
cd proyek-fundamental-analis-data
```

### 2. Setup Virtual Environment & Instalasi Library

**Menggunakan `pip` dan `venv` (Rekomendasi Windows):**
```bash
python -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt
```

**Menggunakan `pip` (Mac/Linux):**
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

**Menggunakan `conda`:**
```bash
conda create --name main-ds python=3.10
conda activate main-ds
pip install -r requirements.txt
```

### 3. Menjalankan Dashboard Streamlit
Setelah semua package terinstal, Anda dapat menjalankan server Streamlit menggunakan perintah di bawah ini dari branch dan main folder utama:
```bash
streamlit run dashboard/dashboard.py
```
atau (jika script Streamlit tidak terdeteksi via default PATH):
```bash
python -m streamlit run dashboard/dashboard.py
```

Dashboard akan otomatis terbuka pada antarmuka web browser Anda di alamat lokal `http://localhost:8501`.

## 📌 Catatan Penggunaan (Date Range)
Di dalam dashboard terdapat fitur filter *Date Range* (rentang waktu) pada bagian antarmuka samping (sidebar). 
- Harap **pilih 2 tanggal** batas pada kalender dropdown yang disediakan agar semua grafik menampilkan visualisasi data dalam rentang tersebut. Contoh: `2016/09/22` – `2017/09/13`.

---
🌟 *Dibuat oleh Ilmal Yakin untuk Final Submission Analisis Data (Dicoding)*
