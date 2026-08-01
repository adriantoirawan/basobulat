# Bagian 2: 5 Workflow Belajar yang Beneran Works

Gue urutin dari fundamental sampe advanced. **Mulai dari Workflow A dulu**, kuasai, baru lanjut.

---

## Workflow A: Project-First — Mulai Ngerjain, Bukan Nonton

> "The best way to learn is to build a real-world project and only search for information when you need it." — Dan Koe

### Cara Jalanin:

1. **Pilih satu mini-project.** Todo app, calculator, quote generator — sesuatu kecil dengan goal jelas.
2. **Jangan buka tutorial dulu.** Jangan YouTube. Jangan dokumentasi. Jangan AI.
3. **Tulis apa yang lo tau.** Mulai dari yang lo yakin.
4. **Pas lo BENERAN stuck, baru tanya.** Bukan minder duluan. Lo harus ngerasain "gap" dulu — ada yang lo pengen lakuin tapi nggak tau caranya.
5. **Search spesifik.** Bukan "gimana bikin REST API" — terlalu luas. Tapi: "di Express, kenapa `req.body` gue undefined padahal udah pake `express.json()`?"
6. **Iterate, jangan perfeksionis.** Project lo jelek? Nggak masalah. Yang penting jalan dan lo ngerti.

### Contoh Konkret: Lo Mau Belajar Express.js

```
SALAH:
  Nonton 5 video → coding-along → copy → nggak inget

BENER:
  Target: "Gue mau bikin API return data user"
  → Init project, install express
  → Nulis route GET /users sebisanya
  → Error "Cannot GET /" → tanya AI kenapa
  → Lanjut nulis → stuck lagi → tanya lagi → selesai
  Hasil: lo INGET karena lo NGALAMIN
```

---

## Workflow B: Feynman AI — Lo Jelasin, AI Koreksi

### Cara Jalanin:

1. **Tutup semua resource.**
2. **Prompt:**
   ```
   "Gue lagi belajar [KONSEP]. Lo jadi guru yang kritis:
   koreksi pemahaman gue, tunjukin yang miss, tanya balik.
   Gue mulai: [LO JELASIN KONSEPNYA]"
   ```
3. **Jelasin pake bahasa sehari-hari.** Analogi. Jangan jargon.
4. **AI respon.** Lo baca, lo cerna.
5. **Ulangi besok.** Topik sama. Liat improvement.

### Contoh:

```
LO:
  "Gue jelasin async/await ya. Ini kayak lo pesen makanan:
  lo bilang 'await pesanan' — lo nunggu makanan dateng,
  tapi sambil nunggu lo masih bisa ngelakuin hal lain
  (kode synchronous di luar fungsi async tetap jalan).
  Kalo berhasil, lanjut. Kalo error, pake try/catch buat nangkap.
  Bener nggak? Ada yang miss?"

AI:
  "Cukup bagus tapi ada yang perlu dilurusin:
  1. 'Sambil nunggu lo bisa ngelakuin hal lain' — ini kurang
     tepat. Di DALAM fungsi async, kode SETELAH await memang
     nunggu. Yang tetep jalan itu kode di LUAR fungsi async.
  2. Lo belum mention bahwa async function SELALU return Promise,
     meskipun lo nggak explicit.
  3. Gimana kalo lo perlu ngejalanin beberapa async task paralel
     (Promise.all)? Kenapa itu penting?

  Sekarang coba jelasin nomor 1 lebih detail."
```

---

## Workflow C: Quiz Yourself — Paksa Otak Recall

**Retrieval practice** (Dunlosky et al., 2013): practice testing = satu-satunya teknik "high utility" bareng spaced repetition.

### Cara Jalanin:

1. **Kasih resource ke AI.** Dokumentasi, artikel, catetan lo.
2. **Suruh AI bikinin soal bertingkat:**
   ```
   "Gue abis belajar [TOPIK]. Bikinin 10 soal:
   3 gampang (definisi), 4 medium (penerapan),
   3 susah (edge cases). JANGAN kasih jawaban dulu."
   ```
