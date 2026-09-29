# Rencana Web Portfolio: Stephen Prasetya Chrismawan

> Dokumen perencanaan untuk portfolio interaktif dengan animasi 2D dan JavaScript.
> Disusun: 29 September 2026 · Revisi 2: keputusan pemilik sudah dimasukkan (lihat §11) · Status: **Siap dikerjakan, menunggu data LinkedIn**

---

## 0. Ringkasan Eksekutif

| Item | Keputusan yang diusulkan |
|---|---|
| **Nama di situs** | **Stephen Prasetya Chrismawan** (menggantikan `stevewithcode.net`) |
| **Positioning** | *Odoo Developer & AI Researcher*, mahasiswa S2 Master of Computer Science UGM, "Systems, made human." |
| **Konsep visual** | Portfolio 2D bertema *simulation lab*: grid, agen, kurva, dan jadwal yang bergerak |
| **Tumpuan animasi** | Canvas 2D + GSAP (ScrollTrigger) + SVG/Lottie ringan |
| **Signature interaction** | Tiga demo hidup: agen RL di gridworld, evolusi Genetic Algorithm, dan pencarian rute metaheuristik (TSP) |
| **Stack** | Vite + TypeScript + Vanilla (tanpa framework berat), Tailwind CSS, GSAP, deploy ke GitHub Pages/Vercel |
| **Bahasa** | Indonesia + Inggris (toggle, dua-duanya wajib) |
| **Topik tesis** | **Tidak dipublikasikan.** Cukup ditulis "sedang studi S2 Master of Computer Science, UGM" |

---

## 1. Hasil Riset: Jejak Digital

### 1.1 Catatan penting soal identitas dan ejaan

Nama yang ditulis sebagai *"Steven Prasetya Krismawan"* hampir tidak menghasilkan temuan yang cocok. Semua sumber yang **terverifikasi** memakai ejaan **"Stephen Prasetya Chrismawan"** (handle GitHub `stephenprasetyachrismawan`). **Keputusan pemilik: ejaan resmi yang dipakai adalah Stephen Prasetya Chrismawan.** Metadata SEO menyertakan variasi *"Steven Prasetya Krismawan"* agar tetap mudah ditemukan lewat pencarian.

**Bukan Anda (jangan dimasukkan ke portfolio):**

- `github.com/stevenpjg`: hasil pencarian sempat mengaitkannya dengan Anda, tetapi tidak ada bukti; itu akun orang lain (pemilik repo implementasi DDPG).
- Steven Prasetya (VP Marketing, Black Wolves Capital), Steven Prasetya (Humber College, Kanada), Steven Prasetya (LSPR), dan sejenisnya: orang berbeda.

### 1.2 Temuan yang terverifikasi

