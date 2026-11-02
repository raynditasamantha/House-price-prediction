# Prediksi Harga Rumah Menggunakan Linear Regression

## Deskripsi Proyek
Proyek ini bertujuan untuk memprediksi harga rumah menggunakan algoritma **Linear Regression** berdasarkan beberapa fitur, seperti rata-rata pendapatan wilayah, usia rumah, jumlah kamar, jumlah kamar tidur, dan populasi wilayah.

Proyek ini juga mengeksplorasi penggunaan informasi State melalui proses *Feature Engineering* dan *One-Hot Encoding* untuk mengetahui apakah informasi geografis dapat meningkatkan performa prediksi model.

## Dataset
Dataset yang digunakan adalah USA Housing dengan total 5.000 data dan 7 kolom, yaitu:

- Avg. Area Income
- Avg. Area House Age
- Avg. Area Number of Rooms
- Avg. Area Number of Bedrooms
- Area Population
- Price (Target)
- Address

## Tools dan Library
- Python
- Pandas dan NumPy
- Matplotlib dan Seaborn
- Scikit-learn
- Jupyter Notebook

## Tahapan Proyek
1. Memuat dan memahami dataset.
2. Melakukan Exploratory Data Analysis (EDA).
3. Melakukan persiapan data dan pemilihan fitur.
4. Membagi dataset menjadi data latih dan data uji dengan rasio 80:20.
5. Melatih model Linear Regression.
6. Mengevaluasi performa model menggunakan MAE, RMSE, dan R².
7. Melakukan Feature Engineering menggunakan Regex dan One-Hot Encoding untuk mengekstrak informasi State dari kolom Address.
8. Membandingkan performa model sebelum dan sesudah penambahan fitur State.

## Hasil Evaluasi Model

Berikut merupakan perbandingan hasil evaluasi model Linear Regression:

| Eksperimen | MAE | RMSE | R² |
|---|---:|---:|---:|
| Tanpa fitur State | 80.879,10 | 100.444,06 | 0,9180 |
| Dengan fitur State | 81.901,89 | 101.302,88 | 0,9166 |

## Hasil dan Temuan
- Model Linear Regression memperoleh nilai R² sebesar 0,9180 tanpa penambahan fitur State.
- Penambahan informasi State menggunakan One-Hot Encoding belum berhasil meningkatkan performa model.
- Penggunaan lima fitur numerik awal menghasilkan performa prediksi yang sedikit lebih baik pada eksperimen ini.

## Struktur Repository
```text
├── USA_Housing.csv
├── Prediksi_Harga_Rumah_Regresi_Linear.ipynb
├── Prediksi_Harga_Rumah_Regresi_Linear_State.ipynb
└── README.md
```

## Cara Menjalankan Proyek
1. Clone repository ini.
2. Install library yang dibutuhkan:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
3. Jalankan Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Buka file notebook dan jalankan setiap cell secara berurutan.

## Kesimpulan
Proyek ini menunjukkan penerapan algoritma Linear Regression untuk memprediksi harga rumah berdasarkan sejumlah fitur numerik. Berdasarkan hasil eksperimen, penambahan fitur State melalui One-Hot Encoding belum memberikan peningkatan performa model dibandingkan penggunaan fitur numerik awal.

## Author
Rayndita.
