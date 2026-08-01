# Changelog

## v11.0 — 2026-07-26

### Fixes
- **04-habit-loop.md:** `mkdir -p` → `mkdir` — nggak ada parent directory yang perlu dibuat, `-p` misleading. Tracking system path sekarang fleksibel: "misal di ~/belajar-tracker/", "lo bisa taruh di mana aja", "tracker-lo/ ← nama folder bebas, di mana aja."

### Retained from v10
- Semua konten lain tidak berubah.

## v10.0 — 2026-07-26

### Changes
- **Metaphor refined:** "Dispenser Non-Deterministik" → "Vending Machine Non-Deterministik" di seluruh modul (INDEX, 01-mental-model, 05-meta, CHANGELOG). Lebih tepat: lo request (prompt = koin + tombol), AI ngeluarin — kadang sesuai pesanan, kadang meleset (halusinasi). Lo verifikasi sebelum "minum."
- **01-mental-model.md:** "randomness" → "probabilitas" di penjelasan Non-Deterministik — lebih akurat teknis untuk LLM token prediction.
- **02-workflow-belajar.md:** Workflow E Step 5 — "Kalo instruktur pake Express, lo coba Fastify" sekarang ada peringatan: "(JIKA DAN HANYA JIKA lo udah nguasain Express dan mau explore aja. Kewajiban lo ngerti kurikulum dulu, baru eksplorasi)."

### Retained from v9
- Semua konten lain tidak berubah. Tracker system, policy, 3-mode, timeblock — identik.

## v9.0 — 2026-07-26

### Major Changes
- **Tracker system direstruktur — dari `belajar.md` flat ke `~/belajar-tracker/` folder structure**
  - **04-habit-loop.md:** "File belajar.md" section diganti total.
  - **Struktur baru:** Satu folder `~/belajar-tracker/` dengan file per phase (`phase-0.md` s/d `phase-3.md`).
  - **Format entry:** ✅ UDAH BISA / 🎯 LAGI BELAJAR / ❌ STUCK / BUTUH BANTUAN / 📝 NOTES — diorganisir per GC milestone + per tanggal.
  - **Kenapa:** Format lama ("Yang gue kerjain", "Yang gue pelajari") nggak scannable instruktur. Format baru bikin 1-on-1 efisien — instruktur scan 30 detik, langsung tau gap lo.
  - **"Coba Sendiri" di-update:** step 2 sekarang "Setup ~/belajar-tracker/" dengan perintah mkdir + file per phase.
- **Semua referensi tahun dikoreksi:** 2025 → 2026 di INDEX.md, 00-prolog.md, 01-mental-model.md, 04-habit-loop.md, CHANGELOG.md.

### Retained from v8
- Semua konten lain tidak berubah. Judul, tema, policy, 3-mode, timeblock, pitfalls — identik.

## v8.0 — 2026-07-26

### Minor Fixes
- **04-habit-loop.md:**
  - Pitfall 4: "Ngoding pas lecture, sambil dengerin" → "Ngoding pas instruktur lagi jelasin atau demo." Fix text: "Coding-along = pas lab session" → "Coding-along = pas sesi exercise sendiri, bukan pas instruktur lagi demo." (Nggak ada "lab session" di Hacktiv8 — instruktur demoin, lalu student exercise sendiri.)
  - Tracking headers: "JANGAN tracking:" → "JANGAN tracking vanity metrics ini:" dan "TRACKING ini:" → "TRACKING ini (metrics that counts):" — biar beda input kosong vs output nyata makin jelas.
- **INDEX.md:** v8 header, "Yang Baru di v8" section, TOC description update.

### Retained from v7
- Semua konten v7 tidak berubah. Judul, tema, policy, 3-mode, timeblock — semuanya identik.

## v7.0 — 2026-07-26

### Major Changes
- **Judul + tema fundamental diganti:** "AI Itu Vending Machine Informasi Non-Deterministik, Bukan Joki Mikir"
  - Reframing menyeluruh: AI bukan guru, bukan expert — AI itu mesin probabilitas. Lo yang harus mikir.
  - **INDEX.md:** Intro baru ngejelasin kenapa judul ini — "vending machine" vs "guru", "non-deterministik" artinya apa, dan kenapa "joki mikir" lebih bahaya dari sekadar "joki."
  - **01-mental-model.md:** Section baru "AI Itu Vending Machine, Bukan Guru" — tabel 4 mental model (guru/expert/joki/vending machine) dengan akibat masing-masing. Sycophant problem sekarang dibingkai sebagai "efek dari sifat non-deterministik."
- **Policy Hacktiv8 dikoreksi — phase-aware:**
  - Phase 0, 1, Phase 2 (minggu 1-2): ❌ no AI di tugas
  - Phase 2 (minggu 3+) dan Phase 3: ✅ AI BOLEH di tugas — kecuali livecode
  - Livecode: ❌ selalu no AI, di semua phase
  - **01-mental-model.md:** Warning section jadi "Aturan AI di Hacktiv8 — Phase-Aware" dengan dua aturan praktis (phase awal vs phase lanjut). Aturan JANGAN sekarang bedakan: repo tugas Phase awal, livecode semua phase, dan joki mikir Phase lanjut.
  - **03-bootcamp-survival.md:** Section "REALITAS" diganti — ✅/❌ rules sekarang punya 3 kategori: BOLEH DI SEMUA PHASE, BOLEH MULAI PHASE 2 WEEK 3+, JANGAN DI SEMUA PHASE.
