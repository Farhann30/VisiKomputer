**SEGERA GANTI BAGIAN DALAM TANDA KURUNG SIKU `[]` DENGAN INFORMASI ANDA.**

```markdown
# Proyek Tugas Akhir Visi Komputer: Peningkatan Kualitas Citra Nota Pembayaran

## Deskripsi Singkat
Proyek ini bertujuan untuk meningkatkan kualitas citra nota pembayaran menggunakan kombinasi teknik _classical computer vision_, yaitu _Contrast Stretching_ dan Filter Penajaman Laplacian. Aplikasi ini dikembangkan sebagai bagian dari tugas akhir mata kuliah Visi Komputer Semester 6 2024/2025. Fokus utama adalah pada implementasi teknik pemrosesan citra klasik tanpa menggunakan _library deep learning_[cite: 3, 4].

## Identitas Mahasiswa
- Nama: **M Farhan Bachtiar**
- NIM: **D121221011**

## Tujuan README
Dokumen `README` ini disediakan untuk memastikan kode program dapat dijalankan dan direproduksi hasilnya, serta berisi instruksi eksekusi yang jelas sesuai dengan ketentuan tugas akhir.

## Prasyarat Sistem & Instalasi Library
Untuk menjalankan kode dan mereproduksi hasil, Anda memerlukan:
- Python 3.x
- Jupyter Notebook (atau VSCode dengan ekstensi Jupyter).
- Library Python berikut (versi yang digunakan saat pengembangan atau versi stabil terbaru):
    - OpenCV (`opencv-python`)
    - NumPy (`numpy`)
    - Matplotlib (`matplotlib`)

Instalasi library dapat dilakukan menggunakan pip:
```bash
pip install opencv-python numpy matplotlib
```

## Instruksi Eksekusi Kode
Untuk menjalankan kode dan mereproduksi hasil yang dilaporkan:

1.  **Persiapan File:**
    * Pastikan semua prasyarat sistem dan library telah terinstal.
    * Letakkan file Jupyter Notebook utama (VisKom_CitraNotaPembayaran.ipynb`) dalam satu folder.
    * Siapkan satu atau beberapa file citra nota pembayaran (format `.jpg` atau `.png`) yang akan diuji. Anda dapat menggunakan contoh citra yang sama dengan yang digunakan dalam laporan untuk mereproduksi hasil.

2.  **Konfigurasi Path Citra Input:**
    * Buka file `VisKom_CitraNotaPembayaran.ipynb`.
    * Pada sel kode yang berfungsi untuk memuat citra (biasanya di bagian awal notebook), temukan baris kode yang mendefinisikan `image_path`.
    * **Ubah nilai variabel `image_path` tersebut agar menunjuk ke lokasi dan nama file citra nota pembayaran yang ingin Anda proses.**
        ```python
        # Contoh baris kode yang perlu diubah di dalam notebook:
        image_path = 'path/ke/citra/nota_anda.jpg' # GANTI DENGAN PATH CITRA YANG SESUAI
        ```

3.  **Menjalankan Notebook:**
    * Buka file `VisKom_CitraNotaPembayaran.ipynb` menggunakan Jupyter Notebook, Jupyter Lab, atau VSCode.
    * Untuk mereplikasi hasil seperti pada laporan, jalankan semua sel kode secara berurutan dari atas ke bawah. Perintah untuk menjalankan sel biasanya "Shift + Enter" atau melalui menu "Run".

## Input yang Diharapkan
-   Program ini menerima input berupa satu file citra nota pembayaran digital (misalnya, format JPG, PNG). Path ke file ini harus dikonfigurasi di dalam kode notebook seperti dijelaskan pada instruksi eksekusi.

## Output yang Dihasilkan
-   Setelah semua sel dijalankan, output akan ditampilkan langsung di dalam Jupyter Notebook. Output meliputi:
    1.  Visualisasi citra asli (grayscale).
    2.  Visualisasi citra setelah proses _Contrast Stretching_.
    3.  Visualisasi hasil antara dari filter Laplacian.
    4.  Visualisasi citra final setelah penajaman Laplacian.
    5.  Plot histogram untuk citra asli, setelah _contrast stretching_, dan setelah penajaman, untuk analisis distribusi intensitas piksel.
-   Secara default, program tidak menyimpan file citra hasil olahan secara otomatis, kecuali jika kode untuk menyimpan file diaktifkan atau ditambahkan secara manual.

## Struktur Folder yang Direkomendasikan untuk Reproducibilitas
```
/NamaFolderProyek
|-- README.md
|-- VisKom_CitraNotaPembayaran.ipynb  
|-- Image
    |-- blur.jpg
    |-- blur1.jpg
    |-- blur2.jpg
    |-- gelap.jpg
    |-- gelap1.jpg
    |-- jelas.jpg
|-- output
    |-- output.png  
```
