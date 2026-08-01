# AI Itu Vending Machine Informasi Non-Deterministik, Bukan Joki Mikir — v11

## Cara Belajar dengan AI Tanpa Nge-bodohin Diri Sendiri

**Versi:** v11.0
**Target:** Bootcamp student (pemula-sedang, termasuk failing students)
**Bahasa:** Indonesia casual (gue/lo)
**Estimasi baca:** 45-60 menit penuh (termasuk latihan di Bagian 5)

---

### Kenapa Judulnya Kayak Gitu

AI itu bukan guru. Serius. AI nggak "ngerti" apa yang lo tanya. AI nggak "mikir." AI itu **vending machine informasi non-deterministik** — mesin yang ngeluarin teks berdasarkan probabilitas. Lo kasih prompt, dia ngeluarin output. Outputnya BEDA-BEDA tiap kali — meskipun promptnya sama persis. Itu artinya non-deterministik. Dia nggak punya jawaban "benar" yang konsisten. Dia cuma nebak token berikutnya.

Kenapa ini penting? Karena kalo lo nganggep AI sebagai "guru"...

- **Lo percaya outputnya mentah-mentah.** Padahal AI bisa halusinasi.
- **Lo nggak verifikasi.** Karena guru kan harusnya bener. AI nggak.
- **Lo nyerahin proses mikir lo.** "AI udah jelasin, berarti gue udah ngerti." Padahal AI cuma vending machine — dia ngeluarin kata-kata, bukan pemahaman.

Tapi kalo lo nganggep AI sebagai **vending machine informasi non-deterministik**...

- **Lo selalu verifikasi.** Karena lo tau outputnya probabilistik, bukan kebenaran.
- **Lo yang mikir.** AI cuma supply bahan mentah. Lo yang proses, lo yang sintesis, lo yang simpulin.
- **Lo pake AI dengan strategi.** Kapan SURVIVE (vending machine percepat), kapan STRETCH (vending machine supply, lo yang olah), kapan PROVE (vending machine mati total).

**"Joki mikir"** = lo nyerahin proses berpikir ke AI. Yang ini yang bahaya. Yang ini yang bikin lo gagal livecode, gagal interview, gagal di kerjaan. Vending Machine boleh bantu supply informasi. Tapi mikir? Itu kerjaan lo.

---

### Yang Baru di v11

- **`mkdir -p` dihapus dari tracker setup** — nggak ada parent directory yang perlu dibuat. `mkdir ~/belajar-tracker` aja cukup.
- **Tracker path sekarang fleksibel** — lo bisa taruh di mana aja (`~/Documents/`, folder bootcamp, dll), bukan harus di `~/belajar-tracker/`.

### Yang Baru dari v10

- **Metaphor refined:** "Dispenser Non-Deterministik" → "Vending Machine Non-Deterministik." Lebih tepat: lo request informasi (kayak masukin koin + pencet tombol), AI ngeluarin sesuatu — kadang sesuai, kadang nggak. Lo verifikasi.
- **Penjelasan Non-Deterministik:** "randomness" → "probabilitas" — lebih akurat untuk cara kerja LLM.
- **Fastify caveat:** Workflow E Step 5 sekarang ada peringatan: eksplorasi framework alternatif HANYA kalo lo udah nguasain kurikulum.

### Yang Baru dari v9

- **Tracker system direstruktur:** `belajar.md` flat → `~/belajar-tracker/` folder structure. Satu file per phase (`phase-0.md` s/d `phase-3.md`), diorganisir per GC milestone. Format baru: ✅ UDAH BISA / 🎯 LAGI BELAJAR / ❌ STUCK — scannable instruktur 30 detik untuk 1-on-1 yang presisi.
- **Semua referensi tahun dikoreksi:** 2025 → 2026. Kita di Juli 2026, bukan 2025.

### Yang Baru dari v8

- **Terminologi Hacktiv8 dikoreksi:** "lab session" → "sesi exercise", "lecture" → "instruktur jelasin/demo." Pitfall 4 sekarang: "Ngoding pas instruktur lagi jelasin atau demo."
- **Tracking headers diperjelas:** "JANGAN tracking" → "JANGAN tracking vanity metrics ini", "TRACKING ini" → "TRACKING ini (metrics that counts)."

### Yang Baru dari v7

- **Judul + tema diganti:** "AI Itu Vending Machine Informasi Non-Deterministik, Bukan Joki Mikir." Reframing fundamental: AI bukan guru, bukan expert — AI itu mesin probabilitas. Lo yang harus mikir.
- **Policy Hacktiv8 dikoreksi:** Phase 0-2 awal = no AI di tugas. Phase 2 Week 3+ = AI BOLEH di tugas, kecuali livecode. Modul sekarang phase-aware — warning-nya nggak absolut lagi.

### Yang Baru dari v6

- **⚠️ Policy Hacktiv8 v6** — framing awal "pisahin belajar dari nugas" + 2 skenario (Mandiri + Post-Tugas Review)
- **AI dikasih konteks modul** di Latihan 2, 3, 5 (Bagian 5)

### Yang Baru dari v5

- **Bootcamp-Aware Timeblock** — 2 skenario weekday + weekend golden hours + 4 pitfalls (Bagian 4)

### Yang Baru dari v4

- **3 Mode SURVIVE/STRETCH/PROVE** (Bagian 1)

### Yang Baru dari v2-v3

- Vibe Coding Hell, AI Sycophant Problem, Ebbinghaus Curve, Spaced Repetition, Async/Await modern, Kamus 37+ istilah, APPENDIX 11 template

