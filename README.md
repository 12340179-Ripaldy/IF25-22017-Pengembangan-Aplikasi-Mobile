# IF25-22017 — Pengembangan Aplikasi Mobile

Mata kuliah ini mempelajari pengembangan aplikasi mobile multiplatform menggunakan **Kotlin Multiplatform (KMP)** dan **Compose Multiplatform**. Mahasiswa akan belajar membuat aplikasi yang dapat berjalan di Android dan iOS dengan satu codebase, termasuk integrasi dengan sistem cerdas (AI).

## Identitas Mata Kuliah

| | |
|---|---|
| Nama MK | Pengembangan Aplikasi Mobile |
| Kode MK | IF25-22017 |
| Rumpun MK | Rekayasa Perangkat Lunak & Sistem Informasi |
| Bobot (SKS) | 3 |
| Semester | Ganjil/Genap |
| Matakuliah Syarat | IF25-21012, IF25-21009 |
| Team Teaching | Muhammad Habib Algifari, S.Kom., M.T.I. |

## Capaian Pembelajaran

**CPL05** — Mampu menganalisis dan menerapkan konsep rekayasa perangkat lunak untuk pengembangan sistem cerdas secara profesional.

| CPMK | Deskripsi | CPL didukung |
|---|---|---|
| CPMK0501 | Mahasiswa mampu menerapkan konsep pemrograman untuk pengembangan perangkat lunak | CPL05 |
| CPMK0502 | Mahasiswa mampu menjelaskan konsep pemrograman untuk pengembangan perangkat lunak | CPL05 |
| CPMK0503 | Mahasiswa mampu menerapkan teknologi sistem cerdas dalam pengembangan perangkat lunak | CPL05 |

## Materi Pembelajaran / Pokok Bahasan

Intro KMP, Setup Environment, Hello World; Advanced Kotlin (Coroutines, Flow); Compose Multiplatform Basics; State Management (MVVM, ViewModel); Navigasi Antar Layar, Passing Data; Networking (Ktor Client, JSON); Local Data Persistence; Platform Specific Code; Sensor; Integrasi Sistem Cerdas (AI API); Testing dan Dependency Injection.

## Jadwal Mingguan

| Minggu | CPMK | Topik | Bahan Kajian | Bobot |
|---|---|---|---|---|
| 1 | CPMK0502 | Pengenalan MK dan Setup Environment | Kontrak kuliah, Overview KMP, Setup Android Studio, Hello World KMP | 4% |
| 2 | CPMK0501, CPMK0502 | Advanced Kotlin, Coroutines & Flow | Coroutines, Flow, Extension Functions, Null Safety, Data Classes, Sealed Classes | 4% |
| 3 | CPMK0501 | Compose Multiplatform Basics | UI terstruktur dengan layout yang tepat | 4% |
| 4 | CPMK0501 | State Management (MVVM) | State, remember, MutableState, ViewModel, StateFlow, Unidirectional Data Flow | 4% |
| 5 | CPMK0501 | Navigasi Antar Layar, Passing Data | Navigation Component, NavHost, NavController, Arguments, Bottom Navigation, Drawer | 4% |
| 6 | CPMK0501 | Networking | HTTP/REST, Ktor Client, JSON Serialization, Repository Pattern, Loading States | 4% |
| 7 | CPMK0501 | Local Data Persistence | DataStore Preferences, SQLDelight, Room (Android), Offline-First Architecture | 4% |
| 8 | — | **Ujian Tengah Semester (UTS)** | — | — |
| 9 | CPMK0501 | Platform Specific Code | expect/actual Pattern, Platform APIs, Permissions, Dependency Injection dengan Koin | 4% |
| 10 | CPMK0503 | Integrasi Sistem Cerdas (AI API) | OpenAI/Gemini API, Prompt Engineering, AI-powered Features | 4% |
| 11 | CPMK0502 | Testing dan Dependency Injection | Unit Testing, UI Testing, Koin DI, Test Doubles, Debugging | 4% |
| 12 | CPMK0501, CPMK0502 | Perencanaan & Setup Proyek Akhir | Requirements, Architecture Design, Repository Setup, CI/CD Basic | 10% |
| 13 | CPMK0501 | Pengembangan Fitur Lanjutan | Implementasi fitur lanjutan, Integration Testing, Performance | 5% |
| 14 | CPMK0501 | Penyempurnaan UI/UX & Testing | UI/UX Polish, Bug Fixing, Full Testing, Documentation | 5% |
| 15 | CPMK0503, CPMK0501, CPMK0502 | Final Demo & Presentasi | Final Bug Fixes, Demo Preparation, Presentation Practice, Live Code Review, QnA | 20% |
| 16 | — | **Ujian Akhir Semester (UAS)** | — | — |

## Penilaian

| Kriteria | CPMK0503 | CPMK0501 | CPMK0502 | Total Bobot |
|---|---|---|---|---|
| Observasi (Praktik) | 4 | 26 | 10 | 40 |
| Laporan Hasil Proyek | 5 | 0 | 0 | 5 |
| Tes Lisan (Tugas Kelompok) | 0 | 35 | 20 | 55 |
| **Total Bobot per CPMK** | **9** | **61** | **30** | **100** |

