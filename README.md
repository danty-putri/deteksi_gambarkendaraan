# 🚗 YOLOv9 Vehicle Detection and Counting

Proyek ini menggunakan model **YOLOv9** untuk mendeteksi dan menghitung jumlah kendaraan (mobil dan motor) pada gambar secara otomatis.
Kode ini menampilkan hasil deteksi dengan *bounding box* berwarna, label, dan jumlah kendaraan yang terdeteksi.

---

## 🔍 Fitur Utama

* Deteksi objek menggunakan model **YOLOv9 custom** yang telah dilatih pada dataset kendaraan.
* Menghitung jumlah objek berdasarkan label (`mobil`, `motor`, dll).
* Visualisasi hasil deteksi dengan **warna berbeda untuk setiap label**.
* Menampilkan hasil dalam bentuk gambar yang telah diberi *bounding box* dan teks jumlah kendaraan.
* Gambar hasil deteksi otomatis disimpan ke file output.

---

## 🧠 Teknologi yang Digunakan

* Python
* Ultralytics YOLO
* OpenCV
* Matplotlib
* NumPy

---

## ⚙️ Cara Penggunaan

1. Pastikan semua dependensi sudah terinstal:

   ```bash
   pip install ultralytics opencv-python matplotlib numpy
   ```

2. Jalankan script dengan menyesuaikan path model dan gambar:

   ```python
   python detect_vehicle.py
   ```

3. Gambar hasil deteksi akan disimpan di path yang ditentukan (`output_path`).

---

## 📊 Contoh Output

Setiap kendaraan yang terdeteksi akan ditandai dengan kotak berwarna:

* 🟩 **Hijau muda** → Mobil
* 🟦 **Biru muda** → Motor

Teks jumlah kendaraan juga ditampilkan di bagian atas gambar:

```
Kendaraan mobil yang terdeteksi berjumlah 3
Kendaraan motor yang terdeteksi berjumlah 5
```

---

## ✨ Hasil Akhir

Proyek ini dapat digunakan untuk:

* Analisis kepadatan lalu lintas
* Sistem monitoring parkir
* Penelitian terkait deteksi kendaraan otomatis berbasis visi komputer

---

**Author:** Putri Danty Apriani
**Model:** YOLOv9 (custom trained for car and motorcycle detection)
