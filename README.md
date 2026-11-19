# ♟️ Catur Game v1 — Chess Royale

> **Catur modern di browser: main lawan bot, tantang teman, atau kumpulkan 33 papan lewat gacha.**

[![Live Demo](https://img.shields.io/badge/🎮_Mainkan_Sekarang-Catur_Game_v1-7c3aed?style=for-the-badge&logo=googlechrome&logoColor=white)](https://rxfatih-2.github.io/Catur-game_v1/)
[![GitHub Repo](https://img.shields.io/badge/📦_Source_Code-GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/rxfatih-2/Catur-game_v1)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/)

---

## 📖 Tentang Project

**Catur Game v1** (atau *Chess Royale*) adalah permainan catur berbasis web yang dibangun untuk menghadirkan pengalaman catur yang **lengkap dan menyenangkan** langsung dari browser—tanpa perlu install aplikasi.

Project ini bukan sekadar papan catur biasa. Di dalamnya ada **multiplayer online**, **bot dengan berbagai tingkat kesulitan**, **sistem progresi** (koin & ranked), dan **koleksi papan** yang bisa didapatkan lewat **gacha**. Semuanya dibungkus dalam antarmuka modern dengan dukungan **WebGL** untuk pengalaman visual yang lebih hidup.

---

## ✨ Fitur Unggulan

### 🎮 Mode Permainan
- **Main Berdua** — Dua pemain bergantian di satu layar (pass-and-play).
- **Lawan Bot** — Hadapi komputer dengan **4 level kesulitan**: Easy, Medium, Hard, dan Professional. Menang lawan bot dapat **+5.000 koin**.
- **Main Online (1v1)** — Tantang pemain lain lewat **Firebase**. Buat room, bagikan kode/link, atau langsung tantang dari daftar pemain online.

### ♟️ Fitur Gameplay
- **Undo & Redo** — Batalkan atau ulangi langkah.
- **Jeda Game** — Hentikan permainan sementara, lanjutkan atau ulangi dari awal.
- **Promosi Pion** — Pilih bidak pengganti (Ratu, Benteng, Gajah, Kuda).
- **Deteksi Checkmate & Stalemate** — Aturan catur standar diberlakukan penuh.

### 👤 Profil & Sosial
- **Profil Pemain** — ID permanen unik, bisa disalin, dan nama bisa diacak.
- **Riwayat Match** — Catatan pertandingan yang bisa dihapus.
- **Sistem Tantangan** — Terima atau tolak tantangan dari pemain lain.

### 🎨 Koleksi & Progresi
- **Toko Papan dengan Gacha** — Kumpulkan **33 papan** dari berbagai tingkat kelangkaan:
  - Common (50%), Langka (27%), Epic (13%), Legend (6%), Mitos (3%), Secret (1%).
- **Koin** — Mata uang in-game. Duplikat papan saat gacha dikembalikan **5.000 koin**.
- **Papan Peringkat (Ranked)** — Kumpulkan poin dari pertandingan ranked dan naikkan peringkatmu.

### 🎵 Audio & Visual
- **Musik Latar** — Beberapa trek musik (`.mp3`) dengan pengaturan volume.
- **Dukungan WebGL** — Render papan dan bidak dengan grafis 3D (dengan fallback jika perangkat tidak mendukung).

---

## 🛠️ Tech Stack

| Komponen | Teknologi |
|----------|-----------|
| **Frontend** | HTML5, CSS3, JavaScript (vanilla) |
| **Rendering 3D** | WebGL |
| **Backend / Realtime** | Firebase (untuk mode online & daftar pemain) |
| **Audio** | File MP3 (`lagu1.mp3` – `lagu4.mp3`) |
| **Deployment** | GitHub Pages (via GitHub Actions) |
| **Arsitektur** | Single-file (`index.html`) + aset audio |

---

## 🚀 Cara Menjalankan Secara Lokal

Karena project ini berupa aplikasi statis, kamu cukup menjalankan server lokal sederhana.

```bash
# 1. Clone repositori
git clone https://github.com/rxfatih-2/Catur-game_v1.git

# 2. Masuk ke folder project
cd Catur-game_v1

# 3. Jalankan server lokal (pilih salah satu)
#    Python 3
python -m http.server 8000

#    Atau Node.js (http-server)
npx http-server .

# 4. Buka di browser
#    http://localhost:8000
