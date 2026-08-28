# Animasi Lirik Lagu: Pelangi - HiVi! 🌈

Program Python sederhana ini dibuat untuk menampilkan sebagian lirik lagu **"Pelangi"** dari **HiVi!** secara animasi di terminal. Program ini menyimulasikan efek pengetikan (*typing effect*) yang kecepatannya disesuaikan per karakter dan per baris agar selaras dengan irama dan tempo asli lagu tersebut.

Proyek ini dikembangkan oleh **KELOMPOK JAVA**.

---

## Fitur Utama

1. **Typing Effect (Efek Mengetik)**
   Menampilkan teks lirik huruf demi huruf seperti sedang diketik secara real-time, memberikan kesan estetik dan dinamis pada output CLI (Command Line Interface).
2. **Dynamic Delay (Jeda Dinamis)**
   Memiliki konfigurasi tempo pengetikan untuk setiap karakter dan pengaturan jeda (*delay*) antar-baris lagu agar pas dengan ketukan irama lagu aslinya.
3. **Clean & Smooth Output**
   Menggunakan perintah `sys.stdout.flush()` untuk memastikan karakter yang dicetak langsung tampil ke layar tanpa tertahan di dalam *buffer* terminal.

---

## Penjelasan Kode (`Kelompok2_Hivi_Pelangi.py`)

Program ini hanya mengandalkan modul bawaan dari Python, yaitu `sys` dan `time`, sehingga sangat ringan dan tidak memerlukan instalasi *library* eksternal tambahan.

Di dalam fungsi utama `jalanin_lirik()`, logika program dibagi menjadi beberapa komponen data:
- **`lirik`**: Sebuah daftar (*list*) yang berisi pasangan data (*tuple*). Tuple ini memuat untaian lirik lagu (bagian *Bridge* dan *Chorus*) beserta durasi *delay* untuk kecepatan cetak per karakternya.
- **`delay`**: Sebuah *list* yang mengatur durasi jeda waktu (dalam hitungan detik) setelah sebuah baris lirik selesai dicetak secara utuh sebelum berlanjut ke baris lirik berikutnya.

Program menggunakan *nested loop* (perulangan bersarang). Loop luar untuk memproses setiap baris lirik, dan loop dalam untuk mencetak setiap karakter secara berurutan dengan jeda (`time.sleep()`).

---

##  Prasyarat & Cara Menjalankan

### Prasyarat
- Pastikan komputer Anda telah terinstal **Python 3.x**.
- Tidak ada *package* eksternal (seperti dari `pip`) yang perlu diinstal.

### Eksekusi Program
1. Unduh atau simpan kode program ke dalam direktori lokal Anda.
2. Buka aplikasi **Terminal** (di Mac/Linux) atau **Command Prompt / PowerShell** (di Windows).
3. Arahkan *path* ke direktori tempat file kode berada.
4. Jalankan perintah berikut ini:

```bash
python Kelompok2_Hivi_Pelangi.py
```

Setelah perintah dijalankan, program akan memunculkan judul `== PELANGI - HIVI` dan kemudian memulai animasi lirik lagunya!
