# Rencana Web Portfolio: Stephen Prasetya Chrismawan

> Dokumen perencanaan untuk portfolio interaktif dengan animasi 2D dan JavaScript.
> Disusun: 29 September 2026 · Status: **Draf untuk ditinjau pemilik**

---

## 0. Ringkasan Eksekutif

| Item | Keputusan yang diusulkan |
|---|---|
| **Positioning** | *Odoo Developer & AI Researcher*, "Systems, made human." |
| **Konsep visual** | Portfolio 2D bertema *simulation lab*: grid, agen, kurva, dan jadwal yang bergerak |
| **Tumpuan animasi** | Canvas 2D + GSAP (ScrollTrigger) + SVG/Lottie ringan |
| **Signature interaction** | Tiga demo hidup: agen RL di gridworld, evolusi Genetic Algorithm, dan Gantt job-shop yang menjadwal ulang saat gangguan |
| **Stack** | Vite + TypeScript + Vanilla (tanpa framework berat), Tailwind CSS, GSAP, deploy ke GitHub Pages/Vercel |
| **Bahasa** | Indonesia + Inggris (toggle) |

---

## 1. Hasil Riset: Jejak Digital

### 1.1 Catatan penting soal identitas dan ejaan

Nama yang ditulis sebagai *"Steven Prasetya Krismawan"* hampir tidak menghasilkan temuan yang cocok. Semua sumber yang **terverifikasi** memakai ejaan **"Stephen Prasetya Chrismawan"** (handle GitHub `stephenprasetyachrismawan`, nama yang sama dengan pemilik repo ini). **Pastikan ejaan mana yang ingin dipakai di portfolio.** Rencana ini memakai ejaan yang muncul di sumber resmi.

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

1. **Halaman LinkedIn dan Google Scholar** tidak bisa dibuka otomatis, jadi riwayat kerja, gelar terbaru, dan daftar lengkap publikasi belum terbaca.
2. **Urutan penulis dan DOI** artikel IJRCS belum terkonfirmasi. Peran Anda sebagai penulis (pertama/kedua/dst.) harus diisi sendiri.
3. **Studi lanjut di UGM**: ada indikasi (email `mail.ugm.ac.id`) dan repo `dfjsp_1_from_article`, `thesis-writing-skills`, `My-Lovely_thesis` mengarah ke riset *Dynamic Flexible Job Shop Scheduling* dengan RL. Isi repo tidak bisa saya baca (di luar cakupan sesi), jadi **jangan menulis klaim riset tesis** di portfolio sebelum Anda menyetujui teksnya.
4. **Tempat kerja / pengalaman industri Odoo**: repo `custom_odoo_skills`, `odoo-task-mcp`, `airflow-dbt-example`, `Cogstack-TestCase`, dan `BCATestCodingStephen` menunjukkan aktivitas, tetapi bukan jabatan atau perusahaan.
5. **Minat Reinforcement Learning dan Metaheuristik**: minat Anda tercermin kuat dari skripsi (GA), repo `Genetic-Algorithm`, dan `dfjsp_*`. Belum ada publikasi RL yang terverifikasi, jadi bagian RL ditampilkan sebagai *"Research Interest / In Progress"*, bukan hasil terbit.

### 1.4 Aspek privasi

- Keterlibatan di komunitas gereja (`bible-ppt`, `ppt2liturgi`, GKJ Cilacap Utara) menyangkut data agama. **Default: tidak ditampilkan.** Tampilkan hanya jika Anda memilihnya, misalnya sebagai proyek *"multimedia & tooling untuk komunitas"* tanpa menyebut afiliasi.
- Akun Instagram/Facebook: tidak dimasukkan.
- Repo tugas kuliah (`H1D021025-*`, `Tugas2Praktikum2024`, dll.) memuat NIM. **Jangan ditautkan.**

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
| 4 | **Research** | Skripsi GA, artikel IJRCS, minat RL dan DFJSP | Demo GA dan RL (lihat §5) |
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

**C. Dynamic Rescheduling: Gantt job-shop**