## Pustaka

**Utama:**
1. Dokumentasi KMP

**Pendukung:**
2. Panduan Proyek
3. Android Studio
4. Dokumentasi Kotlin
5. Dokumentasi API OpenAI/Gemini

## Media Pembelajaran

- **Software:** Framework Kotlin Multiplatform, Android Studio, Github, Youtube, dan lain-lain
- **Hardware:** Mobile Device, Komputer Lab, dan Laptop

## Struktur Repo

### Materi inti (sesuai Jadwal Mingguan RPS di atas)

- `P1 - Pengenalan MK dan Setup Environment.pdf`, `P2 - Advanced Kotlin Coroutines Flow.pdf`, `P3 - Compose Multiplatform Basics.pdf`, `P4 - State Management MVVM.pdf` — slide materi per pertemuan (baru tersedia untuk Pertemuan 1-4; Pertemuan 5-11 belum ada slide, hands-on-nya diturunkan langsung dari RPS).
- `P{n} - {Topik} - Hands-on/` — proyek **Kotlin Multiplatform + Compose Multiplatform** nyata (modul `composeApp` dengan `commonMain`/`androidMain`/`iosMain`/`desktopMain`, 3 latihan + solusi per pertemuan) untuk tiap pertemuan inti:

  | Folder | Pertemuan | Topik |
  |---|---|---|
  | `P1 - Pengenalan MK dan Setup Environment - Hands-on/` | 1 | Intro KMP, Setup Environment, expect/actual, Compose dasar |
  | `P2 - Advanced Kotlin Coroutines Flow - Hands-on/` | 2 | Advanced Kotlin, Coroutines & Flow (proyek Kotlin/JVM biasa) |
  | `P3 - Compose Multiplatform Basics - Hands-on/` | 3 | Compose Multiplatform Basics (layout, LazyColumn, custom component) |
  | `P4 - State Management MVVM - Hands-on/` | 4 | State Management MVVM (ViewModel, StateFlow, UDF) |
  | `P5 - Navigasi Antar Layar - Hands-on/` | 5 | Navigasi Antar Layar, Passing Data (NavHost, Bottom Navigation) |
  | `P6 - Networking REST API - Hands-on/` | 6 | Networking (Ktor Client, JSON, Repository Pattern) |
  | `P7 - Local Data Storage - Hands-on/` | 7 | Local Data Persistence (SQLDelight, offline-first) |
  | *(Pertemuan 8 = UTS, tidak ada hands-on)* | 8 | — |
  | `P9 - Platform Specific Features - Hands-on/` | 9 | Platform Specific Code (expect/actual lanjutan, Koin DI) |
  | `P10 - Integrasi AI API - Hands-on/` | 10 | Integrasi Sistem Cerdas (AI API — Gemini) |
  | `P11 - Testing dan DI - Hands-on/` | 11 | Testing dan Dependency Injection |
  | *(Pertemuan 12-15 = pengembangan proyek akhir, 16 = UAS, tidak ada hands-on materi baru)* | 12-16 | — |

  Catatan: proyek `P1, P3-P7, P9-P11` tidak menyertakan folder `iosApp/` (proyek Xcode) — lihat README masing-masing folder untuk cara menambahkannya via [kmp.jetbrains.com](https://kmp.jetbrains.com). Belum di-build/verify penuh (tidak ada Android SDK/Xcode di lingkungan pembuatannya) — lakukan Gradle sync di Android Studio sebelum dipakai di kelas.

  **Solusi tidak ikut di-commit.** Setiap folder hands-on punya subfolder/modul `solusi/` (atau `handson{n}-solusi/`) berisi jawaban lengkap — folder ini di-`.gitignore` di tiap proyek supaya mahasiswa yang clone repo hanya mendapat soal `latihan/`. Jawaban dipegang/dibagikan terpisah oleh pengajar.

### Materi suplemen (di luar jadwal RPS)

- `Kotlin Dasar/` — 13 pertemuan slide + hands-on Kotlin dasar (Kotlin/JVM biasa, bukan KMP) untuk memperkuat fondasi Kotlin sebelum masuk ke materi inti KMP: `P1 - Introduction to Kotlin`, `P2 - Object-Oriented Programming`, `P3 - Generics`, `P4 - Collections and co.`, `P5 - Functional Programming`, `P6 - Parallel and Concurrent Programming`, `P7 - Asynchronous Programming in Kotlin`, `P8 - Exceptions`, `P9 - Testing`, `P10 - Build Systems`, `P11 - The Java Virtual Machine and the Kotlin Compiler`, `P12 - Reflection (JVM)`, `P13 - Backend Development Basics` — masing-masing dengan folder `P{n} - {Topik} - Hands-on/` (modul `handson{n}-latihan`/`handson{n}-solusi`; solusi juga di-gitignore).

### Lainnya

- `RPS_MK_IF25-22017.pdf` — Rencana Pembelajaran Semester lengkap (sumber data untuk bagian-bagian di atas).
