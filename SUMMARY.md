
# SUMMARY

Dokumen ini berisi ringkasan beberapa library dan algoritma yang umum digunakan dalam analisis data dan machine learning dengan Python. Materi meliputi pengolahan data, visualisasi, dan algoritma klasifikasi dasar.

---

## 1. Pandas (Pengolahan Data)

**Pandas** adalah library Python yang digunakan untuk manipulasi dan analisis data berbentuk tabel (DataFrame).

### Fitur Utama:
- **Membaca Data**: `read_csv()`, `read_excel()`
- **Menampilkan Data**: `head()`, `tail()`
- **Statistik Ringkas**: `describe()`, `info()`
- **Menangani Missing Values**: `fillna()`, `dropna()`
- **Manipulasi Baris/Kolom**: `groupby()`, `sort_values()`, `drop()`, `rename()`

---

## 2. Matplotlib (Visualisasi Data)

**Matplotlib** digunakan untuk membuat berbagai macam grafik dari data.

### Contoh Penggunaan:
- **Garis (Line Chart)**: `plt.plot()`
- **Histogram**: `plt.hist()`
- **Diagram Batang (Bar Chart)**: `plt.bar()`
- **Sebaran (Scatter Plot)**: `plt.scatter()`
- **Elemen Visualisasi**: `plt.title()`, `plt.xlabel()`, `plt.ylabel()`

---

## 3. Naive Bayes (Klasifikasi Probabilistik)

**Naive Bayes** adalah algoritma klasifikasi berbasis Teorema Bayes yang mengasumsikan bahwa setiap fitur bersifat independen.

### Karakteristik:
- Proses pelatihan cepat dan ringan
- Efektif untuk dataset besar
- Umumnya digunakan untuk klasifikasi teks (spam filter, analisis sentimen)

### Contoh Implementasi:
```python
from sklearn.naive_bayes import GaussianNB

model = GaussianNB()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
```

---

## 4. Decision Tree (Klasifikasi dan Regresi)

**Decision Tree** menggunakan struktur pohon untuk mengambil keputusan berdasarkan nilai fitur.

### Karakteristik:
- Mudah dipahami dan divisualisasikan
- Dapat digunakan untuk:
  - Klasifikasi
  - Regresi
- Rentan terhadap overfitting jika tidak dilakukan pruning

### Contoh Implementasi:
```python
from sklearn.tree import DecisionTreeClassifier

model = DecisionTreeClassifier()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
```

### Visualisasi Pohon Keputusan:
```python
from sklearn.tree import plot_tree
import matplotlib.pyplot as plt

plt.figure(figsize=(12, 8))
plot_tree(model, filled=True)
plt.show()
```

---

Dokumen ini cocok digunakan sebagai catatan cepat untuk implementasi dasar dalam proyek data science dengan Python.