- Gantt chart mesin × waktu dengan operasi berwarna.
- Tombol *"Inject disruption"* (mesin rusak / job baru): jadwal **bergeser dan diperbaiki** dengan animasi, dibandingkan dengan aturan sederhana (misalnya SPT, FIFO).
- Peringatan jujur di UI: *"Demo ilustratif, bukan hasil tesis"* sampai hasil riset resmi tersedia.

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

- `My-Lovely_thesis`, `dfjsp_1_from_article`, `thesis-writing-skills`: terkait riset tesis. Tampilkan hanya jika Anda setuju dan isinya siap publik.
- `bible-ppt`, `ppt2liturgi`: lihat §1.4.
- `BCATestCodingStephen`: tes seleksi perusahaan, sebaiknya disembunyikan.

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
│   │   └── job-shop-gantt/
│   ├── data/              # projects.json, publications.json, timeline.json
│   └── i18n/{id,en}.json
├── tests/
└── .github/workflows/deploy.yml
```

---

## 9. Tahapan Pengerjaan

| Fase | Isi | Hasil |
|---|---|---|
| **0. Konfirmasi** | Jawab pertanyaan di §11, pilih proyek dan gambar | Konten final |
| **1. Fondasi** | Setup Vite/TS/Tailwind, tema, navigasi, tata letak responsif | Kerangka situs berjalan |
| **2. Konten statis** | Hero, About, Timeline, Contact, data proyek dan publikasi, slot gambar placeholder | Portfolio lengkap tanpa demo |
| **3. Animasi global** | Latar jaringan, scroll reveal, kursor, transisi, loader | Situs terasa "hidup" |
| **4. Demo signature** | Demo A (RL), B (GA), C (Gantt) | Bagian Research/Lab interaktif |
| **5. Polesan** | i18n, mode gelap/terang, SEO, OG image, aksesibilitas | Siap publik |
| **6. QA dan rilis** | Lighthouse ≥ 90, uji lintas browser, deploy, domain `stevewithcode.net` | Live |

---

## 10. Kriteria Keberhasilan

- Lighthouse: Performance ≥ 90, Accessibility ≥ 95, SEO ≥ 95.
- Semua slot gambar dapat diganti hanya dengan menimpa file.
- Tiga demo berjalan mulus tanpa *error* dan menghormati *reduced motion*.
- Tidak ada data pribadi sensitif (NIM, afiliasi agama, akun media sosial pribadi) yang tampil tanpa persetujuan.
- Setiap klaim riset dapat ditelusuri ke sumber (repositori, jurnal, atau repo).

---

## 11. Pertanyaan Terbuka untuk Anda

1. Ejaan nama di portfolio: **Stephen Prasetya Chrismawan** (sesuai sumber resmi) atau **Steven Prasetya Krismawan**?
2. Apakah portfolio ini **menggantikan** `stevewithcode.net` atau berdiri sendiri (mis. sebagai versi 2D)?
3. Status studi lanjut (UGM) dan topik tesis yang boleh dipublikasikan?
4. Pekerjaan / pengalaman Odoo (perusahaan, tahun, peran) yang ingin ditampilkan?
5. Peran Anda pada artikel IJRCS 2024 (urutan penulis) dan DOI-nya?
6. Repo mana yang boleh dan tidak boleh tampil (lihat §6.3)?
7. Apakah kegiatan komunitas (multimedia gereja) ingin ditampilkan?
8. Bahasa utama: Indonesia, Inggris, atau dua-duanya?
9. Adakah CV (PDF) yang ingin disediakan untuk diunduh?

---

## Lampiran: Sumber

- [GitHub: stephenprasetyachrismawan](https://github.com/stephenprasetyachrismawan)
- [stevewithcode.net](https://stevewithcode.net)
- [Repositori Unsoed: skripsi](https://repository.unsoed.ac.id/31867/) · [daftar karya penulis](http://repository.unsoed.ac.id/view/creators/CHRISMAWAN=3AStephen_Prasetya=3A=3A.html)
- [IJRCS: Accelerating Convergence in Data Offloading Solutions](https://pdfs.semanticscholar.org/1737/6b7f22135c21b1559a8dcb226304ff6622f0.pdf)
- [Google Scholar](https://scholar.google.com/citations?hl=en&user=EH7NZsgAAAAJ)
- [Cake](https://www.cake.me/users/stephen-prasetya-chrismawan/profile)
