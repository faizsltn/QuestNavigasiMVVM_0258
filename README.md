# 📱 Navigation with MVVM - Jetpack Compose

Aplikasi Android sederhana yang dibangun menggunakan **Jetpack Compose** dan **Navigation Component** untuk mensimulasikan alur pengisian formulir dan pemrosesan data identitas.

---

## 👨‍💻 Identitas Mahasiswa

* **Nama**: Faiz Sulthon Daud Muhammad
* **NIM**: 20240140258
* **Program Studi**: Teknologi Informasi / Teknik
* **Instansi**: Universitas Muhammadiyah Yogyakarta

---

<img width="378" height="797" alt="image" src="https://github.com/user-attachments/assets/5fd8dc69-07d9-472a-944d-35978edfdf5c" />
<img width="372" height="806" alt="image" src="https://github.com/user-attachments/assets/d2f09073-9af2-4f3c-80e5-772efa57709e" />

## 🚀 Fitur & Fitur Layar (Screens)

Aplikasi ini terdiri dari 2 layar utama yang terhubung secara dinamis melalui `NavHost`:

1. **Form Isian (`Formulir.kt`)**:
   * Input teks nama lengkap (`OutlinedTextField`).
   * Pilihan jenis kelamin interaktif menggunakan `RadioButton` dan State Management.
   * Input teks alamat (`OutlinedTextField`).
   * Tombol `Submit` untuk berpindah ke halaman rincian data.

2. **Tampilan Data (`TampilData.kt`)**:
   * Menampilkan ringkasan data yang diinputkan.
   * Kustomisasi tipografi teks bergaya *Cursive*.
   * Pembatas antar-item menggunakan `HorizontalDivider`.
   * Tombol `Back` untuk kembali ke halaman formulir (`popBackStack`).

---

## 🛠️ Arsitektur & Teknologi

| Komponen | Teknologi |
| :--- | :--- |
| **Language** | Kotlin |
| **UI Framework** | Jetpack Compose |
| **Navigation** | Compose Navigation Component (`NavHost`, `NavHostController`) |
| **Theme & Material** | Material3 Design (`Scaffold`, `TopAppBar`) |
| **Resources** | `strings.xml` & `dimens.xml` |

---

## 📂 Struktur Repositori

```text
com.example.navigationwithmvvm/
├── view/
│   ├── Formulir.kt       # Composable FormIsian (Halaman Input Data)
│   └── TampilData.kt     # Composable TampilData (Halaman Ringkasan Data)
├── MainActivity.kt       # Entry Point Utama Aplikasi
└── Navigasi.kt           # Konfigurasi Enum Navigasi & NavHost Controller
