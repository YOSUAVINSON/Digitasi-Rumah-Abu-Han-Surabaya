 APLIKASI DATA SEMANTIK DALAM PROSES DIGITASI ARTEFAK BUDAYA: STUDI KASUS RUMAH ABU HAN

Proyek ini merupakan bagian dari luaran praktis penelitian Tugas Akhir yang bertujuan untuk melakukan digitalisasi, penyimpanan data (metadata), serta visualisasi interaktif dari objek cagar budaya/artefak sejarah milik rumah abu keluarga Han.

---

 Artefak yang Didigitasi

Proyek ini mencakup digitasi terhadap tiga artefak bersejarah berikut:
1.  Fangding : Sebuah wadah pedupaan berbentuk persegi berkaki empat yang dikenal sebagai Fangding.
2.  Lukisan-1: Lukisan potret leluhur tradisional Tionghoa yang menggambarkan sosok pria lanjut usia memegang kipas, didampingi pelayan wanita di sampingnya yang membawa dokumen.
3.  Lukisan-2: Lukisan potret pasangan suami-istri berpakaian pejabat resmi Dinasti Qing. Pria mengenakan Guanmao (topi pejabat) dan jubah bersulam Buzi (lencana pangkat), sedangkan wanita mengenakan Fengguan (mahkota phoenix) dan jubah bersulam phoenix.

---

 Struktur Proyek Tugas Akhir
Seluruh aset digitasi disusun secara terstruktur dengan susunan sebagai berikut:
```text
D:\nitip\Project TUGAS AKHIR\Digitasi Artefak\
├── README.md                 <-- Dokumen petunjuk akademis ini (Terupdate)
├── 3d_models/                <-- Folder penyimpanan 3D model (.glb)
│   ├── lukisan_pejabat.glb
│   ├── pedupaan_perunggu.glb
│   └── lukisan_kaisar.glb
└── metadata/                 <-- Folder penyimpanan basis data informasi
    ├── fangding-pendupaan.json         <-- Metadata artefak fangding
    ├── lukisan-1.json        <-- Metadata lukisan potret leluhur
    ├── lukisan-2.json        <-- Metadata lukisan potret pasangan suami-istri
    └── paradata.json         <-- Rekaman teknis & etis proses digitasi
```

---

 Skema Data Proyek

 1. Metadata Artefak (metadata/metadata.json)
Struktur file metadata ini disederhanakan agar fokus pada parameter utama yang umum digunakan. Format ini sangat ideal untuk demonstrasi Data Entry (memasukkan data baru) dan Data Retrieval (membaca/menampilkan data di program):
*   author_name : Nama pembuat/pelukis/pembuat artefak asli (atau era asalnya).
*   year_made : Tahun atau periode perkiraan pembuatan artefak fisik asli.
*   material : Bahan fisik penyusun artefak asli.
*   description : Deskripsi atau narasi singkat mengenai artefak tersebut.

 2. Paradata Proses (metadata/paradata.json)
Paradata merupakan komponen penting dalam dokumentasi digitasi warisan budaya. File ini berisi rekaman riwayat teknis mengenai bagaimana dokumentasi digital ini dibuat, mulai dari tahap pengambilan foto, pengolahan data, hingga hasil akhir yang ditampilkan:
*   Peralatan: Perangkat, lensa, dan pencahayaan yang digunakan saat perekaman.
*   Fase RAW: Jumlah foto mentah, resolusi, dan format file asal yang diambil.
*   Fase Pemrosesan: Perangkat lunak photogrammetry yang digunakan dan jumlah polygon mentah.
*   Penyuntingan & Optimasi: Langkah retouching di Blender, pengurangan jumlah polygon (retopology/decimation) serta kompresi tekstur agar optimal untuk Web/AR.
*   Perlakuan khusus: Tindakan yang dilakukan untuk melindungi fisik objek asli selama proses digitalisasi.

---
