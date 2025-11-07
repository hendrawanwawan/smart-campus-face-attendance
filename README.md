# 🎓 Sistem Manajemen Presensi Mahasiswa Berbasis Face Recognition
### Universitas Muslim Indonesia (UMI)

---

## 🧾 Deskripsi Proyek
Proyek ini merupakan bagian dari tugas **Mata Kuliah Arsitektur Perangkat Lunak** dengan tema **Ekosistem Smart Campus Digital**.  
Sistem ini dikembangkan untuk mendukung proses **presensi mahasiswa** secara otomatis dengan teknologi **Face Recognition**, sehingga mampu meningkatkan **keakuratan, keamanan, dan efisiensi** presensi di lingkungan kampus Universitas Muslim Indonesia (UMI).

Dengan sistem ini, mahasiswa cukup menghadapkan wajah ke kamera di ruang kelas, dan sistem akan mengenali identitas mahasiswa secara real-time serta mencatat waktu dan lokasi kehadirannya.  
Data kehadiran akan tersimpan di basis data dan dapat diakses oleh **dosen maupun admin fakultas** melalui dashboard.

---

## 🧩 Tujuan Proyek
- Meningkatkan keakuratan presensi dan mencegah manipulasi data.  
- Mengurangi ketergantungan pada tanda tangan manual atau QR code yang mudah disalahgunakan.  
- Mengintegrasikan data kehadiran dengan sistem akademik kampus.  
- Mendukung konsep **Smart Campus Digital** di Universitas Muslim Indonesia.

---

## 🧠 Fitur Utama
✅ Deteksi wajah otomatis menggunakan kamera perangkat (Face Recognition).  
✅ Verifikasi identitas mahasiswa berdasarkan dataset wajah.  
✅ Pencatatan waktu dan lokasi kehadiran.  
✅ Dashboard monitoring kehadiran untuk dosen dan admin fakultas.  
✅ Penyimpanan data kehadiran ke dalam database terpusat.  
✅ Integrasi dengan sistem akademik (siakad) UMI.  

---

## 🏗️ Arsitektur Sistem
Sistem ini dibangun menggunakan pendekatan **Event-Driven Architecture (EDA)** agar setiap proses berjalan asinkron dan efisien.

[Camera Sensor]
↓
[Face Recognition Module (ML Model)]
↓
[Verification Service]
↓
[Attendance Database]
↓
[Dashboard Admin & Lecturer]


---

## ⚙️ Teknologi yang Digunakan
| Komponen | Teknologi |
|-----------|------------|
| Bahasa Pemrograman | Python |
| Library Deteksi Wajah | OpenCV, face_recognition |
| Backend API | Flask / FastAPI |
| Database | MySQL / SQLite |
| Arsitektur | Event-Driven Architecture |
| Tools Diagram | Visual Paradigm / Draw.io |
| Version Control | GitHub Repository |

---

## 📋 Kebutuhan Sistem
### Kebutuhan Fungsional
1. Sistem mampu mengenali wajah mahasiswa dari kamera.  
2. Sistem menyimpan data presensi (nama, waktu, foto, status).  
3. Dosen dapat melihat laporan kehadiran melalui dashboard.  
4. Admin dapat menambahkan dataset wajah mahasiswa baru.

### Kebutuhan Non-Fungsional
- Akurasi pengenalan wajah ≥ 90%.  
- Respon deteksi wajah < 2 detik.  
- Data tersimpan aman dan terenkripsi.  
- Sistem mampu menampung ≥ 100 pengguna aktif.

---

## 🧭 Business Drivers
| No | Driver | Dampak terhadap Arsitektur |
|----|--------|----------------------------|
| 1 | Efisiensi proses presensi | Mendorong sistem otomatis dengan event-driven workflow |
| 2 | Akurasi kehadiran | Membutuhkan model face recognition dengan validasi tinggi |
| 3 | Integrasi akademik | Butuh API modular agar mudah dihubungkan dengan siakad |

---

## 🧩 Trade-offs
| Aspek | Opsi A | Opsi B | Keputusan | Alasan |
|--------|---------|---------|------------|--------|
| Teknologi Pengenalan | QR Code | Face Recognition | Face Recognition | Lebih aman dan sulit dipalsukan |
| Mode Input | Manual | Otomatis | Otomatis | Efisiensi waktu dan tenaga |
| Arsitektur | Monolitik | Event-Driven | Event-Driven | Skalabilitas dan modularitas lebih baik |

---

## 👥 Tim Pengembang
| Nama | NIM | Peran |
|------|-----|-------|
| **Hendarawan Wan** | [Isi NIM Kamu] | System Analyst & Dokumentasi |
| **[Nama Anggota 2]** | [Isi NIM] | Developer & Diagram Specialist |

---

## 📸 Dokumentasi
Folder `documentation/` berisi:
- Foto demo pendeteksian wajah mahasiswa.  
- Screenshot hasil pencatatan kehadiran.  
- Video pendek uji coba sistem.

Contoh:

📸 documentation/
├── demo_photo1.jpg
├── demo_photo2.jpg
└── demo_video.mp4


---

## 📂 Struktur Repository

📦 C2_1_AttendanceManagement_FaceRecognition/
├── 📄 C2_1_AttendanceManagement_FaceRecognition.pdf # Laporan lengkap
├── 🎞️ C2_1_AttendanceManagement_FaceRecognition.pptx # Slide presentasi
├── 💻 prototype/
│ ├── face_recognition_demo.py
│ ├── dataset/
│ └── output_log.csv
├── 📸 documentation/
│ ├── demo_photo1.jpg
│ └── demo_video.mp4
└── 📘 README.md


---

## 📚 Referensi
1. M. Richards and N. Ford, *Fundamentals of Software Architecture: An Engineering Approach*, O’Reilly Media, 2020.  
2. S. Newman, *Building Microservices: Designing Fine-Grained Systems*, 2nd ed., O’Reilly Media, 2021.  
3. A. Geitgey, “Face Recognition with Python,” *GitHub Repository: ageitgey/face_recognition*, 2023.  
4. G. Hohpe and B. Woolf, *Enterprise Integration Patterns*, Addison-Wesley, 2003.  
5. M. Fowler, “Event-Driven Architecture,” *martinfowler.com*, 2017.

---

## 🧠 Lisensi & Catatan
Proyek ini dikembangkan untuk keperluan akademik di **Universitas Muslim Indonesia (UMI)**.  
Dilarang menyalin, mengedit, atau mempublikasikan ulang tanpa izin pengembang.  
Segala data wajah yang digunakan dalam prototipe bersifat **simulasi internal**, bukan data pribadi mahasiswa sebenarnya.

---

## 📆 Informasi Tugas
- **Kelas:** C2  
- **Kelompok:** 1  
- **Mata Kuliah:** Arsitektur Perangkat Lunak  
- **Deadline:** 9 November 2025 – 23:00 WITA  
- **Format File:** PDF (Laporan) dan PPTX (Slide)  
- **Nama File:** `C2_1_AttendanceManagement_FaceRecognition.pdf / .pptx`

---

## 🌐 Link Repository
> https://github.com/hendarawan/umi-face-attendance-system

---

### ✨ Dosen Pengampu
> [Nama Dosen Kamu]  
> Fakultas Ilmu Komputer — Universitas Muslim Indonesia  
> Makassar, 2025