3. **Lo jawab satu-satu.** Jangan ngintip. Paksa otak recall.
4. **AI koreksi + jelasin kenapa bener/salah.**
5. **Catet yang lo salah.** Balik besok.

### Bonus: Auto-generate Quiz dari Catetan

Kalo lo males bikin soal, upload catetan/dokumentasi ke tools kayak Wisdolia atau NotebookLM. Auto generate flashcard + quiz. Tapi inget: setelah AI generate soal, LO yang harus jawab. Jangan AI generate soal terus AI juga yang jawab.

---

## Workflow D: Compress & Structure — Chaos ke Clarity

Ini buat situasi lo bener-bener nol di topik baru.

### Cara Jalanin:

1. **Kumpulin 5-10 resources** (Perplexity bagus buat ini).
2. **Compress pake AI:**
   ```
   "Rangkumin resource ini:
   - Konsep inti (3-5 poin)
   - Analogi sederhana
   - Learning path dasar → advanced
   - Common pitfalls pemula
   - 10 hal paling penting buat diingat"
   ```
3. **Tulis ulang pake bahasa lo.** Jangan cuma baca.
4. **Lanjut ke Workflow A.** Compress cuma orientasi awal.

---

## Workflow E: Tutorial Right Way — Kalo Terpaksa Pake Tutorial

Kadang tutorial memang jalan terbaik buat topik tertentu. Tapi ada cara pakenya biar nggak terjebak.

Diadaptasi dari freeCodeCamp + pengalaman:

### 5 Step Belajar dari Tutorial Tanpa Masuk Hell:

**Step 1: Think first.** Sebelum play, pikirkan project-nya. Lo mau bikin apa? Gimana kira-kira flow-nya? Ini bikin otak lo punya frame of reference.

**Step 2: Try first.** Coba bikin sendiri 15-30 menit. Lo bakal gagal, dan itu bagus. Kegagalan ini bikin lo "lapar" — pas lo nonton tutorial, otak lo jauh lebih reseptif.

**Step 3: Pause & process.** Jangan marathon 2 jam. Pause tiap 15 menit. Tanya diri sendiri: "Gue ngerti nggak kenapa instruktur ngelakuin ini?" Catet pertanyaan lo.

**Step 4: Break things.** Setelah selesai, sengaja rusakin kode. Ganti variabel, ganti logic. Baca error message-nya. Ini ngajarin lo debugging.

**Step 5: Rebuild your way.** Bangun ulang project yang sama — dengan twist. Kalo instruktur pake `if/else`, lo pake `switch`. Kalo instruktur pake Express, lo coba Fastify (JIKA DAN HANYA JIKA lo udah nguasain Express dan mau explore aja. Kewajiban lo ngerti kurikulum dulu, baru eksplorasi). Tambahin fitur kecil. Ini transisi dari "ngikutin" ke "bikin sendiri."

---

## Cara Milih Workflow

| Situasi | Workflow |
|---|---|
| Skill baru yang bisa dipraktekin | **A: Project-First** |
| Udah "belajar" tapi nggak yakin ngerti | **B: Feynman AI** |
| Persiapan ujian/livecode | **C: Quiz Yourself** |
| Nol di topik baru, butuh peta | **D: Compress & Structure** |
| Pengen belajar dari tutorial tanpa terjebak | **E: Tutorial Right Way** |

Idealnya siklus penuh:
```
D (orientasi) → A (praktek) → B (cek pemahaman) → C (tes) → ulangi
```

---

## Coba Sendiri

Pilih satu:
- Ada tugas → Workflow A. 15 menit ngerjain sendiri dulu.
- Abis nonton tutorial → Workflow B. Tutup, jelasin ulang ke AI.
- Ada livecode besok → Workflow C. AI bikinin soal, lo jawab.

30 menit aja. Sekarang.

---

⬅️ Kembali ke [Bagian 1: Ganti Mental Model](01-mental-model.md) | Lanjut ke [Bagian 3: Bootcamp Survival](03-bootcamp-survival.md) ➡️
