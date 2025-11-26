# Stokastik_8_RB
# 📄 Analisis Sistem Antrian Absensi Dosen Fakultas Sains ITERA Menggunakan Model M/M/1 untuk Optimasi Waktu Tunggu  
**Pemodelan Stokastik – 2025**

## 👥 Anggota
- Safitri – 122450071  
- Fayyaza Aqila Syafitri Achjar – 122450131  
- Chevando Daffa Pramanda – 122450095  
- Residen Nusantara R. M – 122450080  

Program Studi Sains Data  
Fakultas Sains, Institut Teknologi Sumatera  

---

## 📌 Gambaran Umum  
Repository ini berisi analisis sistem antrian pada proses absensi dosen Fakultas Sains ITERA menggunakan **model antrian M/M/1**. Penelitian dilakukan melalui observasi langsung selama jam sibuk (06.00–08.00 WIB) dan dianalisis untuk mengetahui efektivitas mesin absensi dalam menangani beban kedatangan dosen.

Model M/M/1 dipilih karena sistem absensi memiliki:
- satu server (1 mesin absensi),
- kedatangan acak mengikuti distribusi Poisson (λ),
- waktu pelayanan mengikuti distribusi eksponensial (μ).

---

## 🎯 Tujuan Penelitian
1. Menentukan parameter kedatangan (λ) dan pelayanan (μ).  
2. Menganalisis performa sistem melalui metrik antrian seperti Lq, Ls, Wq, Ws, dan utilisasi (ρ).  
3. Mengidentifikasi jam puncak (peak minutes) dan memberikan rekomendasi optimalisasi.

---

## 🧩 Metodologi

### **1. Data**
- **Jenis data:** Primer  
- **Durasi:** 10–13 November 2025  
- **Waktu:** 06.00–08.00 WIB  
- **Interval:** Per menit  
- **Dicatat:** jumlah kedatangan dosen & waktu pelayanan  

### **2. Variabel**
- λ: rata-rata kedatangan dosen (per menit)  
- μ: rata-rata pelayanan (per menit)  
- s: jumlah server (1)  
- Ukuran performa: Lq, Ls, Wq, Ws, ρ  

### **3. Model Antrian M/M/1**

Model antrian **M/M/1** digunakan untuk menggambarkan sistem pelayanan dengan satu server (single server) di mana:

- Kedatangan pelanggan (dosen) mengikuti pola **acak** dengan rata-rata tertentu.
- Waktu pelayanan juga bersifat **acak** namun memiliki distribusi rata-rata yang konsisten.
- Sistem hanya memiliki **1 mesin absensi** sebagai server.

Model ini menghasilkan beberapa ukuran performa penting, yaitu:

- **Laju kedatangan (lambda / λ)**  
  Rata-rata jumlah dosen yang datang per menit.

- **Laju pelayanan (mu / μ)**  
  Rata-rata jumlah dosen yang dapat dilayani per menit oleh mesin absensi.

- **Utilisasi sistem (rho / ρ)**  
  Menggambarkan tingkat kesibukan mesin. Semakin besar nilai ini, semakin sibuk server bekerja.

- **Jumlah rata-rata dosen dalam sistem (Ls)**  
  Banyaknya dosen yang sedang menunggu maupun yang sedang dilayani.

- **Jumlah rata-rata dosen dalam antrian (Lq)**  
  Banyaknya dosen yang hanya menunggu (belum dilayani).

- **Waktu rata-rata dalam sistem (Ws)**  
  Waktu total yang dihabiskan dosen sejak datang hingga selesai absensi.

- **Waktu rata-rata menunggu (Wq)**  
  Waktu yang diperlukan dosen sebelum mendapatkan pelayanan.

Model M/M/1 membantu menganalisis apakah sistem absensi berpotensi menumpuk antrian, seberapa besar tingkat kesibukan mesin, serta efisiensi waktu tunggu yang dialami dosen.




---

## 📊 Hasil Utama

### **1. Data Kedatangan**

| Hari   | Total Kedatangan | λ (per menit) |
|--------|------------------|---------------|
| Senin  | 51               | 0.4215        |
| Selasa | 44               | 0.3636        |
| Rabu   | 50               | 0.4132        |
| Kamis  | 43               | 0.3554        |

Durasi tiap pengamatan: **120 menit**.

---

### **2. Hasil Perhitungan M/M/1**

Semua hari menunjukkan:

- Utilisasi (ρ) rendah → **0.35–0.42**  
- Antrian hampir tidak terbentuk  
- Wq: **0.3–0.7 menit**  
- Ws: **< 2 menit**  
- Lq < **1 orang**

Sistem bekerja **sangat efisien dan stabil**.

---

### **3. Peak Minutes (Menit Puncak)**

- Senin: **07.23–07.24**  
- Selasa: **07.38–07.39**  
- Rabu: **07.22–07.23**  
- Kamis: **07.33–07.34**  

---

## 📝 Kesimpulan

- Sistem absensi dosen dapat dimodelkan secara tepat menggunakan model antrian **M/M/1**.  
- Nilai utilisasi yang rendah menunjukkan bahwa kapasitas mesin absensi sangat mencukupi.  
- Waktu tunggu (Wq) dan waktu total dalam sistem (Ws) sangat rendah.  
- Antrian tidak terbentuk secara signifikan meskipun terdapat puncak kedatangan.  
- Model M/M/1 berhasil menggambarkan performa sistem secara akurat.

---

## 💡 Rekomendasi
1. Pemantauan berkala pada jam dan menit puncak.  
2. Peningkatan teknologi mesin absensi (biometrik cepat / QR / pengenalan wajah).  
3. Pertimbangan menambah server (M/M/s) bila jumlah dosen meningkat.  
4. Penelitian lanjutan menggunakan model M/G/1 atau simulasi komputer.  

---



