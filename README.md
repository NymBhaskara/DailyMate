# DailyMate 🚀

**DailyMate** adalah platform pengembangan diri yang didesain untuk kesederhanaan dan konsistensi. Aplikasi ini membantu pengguna membangun kebiasaan positif melalui *random task generator* (generator tugas) yang memberikan tugas mikro berdasarkan kategori fokus: Kesehatan, Sosial, atau Literatur.

## 👥 Anggota Kelompok 5

| Nama | NRP |
| :--- | :--- |
| **Muhammad Akmal Rafiansyah** | 5026231101 |
| **I Nyoman Mahadyana Bhaskara** | 5026231162 |
| **Javier Pandapotan Valerian** | 5026231201 |
| **Redo Adika Dharmawan** | 5026231171 |

---

## ✨ Fitur Utama

1.  **Random Task Generator**: Mendapatkan tugas acak dari database berdasarkan kategori (Health, Social, Literature).
2.  **Mastery Level (XP System)**: Sistem gamifikasi di mana pengguna mendapatkan XP setiap kali menyelesaikan tugas untuk menaikkan level di setiap kategori.
3.  **Task History**: Melacak riwayat tugas yang telah diselesaikan, dikelompokkan berdasarkan waktu (Today, Yesterday, Older).
4.  **Authentication**: Login dan Sign Up aman menggunakan Supabase Auth.

---

## 🛠️ Teknologi yang Digunakan

* **Frontend Framework**: Flutter (Dart)
* **Backend & Database**: Supabase (PostgreSQL)
* **Fitur Supabase**: Authentication, Database (CRUD), Realtime.

---

## 💻 Cara Instalasi

Ikuti langkah-langkah berikut untuk menyiapkan proyek di lingkungan lokal Anda:

1.  **Prasyarat**
    Pastikan komputer Anda telah terinstal:
    * **Flutter SDK** (Versi terbaru stable)
    * **Git**
    * **Visual Studio Code** atau **Android Studio**

2.  **Clone Repository**
    Buka terminal atau command prompt, lalu jalankan perintah berikut untuk mengunduh kode sumber:
    ```bash
    git clone [https://github.com/NymBhaskara/DailyMate.git](https://github.com/NymBhaskara/DailyMate.git)
    ```

3.  **Masuk ke Direktori Proyek**
    ```bash
    cd DailyMate
    ```

4.  **Instal Dependencies**
    Unduh semua library yang diperlukan (seperti `supabase_flutter`, dll) dengan perintah:
    ```bash
    flutter pub get
    ```

5.  **Konfigurasi Database**
    Proyek ini menggunakan **Supabase**. Pastikan file konfigurasi (biasanya di `lib/main.dart` atau `lib/env.dart`) sudah menyertakan **URL** dan **Anon Key** Supabase yang valid agar aplikasi dapat terhubung ke database.

---

## ▶️ Cara Menjalankan Aplikasi

Setelah proses instalasi selesai, Anda dapat menjalankan aplikasi dengan langkah berikut:

1.  **Siapkan Emulator / Device**
    * Buka **Android Emulator** atau **iOS Simulator**.
    * Atau, hubungkan perangkat fisik Anda dan pastikan mode *USB Debugging* aktif.

2.  **Jalankan Perintah Run**
    Ketik perintah berikut di terminal:
    ```bash
    flutter run
    ```

3.  **Tunggu Proses Build**
    Tunggu beberapa saat hingga proses *build* selesai dan aplikasi terbuka di emulator/perangkat Anda.

## 📂 Struktur Folder

Berikut adalah struktur folder utama dalam direktori `lib/` proyek ini:

```text
lib/
├── env.dart             # Konfigurasi Environment (API Keys Supabase)
├── history_page.dart    # Halaman riwayat tugas yang sudah selesai
├── home_page.dart       # Halaman utama (Generate Task & Task List)
├── login_page.dart      # Halaman Login dan Registrasi
├── main.dart            # Entry point aplikasi & Auth Wrapper
└── profile_page.dart    # Halaman profil pengguna & Mastery Progress