- **Kamus:** +1 istilah baru (Non-Deterministik), +3 istilah di-update (Sycophant Problem, Repo Latihan vs Repo Tugas, Post-Tugas Review). Total: 38+ istilah.

### Retained from v6
- 3-Mode SURVIVE/STRETCH/PROVE framework (tidak berubah)
- Bootcamp Timeblock, 4 Pitfalls, Spaced Repetition (tidak berubah)
- AI-dikasih-konteks di Latihan 2, 3, 5 (tidak berubah)
- Semua bagian lain (0, 2, 4) tidak berubah

### Major Changes
- **⚠️ Policy Hacktiv8 diakomodasi — "pisahin belajar dari nugas"**
  - **01-mental-model.md direstruktur:**
    - Section baru di awal: "⚠️ PENTING: Pisahin Belajar dari Nugas" — golden rule repo tugas ≠ repo belajar
    - Semua kata "tugas" → "sesi latihan" / "topik belajar"
    - 3-mode sekarang bingkai-nya: "3 Mode dalam 1 Sesi Belajar" (bukan "dalam 1 Tugas")
    - **Dua skenario:** Skenario A (Latihan Mandiri — weekend/malam) + Skenario B (Post-Tugas Review — abis ngumpulin, copy ke ~/review/)
    - Learning Target template sekarang punya ⚠️ footer: "INI DI FOLDER LATIHAN — bukan repo tugas"
    - Aturan main: tambah baris "Repo tugas asli — dalam bentuk apa pun" di kolom JANGAN
  - **03-bootcamp-survival.md diperkuat:**
    - Section baru: "⚠️ REALITAS: Nggak Boleh Pake AI Pas Nugas" dengan ✅ BOLEH / ❌ JANGAN konkret
    - Real Talk direframe: "lo nggak bisa pake AI. Dan itu bagus."
    - Semua template prompt tetap ada — diperjelas buat konteks Post-Tugas Review
- **05-meta.md: AI sekarang dikasih konteks modul**
  - Latihan 2 (Feynman AI): +step paste modul ke AI dulu, baru lo jelasin dari ingatan → AI bandingin, feedback akurat
  - Latihan 3 (Quiz Yourself): +step paste modul → soal spesifik ke isi modul, bukan generic
  - Latihan 5 (Ajarin Temen ke AI): split 2 tahap — Tahap 1 tanpa konteks (tes kejelasan), Tahap 2 dengan modul (tes akurasi)
- **Kamus tambahan:** +2 istilah (Repo Latihan vs Repo Tugas, Post-Tugas Review)

### Retained from v5
- Semua bagian lain (0, 2, 4, APPENDIX) tidak berubah
- Bootcamp Timeblock, 4 Pitfalls, Spaced Repetition system tetap sama
- 3-Mode konsep SURVIVE/STRETCH/PROVE tetap sama — cuma framing-nya yang direpair

### Major Changes
- **Bagian 4 direstruktur total — Bootcamp-Aware Timeblock**
  - **Dihapus:** "3 Timeblock Harian" generic (Pagi Project / Siang Study / Malam Reflect). Nggak realistis buat mahasiswa yang dikuasai bootcamp dari jam 9 pagi sampai jam 4-6 sore.
  - **Diganti:** Sistem yang di-align ke realita jadwal bootcamp Hacktiv8:
    - **2 Skenario Weekday:** "Selesai jam 4 sore" (ada slot Deep Study + SURVIVE) vs "Stretch jam 6 sore" (pilih satu: SURVIVE atau Deep Study)
    - **Weekend Golden Hours:** Sabtu 09:00-12:00 STRETCH + PROVE, 14:00-16:00 DEEP STUDY + Spaced Repetition Review. Minggu bebas.
    - **Istirahat explicit:** 90 menit non-negotiable setelah bootcamp dijadwalkan + justifikasi ilmiah (cognitive fatigue)
  - **4 Pitfall spesifik bootcamp:** Deep Study skip, begadang, Sabtu males, coding pas lecture. Masing-masing dengan "mental lo" vs "realita" + fix.
  - **Spaced Repetition di-align ke minggu bootcamp:** hari 1 & 3 = weekday malam 30 menit, hari 7 & 14 = Sabtu siang (review mingguan), hari 30 = weekend kosong.
- **Kamus tambahan:** +2 istilah (Golden Hours, Bootcamp-Weekday)

### Retained from v4
- Ebbinghaus curve + Dunlosky meta-review
- Progress tracking (belajar.md)
- Social accountability
- Transisi pasca-bootcamp
- Semua bagian lain (0, 1, 2, 3, 5, APPENDIX) tidak berubah

