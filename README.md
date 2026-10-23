# StatefulWidget – Flutter

## 📝 Deskripsi Singkat

Aplikasi tasbih digital berbasis Flutter yang menerapkan konsep **StatefulWidget** untuk mengelola perubahan data secara dinamis. Aplikasi ini dilengkapi dengan penghitung tasbih, circular progress bar, tombol tambah berbentuk ikon sidik jari, serta tombol reset untuk mengembalikan hitungan ke nol.

Aplikasi membatasi hitungan hingga 33 dan menampilkan perkembangan hitungan melalui indikator berbentuk lingkaran.

## ✨ Fitur Utama

- **Penghitung Tasbih:** Menampilkan jumlah hitungan yang sedang berjalan.
- **Circular Progress Bar:** Memvisualisasikan perkembangan hitungan menuju 33.
- **Tombol Tambah:** Menambahkan satu hitungan setiap kali ikon sidik jari ditekan.
- **Tombol Reset:** Mengembalikan hitungan dan progress ke nilai awal.
- **Pembaruan Tampilan Otomatis:** Tampilan berubah mengikuti nilai state terbaru.

## 🛠️ Teknologi yang Digunakan

- **Flutter & Dart** – Pengembangan aplikasi.
- **Material Design** – Komponen dan tampilan antarmuka.
- **simple_circular_progress_bar** – Menampilkan indikator progres berbentuk lingkaran.
- **StatefulWidget & setState()** – Mengelola perubahan state.
- **ValueNotifier** – Memperbarui nilai circular progress bar.

## 📂 Struktur Proyek

```text
tasbih_app/
├── lib/
│   └── main.dart
├── pubspec.yaml
└── README.md
```

## ⚙️ Cara Kerja Aplikasi

1. Aplikasi dimulai dengan nilai hitungan `0`.
2. Pengguna menekan ikon sidik jari untuk menambah hitungan.
3. Hitungan bertambah hingga maksimal `33`.
4. Circular progress bar ikut berubah sesuai jumlah hitungan.
5. Tombol reset digunakan untuk mengembalikan hitungan dan progress ke `0`.

## 📚 Konsep Flutter yang Dipelajari

- **StatefulWidget:** Widget yang dapat berubah selama aplikasi berjalan.
- **setState():** Memperbarui tampilan setelah terjadi perubahan data.
- **ValueNotifier:** Mengelola nilai yang digunakan oleh circular progress bar.
- **initState() dan dispose():** Menginisialisasi serta membersihkan objek yang digunakan selama siklus hidup widget.
- **InkWell:** Membuat area yang dapat merespons sentuhan pengguna.
- **FloatingActionButton:** Menyediakan tombol aksi untuk mereset hitungan.
- **SimpleCircularProgressBar:** Menampilkan progres hitungan dalam bentuk lingkaran.

## 🚀 Cara Menjalankan

1. Pastikan Flutter SDK telah terpasang.
2. Buka proyek `tasbih_app` melalui VS Code atau Android Studio.
3. Tambahkan dependency berikut pada bagian `dependencies` di file `pubspec.yaml`:

   ```yaml
   simple_circular_progress_bar: ^1.0.2
   ```

4. Jalankan perintah berikut pada terminal:

   ```bash
   flutter pub get
   ```

5. Jalankan aplikasi menggunakan perintah:

   ```bash
   flutter run
   ```

## 📌 Kesimpulan

Aplikasi tasbih digital menerapkan StatefulWidget untuk mengelola perubahan hitungan secara dinamis. Penggunaan `setState()` dan `ValueNotifier` memungkinkan nilai hitungan serta circular progress bar diperbarui sesuai interaksi pengguna. Aplikasi ini menjadi contoh penerapan pengelolaan state dasar dalam Flutter.
