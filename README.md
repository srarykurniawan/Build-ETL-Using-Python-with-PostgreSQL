# 1. Apa itu ETL
ETL (Extract – Transform – Load) adalah proses pengolahan data dari berbagai sumber hingga siap digunakan di database atau data warehouse.
* 🔄Extract → Mengambil data (API, database, file CSV/Excel, web scraping).
* 🧹 Transform → Membersihkan, memvalidasi, dan mengubah data.
* 📦 Load → Menyimpan data ke database / data warehouse.

| Tahap      | Library                                                          |
| ---------- | ---------------------------------------------------------------- |
| Extract    | `requests`, `pandas`, `sqlalchemy`, `beautifulsoup4`, `selenium` |
| Transform  | `pandas`, `numpy`                                                |
| Load       | `psycopg2`, `sqlalchemy`, `pymysql`                              |
| Logging    | `logging`                                                        |
| Orkestrasi | `Airflow`, `Prefect`                                             |
| Testing    | `pytest`, `great_expectations`                                   |

# 2. Apa Tujuan ETL menggunakan Python
untuk mengelola, menyiapkan, dan memindahkan data secara otomatis dari berbagai sumber agar siap digunakan untuk analisis, reporting, dan pengambilan keputusan.

### 1. Mengintegrasikan Data dari Berbagai Sumber > 👉 Tujuan: memastikan data akurat, konsisten, dan berkualitas.
Python memungkinkan pengambilan data dari:
* API
* Database (MySQL, PostgreSQL, SQL Server)
* File (CSV, Excel, JSON)
* Web scraping

### 2. Membersihkan dan Menstandarkan Data > 👉 Tujuan: menyatukan data yang tersebar ke dalam satu sistem terpusat.
Data mentah biasanya:
* Duplikat
* Format tidak konsisten
* Missing value
* Salah tipe data

Python (dengan pandas, numpy) digunakan untuk:
* Data cleaning
* Normalisasi format
* Validasi data

### 3. Mengotomatisasi Proses Pengolahan Data > 👉 Tujuan: efisiensi waktu, minim human error, dan scalable.
Tanpa ETL, proses data sering dilakukan manual.
Dengan Python:
* ETL bisa dijalankan otomatis (harian/jam-an)
* Bisa diatur dengan scheduler (Airflow, Cron)

