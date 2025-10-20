# 🚗 YOLOv9 Vehicle Detection and Counting

![Deteksi Kendaraan](https://github.com/danty-putri/deteksi_gambarkendaraan/blob/main/detected_foto_0031.jpg)

Proyek ini menggunakan **YOLOv9** untuk mendeteksi dan menghitung jumlah kendaraan (*mobil* dan *motor*) dari **banyak gambar secara otomatis**.
Setiap gambar akan diproses, diberi *bounding box*, label, confidence score, serta jumlah kendaraan yang terdeteksi.
Hasil deteksi kemudian disimpan ke folder output.

---

## 🔍 Fitur Utama

* 🚘 **Batch detection:** mendeteksi kendaraan dari banyak gambar dalam satu folder.
* 🎯 Menampilkan label dan tingkat kepercayaan (*confidence score*) di atas setiap *bounding box*.
* 📊 Menghitung jumlah kendaraan berdasarkan label (`mobil`, `motor`).
* 🌈 Warna label berbeda:

  * 🔴 **Merah** untuk mobil
  * 🟠 **Oranye** untuk motor
* 💾 Menyimpan hasil deteksi ke folder output secara otomatis.
* 🖼️ Visualisasi hasil menggunakan **Matplotlib**.

---

## 🧠 Teknologi yang Digunakan

* Python
* Ultralytics YOLOv9
* OpenCV
* Matplotlib
* NumPy
* OS (untuk membaca dan menyimpan file secara otomatis)

---

## ⚙️ Cara Penggunaan

1. Pastikan semua dependensi telah diinstal:

   ```bash
   pip install ultralytics opencv-python matplotlib numpy
   ```

2. Atur path model dan folder input/output di dalam kode:

   ```python
   model = YOLO('/path/to/best.pt')
   input_folder = '/path/to/input_images'
   output_folder = '/path/to/output_results'
   ```

3. Jalankan script:

   ```bash
   python detect_batch_vehicle.py
   ```

4. Semua hasil deteksi akan tersimpan otomatis di folder output (`output_folder`).

---

## 📁 Struktur Folder

```
├── detect_batch_vehicle.py
├── best.pt
├── /input_images
│   ├── foto_001.jpg
│   ├── foto_002.jpg
│   └── ...
└── /output_results
    ├── detected_foto_001.jpg
    ├── detected_foto_002.jpg
    └── ...
```

---

## 🖼️ Contoh Output

Pada setiap gambar hasil deteksi:

* Bounding box berwarna menunjukkan lokasi kendaraan.
* Teks seperti berikut akan muncul di bagian atas:

  ```
  Kendaraan mobil yang terdeteksi berjumlah 3
  Kendaraan motor yang terdeteksi berjumlah 5
  ```

---

## ✨ Manfaat

Proyek ini dapat digunakan untuk:

* Analisis kepadatan lalu lintas dari data citra.
* Sistem monitoring kendaraan di area publik.
* Penelitian deteksi kendaraan berbasis visi komputer.

---

**Author:** Putri Danty Apriani

**Model:** YOLOv9 (Custom-trained for car and motorcycle detection)
