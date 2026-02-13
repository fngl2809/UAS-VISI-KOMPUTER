# 🎓 UAS Visi Komputer

## Implementasi SIFT untuk Image Stitching (Panorama)

---

## Deskripsi Proyek

Proyek ini merupakan tugas akhir (UAS) pada mata kuliah Visi Komputer yang berfokus pada implementasi algoritma **Scale-Invariant Feature Transform (SIFT)** untuk proses *image stitching* atau pembuatan citra panorama.

Tujuan utama dari proyek ini adalah memahami dan mengimplementasikan tahapan utama dalam visi komputer, meliputi:

* Deteksi fitur (Feature Detection)
* Ekstraksi deskriptor fitur
* Pencocokan fitur (Feature Matching)
* Estimasi Homografi (Perspective Transformation)
* Proses penggabungan citra (Image Stitching)

Sebagai analisis tambahan, proyek ini juga membandingkan performa algoritma **SIFT** dengan **ORB (Oriented FAST and Rotated BRIEF)** dari segi jumlah keypoints yang terdeteksi serta efisiensi waktu eksekusi.

---

## Teknologi dan Library

Proyek ini dikembangkan menggunakan bahasa pemrograman **Python** dengan beberapa library utama:

* **OpenCV**
  Digunakan untuk pemrosesan citra, deteksi fitur (SIFT & ORB), feature matching, serta perhitungan homografi.

* **NumPy**
  Digunakan untuk manipulasi array dan operasi matriks dalam proses transformasi perspektif.

* **Matplotlib**
  Digunakan untuk visualisasi hasil deteksi fitur, proses matching, serta hasil panorama akhir.

---

## Dataset

Dataset yang digunakan merupakan foto pribadi yang diambil di area **Jalan Universitas Darussalam Gontor, Ngawi**, terdiri dari dua citra dengan area *overlapping* yang cukup untuk dilakukan proses penyambungan menjadi panorama.

---

## Alur Implementasi

Tahapan dalam proyek ini meliputi:

1. Membaca dua citra input
2. Melakukan deteksi dan ekstraksi fitur menggunakan SIFT
3. Melakukan pencocokan fitur menggunakan metode Brute Force Matcher
4. Menyeleksi *good matches*
5. Menghitung matriks homografi menggunakan RANSAC
6. Melakukan *warping* dan penggabungan citra ke dalam kanvas yang diperluas (*expanded canvas*)
7. Menampilkan hasil panorama akhir
8. Membandingkan hasil SIFT dengan ORB

---

## Cara Menjalankan Proyek

### 1️ Clone Repository

```bash
git clone https://github.com/USERNAME_KAMU/NAMA_REPO.git
cd NAMA_REPO
```

### 2️ Instalasi Library

Pastikan Python sudah terinstal, lalu jalankan:

```bash
pip install opencv-python numpy matplotlib
```

### 3️ Jalankan Notebook

Buka file berikut menggunakan:

* Jupyter Notebook
* Google Colab
* atau Kaggle Notebook

```
uas-visi-komputer.ipynb
```

Kemudian jalankan seluruh cell secara berurutan.

---

## Hasil dan Analisis

Proyek ini menghasilkan beberapa visualisasi utama:

###  SIFT Feature Detection

Menampilkan keypoints yang terdeteksi pada masing-masing citra.

### SIFT Feature Matching

Menampilkan garis penghubung antar fitur yang cocok pada kedua citra.

### Panorama Result

Hasil akhir penggabungan dua citra menggunakan metode expanded canvas sehingga tidak ada bagian penting yang terpotong.

### Perbandingan SIFT vs ORB

Analisis komparatif meliputi:

* Jumlah keypoints yang terdeteksi
* Kualitas pencocokan fitur
* Waktu eksekusi algoritma

---

## 👤 Author

**Fiona Anggilia**
Universitas Darussalam Gontor
Mata Kuliah: Visi Komputer