| Sumber | Temuan | Tautan |
|---|---|---|
| **GitHub** | Akun `stephenprasetyachrismawan`, lokasi Yogyakarta, bio *"Small commits. Unreasonable curiosity."*, tagline *"Do you want P1?"*, 46 repo publik, badge Pull Shark ×3, Pair Extraordinaire ×3, YOLO, Quickdraw, situs `stevewithcode.net` | [github.com/stephenprasetyachrismawan](https://github.com/stephenprasetyachrismawan) |
| **Situs pribadi** | Portfolio imersif yang sudah ada: *"Systems engineer and AI researcher"*, peran utama **Odoo developer**, minat *"intelligent systems that adapt to changing circumstances"*, motto *"Systems, made human."*, enam bagian: Origin, Build, Research, Systems, Apps, Profile | [stevewithcode.net](https://stevewithcode.net) |
| **Repositori Unsoed** | Skripsi S1 Teknik Informatika (2025): *Greedy-Guided Genetic Algorithm untuk Optimasi Data Offloading pada Edge Caching Network*. Pembimbing: Mulki Indana Zulfa dan Nur Alfi Ekowati. Hasil: GA *half-greedy* unggul dalam median fitness, hit ratio, dan Latency Saving Ratio dibanding GA klasik dan *full-greedy* pada empat dataset | [repository.unsoed.ac.id/31867](https://repository.unsoed.ac.id/31867/) |
| **Jurnal** | *Accelerating Convergence in Data Offloading Solutions: A Greedy-Assisted Genetic Algorithm Approach*, International Journal of Robotics and Control Systems (IJRCS), Vol 4 No 4 (2024), hlm. 1934–1946. Penulis pertama tercatat Mulki Indana Zulfa | [PDF](https://pdfs.semanticscholar.org/1737/6b7f22135c21b1559a8dcb226304ff6622f0.pdf) |
| **Google Scholar** | Profil ada, afiliasi email `mail.ugm.ac.id`, minat Computer Science dan Algorithms | [scholar](https://scholar.google.com/citations?hl=en&user=EH7NZsgAAAAJ) |
| **Cake** | Mahasiswa Teknik Informatika, belajar pemrograman web, anggota tim Multimedia GKJ Cilacap Utara | [cake.me](https://www.cake.me/users/stephen-prasetya-chrismawan/profile) |
| **LinkedIn** | `in/stephen-prasetya-chrismawan-84bb2419b` (tertaut dari GitHub) | tidak dapat dibaca otomatis (HTTP 999) |

### 1.3 Yang belum bisa diverifikasi (mohon dilengkapi)

1. **Halaman LinkedIn dan Google Scholar** tidak bisa dibuka otomatis (LinkedIn menolak dengan HTTP 999). Pemilik menyatakan data studi dan pengalaman "sesuai LinkedIn", jadi **teks final untuk Timeline dan pengalaman Odoo perlu disalin dari LinkedIn** (judul jabatan, perusahaan, periode). Sampai itu tersedia, Timeline memakai data placeholder yang ditandai `TODO`.
2. **Artikel IJRCS**: pemilik menyatakan sebagai **penulis pertama**. Tetapi hasil pencarian mencantumkan Mulki Indana Zulfa sebagai penulis pertama di halaman artikel. Perbedaan ini bisa karena urutan yang salah terbaca oleh mesin pencari, tetapi **cek PDF terbit sebelum sitasi dipublikasikan**, dan salin sitasi serta DOI persis seperti tertulis di sana.
3. **Studi lanjut**: ditulis hanya sebagai *"Mahasiswa S2 Master of Computer Science, Universitas Gadjah Mada"* (sesuai LinkedIn). **Topik tesis tidak ditulis** dan repo terkait tesis tidak ditampilkan.
4. **Pengalaman industri Odoo**: repo `custom_odoo_skills`, `odoo-task-mcp`, `airflow-dbt-example`, dan `Cogstack-TestCase` menunjukkan aktivitas teknis, tetapi bukan jabatan atau perusahaan. Ambil dari LinkedIn (poin 1).
5. **Minat Reinforcement Learning dan Metaheuristik**: tercermin dari skripsi (GA) dan repo `Genetic-Algorithm`. Belum ada publikasi RL yang terverifikasi, jadi RL ditampilkan sebagai *"Research Interest"* lewat demo interaktif, bukan sebagai hasil terbit.

### 1.4 Aspek privasi

- Keterlibatan di komunitas gereja (`bible-ppt`, `ppt2liturgi`, GKJ Cilacap Utara): **keputusan pemilik: tidak ditampilkan.**
- Akun Instagram/Facebook: tidak dimasukkan.
- Repo tugas kuliah (`H1D021025-*`, `Tugas2Praktikum2024`, dll.) memuat NIM dan nama lengkap di deskripsi. Pemilik mengizinkan repo publik tampil, tetapi **rekomendasi: repo tugas kuliah tetap disaring** karena nilai portfolionya rendah dan memuat NIM. Pemilik dapat membalik keputusan ini di §6.3.

---

## 2. Positioning dan Narasi

**Tagline:** *Systems, made human.*
**Sub-tagline:** Odoo developer yang meneliti sistem cerdas yang beradaptasi, dari metaheuristik sampai reinforcement learning.

**Tiga pilar cerita:**

1. **Build**: sistem enterprise nyata (Odoo, ERP, integrasi data, aplikasi web dan mobile).
2. **Research**: optimasi dan pembelajaran mesin (Genetic Algorithm, metaheuristik, RL, penjadwalan dinamis).
3. **Human**: teknologi yang mudah dipakai orang, sesuai motto dan gaya bio *"Small commits. Unreasonable curiosity."*

Nada tulisan: profesional, hangat, ringkas. Hindari klaim besar tanpa bukti.

---

## 3. Arsitektur Informasi

Satu halaman *single-page* dengan navigasi anchor, mempertahankan enam bagian situs lama supaya konsisten dengan `stevewithcode.net`.

| # | Bagian | Isi | Animasi kunci |
|---|---|---|---|
| 1 | **Hero / Origin** | Nama, tagline, foto profil, CTA (*Lihat Proyek*, *Unduh CV*) | Grid 2D interaktif: agen kecil mengikuti kursor lalu "belajar" jalur ke tujuan; teks muncul per huruf |
| 2 | **About** | Cerita singkat, statistik (repo, tahun, publikasi), skill | Counter naik saat masuk viewport, kartu foto *tilt* |
| 3 | **Build (Odoo & Software)** | Proyek Odoo, web, mobile, data engineering | Kartu proyek dengan *hover-reveal* dan filter animasi |
| 4 | **Research** | Skripsi S1 (GA), artikel IJRCS (penulis pertama), minat RL dan metaheuristik, status S2 UGM | Demo GA, RL, dan TSP (lihat §5) |
| 5 | **Systems / Lab** | Tiga demo interaktif dalam satu panel tab | Canvas 2D real-time |
| 6 | **Apps** | Aplikasi lengkap (FinJumper, WareHouse-Koperasi, PDFHolmes, dll.) | Carousel horizontal dengan *scroll pinning* |
| 7 | **Timeline** | Pendidikan, riset, pekerjaan | Garis waktu yang tergambar mengikuti scroll (SVG *stroke-dashoffset*) |
| 8 | **Profile / Contact** | Tautan GitHub, LinkedIn, Scholar, email, form kontak | *Magnetic button*, konfeti kecil saat kirim |

---

## 4. Desain Visual

### 4.1 Arah kreatif: *"Simulation Lab"*

Estetika 2D datar dengan grid teknis: garis halus, titik agen, kurva reward. Menggabungkan kesan **engineer** (presisi, grid) dan **manusiawi** (bentuk membulat, warna hangat).

### 4.2 Palet (usulan, dengan mode gelap dan terang)

| Peran | Gelap | Terang |
|---|---|---|
| Latar | `#0B0F1A` | `#F7F8FB` |
| Permukaan | `#141A2B` | `#FFFFFF` |
| Teks | `#E6EAF5` | `#111827` |
| Aksen utama (agen/RL) | `#5EEAD4` | `#0F766E` |
| Aksen kedua (GA/evolusi) | `#F59E0B` | `#B45309` |
| Aksen ketiga (Odoo/ERP) | `#A78BFA` | `#6D28D9` |

Pertahankan rasio kontras WCAG AA (≥ 4.5:1 untuk teks).

### 4.3 Tipografi

- Judul: **Space Grotesk** atau **Sora**
- Isi: **Inter**
- Kode/angka: **JetBrains Mono**

---

## 5. Rencana Animasi (2D dan JavaScript)

### 5.1 Animasi global

| Efek | Teknik | Catatan |
|---|---|---|
| Latar grid bergerak | `<canvas>` 2D, `requestAnimationFrame` | Titik saling terhubung dalam radius (efek jaringan); jumlah titik menyesuaikan lebar layar |
| Reveal saat scroll | GSAP + ScrollTrigger | Fade-up, stagger, *pin* untuk section Apps |
| Pergantian halaman/section | GSAP timeline | Transisi *clip-path* |
| Kursor kustom | JS + CSS `transform` | Berubah bentuk di atas elemen interaktif; dimatikan di layar sentuh |
| Micro-interaction | CSS + Web Animations API | Tombol magnetik, *tilt* kartu, *underline draw* |
| Loader | SVG path animasi | Logo/inisial "SP" tergambar |

### 5.2 Tiga demo signature (bagian Research/Lab)

Ketiganya ditulis dengan **Canvas 2D murni** (tanpa library ML) agar ringan dan mudah dijelaskan.

**A. Reinforcement Learning: Gridworld Q-Learning**

- Grid 12×8, agen mencari tujuan, ada dinding dan jebakan.
- Q-table divisualisasikan sebagai warna sel dan panah kebijakan.
- Kontrol: *learning rate*, *epsilon*, *discount*, tombol *Reset / Train / Speed*.
- Grafik reward per episode di sisi kanan (sparkline canvas).
- Pesan naratif: *"Agen belajar dari trial and error"*.

**B. Metaheuristik: evolusi Genetic Algorithm**

- Populasi titik pada permukaan fitness 2D (peta kontur) yang berevolusi lewat seleksi, crossover, mutasi.
- Perbandingan **GA klasik vs Greedy-Guided (half-greedy)**: dua panel berdampingan, kurva konvergensi ditampilkan langsung. Ini menerjemahkan skripsi dan artikel IJRCS Anda menjadi cerita visual.
- Kontrol: ukuran populasi, laju mutasi, inisialisasi greedy (0 / 50 / 100%).

**C. Metaheuristik: pencarian rute (Traveling Salesman Problem)**

- Kota acak di kanvas; klik untuk menambah/memindah kota.
- Pilih algoritma: **Simulated Annealing**, **Ant Colony Optimization**, atau **2-opt**. Rute terbaik digambar ulang saat membaik, dan panel di samping menampilkan jarak terbaik per iterasi.
- Ini sengaja **tidak memakai topik tesis** (sesuai keputusan pemilik); TSP adalah contoh metaheuristik klasik yang mudah dipahami pengunjung awam.
- Label UI: *"Demo ilustratif untuk metaheuristik."*

### 5.3 Prinsip kinerja dan aksesibilitas

- Target: LCP < 2,5 dtk, CLS < 0,1, 60 fps di laptop menengah.
- Hormati `prefers-reduced-motion`: animasi dimatikan atau diganti transisi sederhana.
- Jeda otomatis canvas saat di luar viewport (`IntersectionObserver`) dan saat tab tidak aktif.
- Turunkan jumlah partikel di perangkat seluler; gunakan `devicePixelRatio` terbatas (maks. 2).
- Semua kontrol dapat diakses keyboard, dengan label ARIA; demo punya deskripsi teks.

---

## 6. Showcase Proyek dari GitHub

Diambil dari 46 repo publik. Dikelompokkan dan diprioritaskan; **repo tugas kuliah tidak ditampilkan**.

### 6.1 Featured (kartu besar)

| Proyek | Bahasa | Deskripsi tampilan | Kategori |
|---|---|---|---|
| **WareHouse-Koperasi** | PHP | Sistem manajemen gudang koperasi *(repo yang Anda sematkan)* | Build |
| **FinJumper** | TypeScript | Aplikasi pencatat keuangan dengan fitur lanjutan | Apps |
| **PDFHolmes** | TypeScript | Alat penelusuran PDF (terbaru: Juni 2026) | Apps |
| **openmrs-tfidf-ngram** | TeX | Fitur pencarian OpenMRS dengan TF-IDF dan n-gram yang toleran salah ketik | Research |
| **odoo-task-mcp** | Python | Integrasi tugas Odoo dengan MCP (agen AI) | Odoo |
| **custom_odoo_skills** | Python | Kumpulan *skill* kustom untuk Odoo | Odoo |
| **Genetic-Algorithm** | Python | Implementasi GA (dasar untuk demo B) | Research |

### 6.2 Sekunder (kartu kecil / daftar)

`airflow-dbt-example` (Airflow + dbt + DuckDB), `Cogstack-TestCase`, `employee_promotion_react_native`, `taskman`, `preZensia` (kolaborasi dengan Irfan), `LookUp-Finding-App`, `PCD_ProjekKelompok`, `LinearRegression`, `dsc_2025`.

### 6.3 Perlu keputusan Anda

Kebijakan: **repo publik boleh tampil**, dengan pengecualian berikut (bisa diubah pemilik):

- **Tidak ditampilkan (keputusan pemilik):** tiga repo terkait tesis (`My-Lovely_thesis`, `thesis-writing-skills`, dan satu repo lain; daftar lengkap disimpan di `hidden` pada `projects.json`), `bible-ppt`, `ppt2liturgi` (komunitas).
- **Tidak ditampilkan (rekomendasi):** repo tugas kuliah berNIM (`H1D021025-*`, `Tugas2Praktikum2024`, `MobileLab*`, `*_UTSMobile_*`, dan sejenisnya) serta `BCATestCodingStephen` (tes seleksi perusahaan).
- **Otomatis mengikuti aturan di atas:** repo baru pada masa depan tampil kecuali masuk daftar `hidden` di `projects.json`.

### 6.4 Cara data proyek diambil

1. **Statis (disarankan untuk versi 1):** file `src/data/projects.json` dikurasi manual (judul, deskripsi, tag, gambar, tautan).
2. **Otomatis (tahap lanjut):** *fetch* GitHub REST API saat *build* (bukan di browser) untuk bintang, bahasa, dan tanggal *push*, dengan *cache* agar tidak kena *rate limit*.

---

## 7. Slot Gambar (bisa Anda unggah sendiri)

Semua gambar berada di `public/assets/images/`. Selama belum ada gambar asli, dipakai **gambar contoh** (placeholder) dengan nama file yang sama, sehingga cukup **ditimpa** tanpa mengubah kode.

| Slot | Nama file | Rasio / ukuran | Isi ideal | Placeholder sementara |
|---|---|---|---|---|
| Foto profil (hero) | `profile/hero.jpg` | 4:5, ≥ 1200×1500 | Foto formal-santai, latar polos | avatar siluet/inisial "SP" |
| Foto profil (about) | `profile/about.jpg` | 1:1, ≥ 800×800 | Foto sedang bekerja | siluet |
| Avatar kecil (nav) | `profile/avatar.png` | 1:1, 256×256 | Crop wajah | inisial "SP" |
| Foto OG / share | `og/cover.jpg` | 1200×630 | Nama + tagline | kartu bergradien |
| Thumbnail proyek | `projects/<slug>.png` | 16:10, 1280×800 | Tangkapan layar aplikasi | gambar abu-abu berlabel nama proyek |
| Publikasi | `research/<slug>.png` | 4:3, 1024×768 | Sampul jurnal / grafik hasil | ikon dokumen |
| Sertifikat/penghargaan | `awards/<slug>.jpg` | bebas | Sertifikat | kotak kosong |
| Galeri (opsional) | `gallery/01.jpg`… | 3:2 | Kegiatan, konferensi | abu-abu |

**Panduan unggah:**

- Format: JPG/WebP untuk foto, PNG/SVG untuk tangkapan layar dan ikon.
- Ukuran maksimum: 500 KB per foto (skrip build akan membuat versi `.webp` dan `srcset` otomatis).
- Semua gambar wajib punya `alt` teks (dikelola di `projects.json`).
- Untuk foto profil, tambahkan **bingkai animasi** (cincin gradien berputar pelan) yang tetap tampil baik dengan gambar apa pun.

---

## 8. Stack Teknis

| Lapisan | Pilihan | Alasan |
|---|---|---|
| Build | **Vite** + **TypeScript** | Cepat, tipe aman untuk kode simulasi |
| UI | HTML semantik + **Tailwind CSS** | Konsisten, mudah tema gelap/terang |
| Animasi | **GSAP** (+ ScrollTrigger), Canvas 2D, Web Animations API | Kontrol presisi, performa baik |
| Demo | Modul TS murni (`rl/`, `ga/`, `scheduling/`) | Tanpa dependensi ML, mudah diuji |
| Konten | JSON/Markdown di `src/data` | Edit tanpa menyentuh kode |
| i18n | Kamus JSON `id` / `en` | Toggle bahasa |
| Kualitas | ESLint, Prettier, Vitest, Playwright, Lighthouse CI | Pengujian otomatis |
| Deploy | **GitHub Pages** (GitHub Actions) atau Vercel | Gratis, otomatis setiap *push* |
| Analitik | Plausible/Umami (opsional) | Ramah privasi |

**Struktur folder yang diusulkan:**

```
2DPortfolio/
├── PORTFOLIO_PLAN.md
├── index.html
├── public/assets/{images,cv,fonts}/
├── src/
│   ├── main.ts
│   ├── styles/
│   ├── components/        # nav, hero, cards, timeline, footer
│   ├── animations/        # background-network, cursor, scroll, loader
│   ├── demos/
│   │   ├── rl-gridworld/
│   │   ├── ga-evolution/
│   │   └── tsp-metaheuristic/
│   ├── data/              # projects.json, publications.json, timeline.json
│   └── i18n/{id,en}.json
├── tests/
└── .github/workflows/deploy.yml
```

---

## 9. Tahapan Pengerjaan

| Fase | Isi | Hasil |
|---|---|---|
| **0. Konfirmasi** | Keputusan pemilik sudah masuk (§11). Sisa: salin data LinkedIn dan cek sitasi IJRCS | Konten final |
| **1. Fondasi** | Setup Vite/TS/Tailwind, tema, navigasi, tata letak responsif | Kerangka situs berjalan |
| **2. Konten statis** | Hero, About, Timeline, Contact, data proyek dan publikasi, slot gambar placeholder | Portfolio lengkap tanpa demo |
| **3. Animasi global** | Latar jaringan, scroll reveal, kursor, transisi, loader | Situs terasa "hidup" |
| **4. Demo signature** | Demo A (RL), B (GA), C (TSP metaheuristik) | Bagian Research/Lab interaktif |
| **5. Polesan** | i18n ID/EN, mode gelap/terang, SEO (termasuk variasi ejaan nama), OG image, aksesibilitas, halaman CV (§12) | Siap publik |
| **6. QA dan rilis** | Lighthouse ≥ 90, uji lintas browser, deploy, **pindahkan domain `stevewithcode.net`** ke situs baru dengan pengalihan dari URL lama (§13) | Live |

---

## 10. Kriteria Keberhasilan

- Lighthouse: Performance ≥ 90, Accessibility ≥ 95, SEO ≥ 95.
- Semua slot gambar dapat diganti hanya dengan menimpa file.
- Tiga demo berjalan mulus tanpa *error* dan menghormati *reduced motion*.
- Tidak ada data pribadi sensitif (NIM, afiliasi agama, akun media sosial pribadi) yang tampil tanpa persetujuan.
- Setiap klaim riset dapat ditelusuri ke sumber (repositori, jurnal, atau repo).

---

## 11. Keputusan Pemilik

| # | Pertanyaan | Keputusan |
|---|---|---|
| 1 | Ejaan nama | **Stephen Prasetya Chrismawan** |
| 2 | Hubungan dengan `stevewithcode.net` | **Menggantikan** situs lama |
| 3 | Studi lanjut | Cukup *"Mahasiswa S2 Master of Computer Science, UGM"*, **tanpa topik tesis** |
| 4 | Pengalaman Odoo | Mengikuti LinkedIn (data perlu disalin, lihat §1.3) |
| 5 | Peran di artikel IJRCS | Penulis pertama (verifikasi terhadap PDF, lihat §1.3) |
| 6 | Repo yang tampil | Repo publik boleh tampil, dengan penyaringan di §6.3 |
| 7 | Kegiatan komunitas gereja | **Tidak ditampilkan** |
| 8 | Bahasa | **Indonesia dan Inggris** |
| 9 | CV unduhan | Belum ada, akan dibuatkan (§12) |

## 12. CV yang Dapat Diunduh

Pemilik belum punya CV. Rencana:

1. Halaman `/cv` di situs ini dibangun dari data yang sama dengan Timeline dan Publikasi (`timeline.json`, `publications.json`), lengkap dengan stylesheet `@media print`.
2. Tombol *Unduh CV* menghasilkan PDF (dari halaman `/cv` lewat Playwright saat *build*) dan menyimpannya di `public/assets/cv/`.
3. Sebelum data LinkedIn masuk, tombol menampilkan status *"CV segera hadir"* (nonaktif) agar tidak mengirim CV yang isinya kosong.
4. CV tersedia dalam dua bahasa (ID/EN).

## 13. Migrasi dari `stevewithcode.net`

- Situs lama memiliki bagian Origin, Build, Research, Systems, Apps, Profile. Semuanya sudah terpetakan di §3, jadi tidak ada konten yang hilang.
- Pertahankan URL lama yang mungkin sudah dibagikan (jika ada halaman selain beranda) dengan pengalihan 301 atau anchor yang sepadan.
- Ambil dulu salinan konten situs lama (teks yang belum terbaca lengkap oleh riset ini) sebelum diganti, agar tidak ada teks penting yang terlewat.
- Ganti domain hanya setelah situs baru lolos QA (Fase 6).

---

## Lampiran: Sumber

- [GitHub: stephenprasetyachrismawan](https://github.com/stephenprasetyachrismawan)
- [stevewithcode.net](https://stevewithcode.net)
- [Repositori Unsoed: skripsi](https://repository.unsoed.ac.id/31867/) · [daftar karya penulis](http://repository.unsoed.ac.id/view/creators/CHRISMAWAN=3AStephen_Prasetya=3A=3A.html)
- [IJRCS: Accelerating Convergence in Data Offloading Solutions](https://pdfs.semanticscholar.org/1737/6b7f22135c21b1559a8dcb226304ff6622f0.pdf)
- [Google Scholar](https://scholar.google.com/citations?hl=en&user=EH7NZsgAAAAJ)
- [Cake](https://www.cake.me/users/stephen-prasetya-chrismawan/profile)
