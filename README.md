# Tugas Praktik Flutter — Halaman Biodata Diri

**Muhammad Zaim El Yafi** · **24090064** · **TI - 5D**

Aplikasi Flutter sederhana yang menampilkan halaman biodata diri: foto, nama
lengkap, NIM, kelas, dan tempat tanggal lahir.

## Struktur

```
lib/main.dart          -> seluruh source code aplikasi
assets/images/         -> foto biodata
pubspec.yaml           -> deklarasi dependency & assets
test/widget_test.dart  -> smoke test
```

## Widget yang digunakan

| Widget | Fungsi |
|---|---|
| `MaterialApp` | Root aplikasi, mengatur tema dan halaman awal |
| `Scaffold` | Kerangka halaman (AppBar + body) |
| `AppBar` | Header halaman dengan judul |
| `GridView.count` | Layout grid (di sini `crossAxisCount: 1`) |
| `SingleChildScrollView` | Membuat konten bisa di-scroll |
| `Column` | Menyusun widget secara vertikal |
| `Image.asset` | Menampilkan foto dari folder assets |
| `Text` | Menampilkan nama, NIM, kelas, TTL |

Penjelasan lengkap tiap widget ada di `Penjelasan_Widget_Biodata.pdf`.

## Cara Menjalankan

Repo ini hanya berisi source code — folder platform (android/ios/web/dll)
sengaja tidak di-push. Jalankan sekali untuk membuatnya kembali:

```bash
flutter create .
flutter pub get
flutter run -d chrome
```

Pastikan file foto ada di `assets/images/biodata.jpeg`.