## v4.0 — 2026-07-26

### Major Changes
- **Bagian 1 direstruktur total — "3 Mode dalam 1 Tugas" (SURVIVE / STRETCH / PROVE)**
  - **Dihapus:** Level 0→1→2→3 dengan timeline 3-bulan. Nggak realistis buat bootcamp 12 minggu.
  - **Diganti:** Sistem 3 mode yang di-toggle dalam satu tugas yang sama:
    - **SURVIVE (~20% waktu):** Komponen yang lo udah bisa. AI generate → lo review paham.
    - **STRETCH (~60% waktu):** 1-2 konsep baru target belajar. LO ngetik, AI navigasi.
    - **PROVE (~20% waktu):** Validasi mandiri. Lo kerjain sendiri, AI review setelahnya.
  - **Learning Target template** — wajib tulis sebelum mulai tugas: 🎯 STRETCH / ⚡ SURVIVE / ✅ PROVE
  - **Contoh konkret** — simulasi tugas e-commerce REST API dengan ketiga mode
  - **Aturan main di-mapping ke 3 mode** — kapan AI boleh generate, kapan harus sparring, kapan off total

### Retained from v3
- Semua bagian lain (0, 2, 3, 4, 5, APPENDIX) tetap sama
- AI sycophant problem, 4 trik anti-sycophant, tes 5 menit, async/await
- Semua footnotes & cross-reference navigation

### Kamus Update
- 05-meta.md: nambah 4 istilah baru (SURVIVE mode, STRETCH mode, PROVE mode, Learning Target)

### Major Additions
- **Bagian 5: 05-meta.md — Kamus Istilah + Baca Ulang dengan Teknik Modul**
  - **Part 1 — KAMUS ISTILAH:** 30+ istilah dijelasin pake bahasa lo, dibagi 3 kolom:
    - 🧠 Konsep Belajar & Psikologi Kognitif (illusion of competence, active recall, spaced repetition, Ebbinghaus curve, desirable difficulty, dll)
    - 🤖 Istilah AI & Tools (tutorial hell, vibe coding hell, sycophant problem, agent mode, AI hallucination, dll)
    - 💻 Istilah Teknis (async/await, Promise, middleware, JWT, ORM, stack trace, dll)
  - **Part 2 — BACA ULANG MODUL:** 5 latihan meta-learning:
    1. Compress & Structure: bikin rangkuman 1 halaman dari ingatan
    2. Feynman AI: jelasin isi modul ke AI guru killer
    3. Quiz Yourself: AI bikinin 15 soal tentang modul, lo jawab
    4. Spaced Repetition: setup jadwal review 30 hari buat isi modul
    5. Ajarin Temen: jelasin modul ke orang lain (atau AI)
  - **Ceklis final** — centang semua sebelum tutup modul
- Cross-reference navigation diperkuat: INDEX → Kamus, 04 → 05 → APPENDIX

### Changes
- INDEX.md: update versi ke v3, tambah Bagian 5 di TOC, tambah cara baca (ke Kamus + latihan)
- 04-habit-loop.md: footer update ke Bagian 5
- APPENDIX.md: footer update ke Bagian 5

## v2.0 — 2026-07-26

### Major Additions
- **Vibe Coding Hell** (Bagian 0): Evolusi dari tutorial hell — "gue nggak bisa ngoding tanpa Cursor/Copilot." Riset 2026 dari arXiv + Boot.dev.
- **AI Sycophant Problem** (Bagian 1): AI selalu setuju sama lo, ini bahaya buat belajar. Plus 4 trik buat maksa AI jadi kritis.
- **Ebbinghaus Forgetting Curve** (Bagian 0 + 4): Scientific backing kenapa lo lupa 70% dalam 24 jam. Data konkret.
- **Spaced Repetition Schedule** (Bagian 4): Jadwal review 1-3-7-14-30 dengan template prompt AI scheduler.
- **Workflow E: Tutorial Right Way** (Bagian 2): 5 step belajar dari tutorial tanpa terjebak, dari freeCodeCamp.
- **Vibe Coding Check** (Bagian 3): Quick self-audit sebelum submit tugas.
- **APPENDIX.md**: Prompt template library (11 template) + curated resource links + tools rekomendasi.

### Fixes
- **Semua contoh async/await**: Nggak ada lagi `.then()` / `.catch()` jadul. Semua analogi Promise di-update ke pola modern.
- **Prompt examples**: Semua contoh prompt di-refine dengan pattern yang lebih kritis (anti-sycophant).
- **Struktur diperkuat**: Cross-reference antar file lebih jelas.

### Removals
- Nggak ada yang dihapus dari v1 secara substansi. Semua konten v1 tetap ada, di-enhanced.

## v1.0 — 2026-07-26

### Initial Release
- 5 file: INDEX, 00-prolog, 01-mental-model, 02-workflow-belajar, 03-bootcamp-survival, 04-habit-loop
- 4 workflow: Project-First, Feynman AI, Quiz Yourself, Compress & Structure
- Target: bootcamp student (failing students)
- Bahasa Indonesia casual (gue/lo)