---

### Kenapa Modul Ini Ada

Gue liat pola yang sama berulang-ulang:

```
dapet tugas → baca soal sekilas → copy ke AI → copy jawaban → upload → minggu depan nggak ingat apa-apa
```

Mereka pikir mereka "belajar pake AI". Padahal mereka cuma **outsource thinking** — nyerahin proses berpikir ke vending machine. Otak nggak dilatih. Pas livecode ketauan kosong. Pas interview teknis nge-blank.

Tahun 2026 ini ada fenomena baru: **Vibe Coding Hell.** Lo terjebak Cursor, Copilot, AI Agent Mode. Lo "bikin" banyak hal... tapi nggak ngerti apa-apa.

Ini bukan salah AI-nya. AI cuma vending machine — dia ngeluarin apa yang lo minta. Ini salah **lo nyerahin mikir ke vending machine.**

Modul ini bakal ngajarin lo:

1. **Kenapa** cara lo sekarang nggak works — dari tutorial hell sampe vibe coding hell
2. **Apa sih AI sebenernya** — vending machine non-deterministik, bukan guru, bukan expert
3. **Gimana** pake AI tanpa nyerahin proses mikir — 3 mode SURVIVE/STRETCH/PROVE
4. **5 Workflow konkret** buat belajar yang beneran nempel di otak
5. **Cara survive bootcamp** sesuai phase — kapan AI boleh, kapan nggak, dan gimana tetep belajar di kedua situasi
6. **Bangun kebiasaan belajar** dengan spaced repetition + bootcamp-aware timeblock

### Siapa yang Paling Butuh Modul Ini

- Lo yang ngerasa "gue nonton tutorial mulu tapi nggak bisa-bisa"
- Lo yang tiap hari pake Cursor/Copilot tapi nggak bisa jelasin kode lo sendiri
- Lo yang panik tiap minggu ngejar deadline tugas
- Lo yang nilai oke tapi nggak pede jelasin balik kode yang lo tulis
- Lo yang udah beberapa kali gagal livecode
- Lo yang udah masuk Phase 2+ dan sekarang AI legal... tapi lo makin nggak ngerti apa-apa
- Lo yang pengen berhenti jadi "prompt engineer" dan mulai jadi actual engineer

### Cara Baca

Modul ini disusun linear — baca dari awal ke akhir. Tapi tiap bagian bisa berdiri sendiri. Kalo lo cuma punya 5 menit: baca **Bagian 0** dulu, itu bakal nge-set mindset lo.

Kalo lo lagi desperate pengen survive tugas besok: langsung lompat ke **Bagian 3**.

Kalo lo udah baca semua dan butuh refrensi cepet: buka **[APPENDIX](APPENDIX.md)**.

Kalo lo nemu istilah asing waktu baca: buka **[Bagian 5: KAMUS ISTILAH](05-meta.md)**.

**PENTING:** Setelah lo selesai baca semua bagian, jangan langsung tutup. Buka **[Bagian 5: BACA ULANG](05-meta.md#part-2-baca-ulang-modul-ini--pake-teknik-dari-modul-ini)** dan kerjain 5 latihan di situ.

---

## Daftar Isi

| Bagian | Judul | Isi |
|---|---|---|
| [0](00-prolog.md) | Prolog: Kenapa Lo Ngerasa Belajar Tapi Nggak Ngerti | Illusion of learning, tutorial hell → vibe coding hell, passive vs active learning, Ebbinghaus intro |
| [1](01-mental-model.md) | AI Itu Vending Machine, Bukan Joki Mikir | **⚠️ Policy Hacktiv8 phase-aware.** Apa itu vending machine non-deterministik. 3 Mode (SURVIVE/STRETCH/PROVE). 2 skenario: Mandiri + Post-Tugas Review. Sycophant problem, anti-kritis. |
| [2](02-workflow-belajar.md) | 5 Workflow Belajar yang Beneran Works | Project-first, Feynman AI, Quiz Yourself, Compress & Structure, Tutorial Right Way |
| [3](03-bootcamp-survival.md) | Pola Khusus Bootcamp: Ngadepin Tugas Sesuai Phase | **⚠️ Phase 0-2 awal vs Phase 2 Week 3+:** kapan AI boleh & nggak. Cara baca soal, template prompt, pair programming, debugging. |
| [4](04-habit-loop.md) | Bangun Kebiasaan Belajar | **★ BOOTCAMP TIMEBLOCK** + **📁 ~/belajar-tracker/** manifest system (per phase, per GC). 4 pitfalls. Spaced repetition. Progress tracking (vanity vs real). Accountability. Transisi pasca-bootcamp. |
| [5](05-meta.md) | Kamus Istilah + Baca Ulang dengan Teknik Modul | **KAMUS:** 38+ istilah. **LATIHAN:** 5 meta-exercise — AI dikasih konteks modul biar feedback akurat. |
| [A](APPENDIX.md) | Appendix: Senjata Tambahan | 11 prompt template, curated resource links, tools rekomendasi |

---

### Rules Penting Module Ini

1. **Nggak ada kode.** Semua dalam bahasa natural.
2. **Contoh pakai async/await** — bukan `.then()` jadul.
3. **Lo disuruh mikir, bukan disuruh ngejalanin perintah.**
4. **Bisa dibaca ulang.** Simpen link modul ini. Pas lo stuck, balik lagi.

---

⬇️ Mulai dari sini: [00 - Prolog](00-prolog.md)
