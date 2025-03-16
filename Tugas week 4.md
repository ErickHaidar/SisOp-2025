# Tugas Week 4 Sistem Operasi

## Identitas
**Nama**: Erick Haidar Rahmat  
**NRP**: 3124500047  
**Dosen Pengajar**: Dr Ferry Astika Saputra ST, M.Sc  
**Program Studi**: D3 Teknik Informatika B  

---

## Perbedaan Multi Programming vs Multi Tasking

**Multi Programming** adalah teknik di mana beberapa program dimuat ke dalam memori utama secara bersamaan untuk meningkatkan efisiensi penggunaan CPU. CPU hanya mengeksekusi satu program pada satu waktu, tetapi jika program yang berjalan membutuhkan operasi I/O, CPU akan beralih ke program lain yang siap dieksekusi. Multi programming sering digunakan dalam sistem batch.

**Multi Tasking**, di sisi lain, memungkinkan beberapa tugas atau proses berjalan secara bersamaan dengan membagi waktu CPU menggunakan teknik time-sharing. CPU secara cepat beralih antar proses dalam interval waktu kecil, memberikan ilusi bahwa semua proses berjalan secara simultan. Multi tasking umum ditemukan dalam sistem operasi modern seperti Windows, Linux, dan macOS.

Perbedaan utama:
- Multi programming bertujuan meningkatkan efisiensi CPU.
- Multi tasking berfokus pada pengalaman pengguna dengan membagi waktu CPU antar proses secara cepat.

---

## Fungsi OS

Sistem operasi (OS) adalah perangkat lunak yang berfungsi sebagai perantara antara perangkat keras komputer dan pengguna. Berikut beberapa fungsi utama OS:

1. **Manajemen Proses**: Mengatur pembuatan, eksekusi, dan terminasi proses serta menjadwalkan CPU untuk eksekusi proses secara efisien.
2. **Manajemen Memori**: Mengalokasikan dan de-alokasi memori untuk proses menggunakan teknik seperti paging dan segmentation.
3. **Manajemen File & Penyimpanan**: Mengatur data dalam sistem file (misalnya NTFS, FAT32, ext4) serta memberikan akses file yang terstruktur.
4. **Manajemen Perangkat I/O**: Mengontrol perangkat keras seperti keyboard, mouse, printer, dan hard drive melalui driver perangkat.
5. **Keamanan & Proteksi**: Mengelola hak akses pengguna, enkripsi data, serta mencegah akses tidak sah.
6. **Antarmuka Pengguna**: Menyediakan CLI (Command-Line Interface) dan GUI (Graphical User Interface) untuk kemudahan penggunaan.

OS memastikan bahwa berbagai perangkat keras dan perangkat lunak bekerja secara harmonis dengan lingkungan yang stabil, aman, dan efisien.

---

## Apa itu Virtualisasi Container

Virtualisasi container adalah teknologi yang memungkinkan isolasi dan eksekusi aplikasi bersama dengan dependensinya dalam lingkungan yang ringan dan mandiri yang disebut **container**. Berbeda dengan virtualisasi tradisional yang menggunakan mesin virtual (VM), container berbagi sistem operasi host tetapi tetap memiliki lingkungan eksekusi sendiri.

### Cara Kerja
Container bekerja menggunakan fitur kernel seperti **namespace** dan **cgroups** untuk memastikan bahwa setiap container memiliki ruang proses, jaringan, dan sistem file yang terisolasi dari container lain.

### Teknologi Populer
- **Docker**: Memudahkan pembuatan, distribusi, dan manajemen container.
- **Kubernetes**: Mengelola container dalam skala besar dengan fitur seperti penjadwalan otomatis, load balancing, dan pemulihan otomatis.

### Keunggulan Virtualisasi Container
- **Ringan**: Berbagi kernel OS, lebih efisien dibandingkan VM.
- **Portabilitas**: Dapat dijalankan di berbagai lingkungan tanpa perubahan.
- **Isolasi**: Setiap container memiliki lingkungan sendiri.
- **Skalabilitas**: Mendukung deployment cepat dalam lingkungan cloud atau microservices.

Teknologi ini menjadi solusi ideal dalam pengembangan perangkat lunak modern seperti **DevOps, CI/CD, dan microservices**.

---

## Flowchart: Proses dari Komputer Dinyalakan hingga Dimatikan

```mermaid
graph TD;
    A[Power On] --> B[BIOS/UEFI Initialization];
    B --> C[POST (Power-On Self Test)];
    C --> D[Load Bootloader];
    D --> E[Load Operating System];
    E --> F[User Authentication];
    F --> G[User Session];
    G --> H[User Runs Applications];
    H --> I[Shutdown Initiated];
    I --> J[Close Applications & Services];
    J --> K[OS Shutdown Process];
    K --> L[Power Off];
```



**Tugas Week 4 Sistem Operasi - Selesai** ✅
