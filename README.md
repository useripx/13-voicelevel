<div align="center">

# 🎙️ Voice Level Detector

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Repo Size](https://img.shields.io/github/repo-size/useripx/13-VoiceLevel?style=for-the-badge&color=blue)
![Version](https://img.shields.io/badge/Version-1.0-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-Free-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Selesai-brightgreen?style=for-the-badge)
![Semester](https://img.shields.io/badge/Semester-1-blueviolet?style=for-the-badge)

**Aplikasi sederhana berbasis CLI untuk mendeteksi tingkat volume suara (dalam desibel) melalui mikrofon secara real-time.**

*Dibuat oleh Yogi Ario — Proyek Semester 1*

---

</div>

## 📖 Deskripsi

**Voice Level Detector** adalah skrip Python pendek dan fungsional yang membaca input audio dari mikrofon default komputer Anda, kemudian menghitung dan menampilkan **tingkat suara / volume** secara seketika (*real-time*). Nilai yang dihasilkan dihitung menggunakan perhitungan norma linear (Linear Algebra Norm) pada data audio, yang merepresentasikan tingkat kenyaringan suara (estimasi dalam *dB*).

## ✨ Fitur Utama

- 🎤 **Real-time Monitoring** — Menangkap sinyal audio secara berkelanjutan.
- 🧮 **Numpy Calculation** — Menggunakan operasi matriks yang cepat dan efisien melalui `numpy.linalg.norm` untuk menghitung intensitas suara.
- ⏱️ **Loop Tanpa Henti** — Pendeteksian berjalan terus-menerus hingga dihentikan manual oleh pengguna (melalui pintasan keyboard `Ctrl+C`).

## 📁 Struktur Proyek

```
13 voicelevel/
└── tes.py        # Source code utama (dan satu-satunya)
```

## 🚀 Cara Menjalankan

### Prasyarat Instalasi

Aplikasi ini bergantung pada dua pustaka pihak ketiga. Pastikan Anda sudah menginstalnya menggunakan `pip`:

```bash
pip install sounddevice numpy
```

*(Catatan: Anda juga perlu memastikan mikrofon sudah terpasang dan berfungsi pada komputer Anda).*

### Menjalankan Program

Jalankan perintah berikut pada terminal atau *command prompt*:

```bash
python tes.py
```

### Menghentikan Program

Untuk menghentikan pendeteksian suara, tekan:
`Ctrl + C` (Keyboard Interrupt).

## 📸 Contoh Output

```text
Mendeteksi tingkat suara. Tekan Ctrl+C untuk menghentikan.
Tingkat suara: 0.12 dB
Tingkat suara: 0.15 dB
Tingkat suara: 5.43 dB    <-- (Saat Anda berbicara)
Tingkat suara: 2.10 dB
...
Pendeteksian dihentikan.
```

## 🛠️ Teknologi

| Komponen | Detail |
|----------|--------|
| Bahasa | Python 3.x |
| Audio API | `sounddevice` (Wrapper untuk PortAudio) |
| Komputasi | `numpy` (Perhitungan vektor & matriks) |
| Sample Rate | 44100 Hz |
| Channels | 1 (Mono) |

## 👤 Author

**Yogi Ario**

---

<div align="center">

*Proyek Mata Kuliah — Semester 1 — Teknik Informatika UNP*

</div>
