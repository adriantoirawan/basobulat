# Bagian 5: Kamus Istilah + Baca Ulang Modul dengan Teknik Sendiri

## Kenapa Halaman Ini Ada

Lo baru aja baca 4 bagian penuh istilah asing:

*"Illusion of competence... spaced repetition... sycophant problem... vibe coding hell... Ebbinghaus curve... desirable difficulty..."*

Kalo lo baru masuk bootcamp, beberapa istilah di atas mungkin bikin lo mikir: "ini apaan sih?" Dan itu wajar. Modul ini ngomongin banyak konsep dari psikologi kognitif, learning science, dan software engineering — tiga dunia yang mungkin belom lo kenal.

Halaman ini punya dua fungsi:

1. **Kamus istilah** — lo bisa balik ke sini kapan aja pas nemu kata yang nggak ngerti
2. **Baca ulang modul ini pake teknik yang diajarin di modul ini sendiri** — ini bagian paling penting. Lo bakal praktekin Workflow B, C, D, dan spaced repetition... ke modul ini.

Kenapa? Karena kalo lo cuma baca modul ini sekali dan nggak pernah balik lagi, lo bakal lupa 70% dalam 24 jam. Ingat Ebbinghaus. Dan ironisnya: lo baca modul tentang cara belajar, tapi lo nggak pake teknik belajar yang diajarin buat belajar modulnya sendiri.

**Jangan jadi orang kayak gitu.**

---

## Part 1: KAMUS ISTILAH

### 🧠 Konsep Belajar & Psikologi Kognitif

| Istilah | Artinya (Bahasa Lo) |
|---|---|
| **Illusion of Competence** | Otak lo ngerasa "udah ngerti" padahal cuma familiar. Kayak lo nonton video orang main gitar, ngerasa "gue bisa nih", padaha pas pegang gitar nggak bisa apa-apa. |
| **Fluency Illusion** | Nama lain dari illusion of competence. Lo "lancar" ngikutin penjelasan orang, tapi nggak bisa jelasin sendiri. |
| **Recognition** | Lo NGELIAT sesuatu dan ngerasa "gue pernah liat ini." Kayak lo ngeliat muka temen: tau itu siapa, tapi nggak bisa gambar ulang mukanya dari ingatan. |
| **Recall** | Lo NARIK informasi dari otak tanpa ada trigger. Kayak lo bisa gambar ulang muka temen tanpa liat foto. Recall = belajar beneran. |
| **Active Recall / Retrieval Practice** | Teknik belajar di mana lo PAKSA otak narik informasi tanpa ngeliat sumber. Contoh: quiz diri sendiri, flashcards, Feynman technique. Riset bilang ini teknik paling efektif (high utility). |
| **Spaced Repetition / Distributed Practice** | Review informasi di interval yang makin lebar (1 hari, 3 hari, 7 hari, 14 hari, 30 hari). Lawannya: cramming (belajar kebut semalam). Riset bilang ini juga high utility. |
| **Ebbinghaus Forgetting Curve** | Grafik yang nunjukin seberapa cepat manusia LUPA. Tanpa review: 70% ilang dalam 24 jam. Hermann Ebbinghaus nemuin ini tahun 1885. |
| **Desirable Difficulty** | Kesulitan yang BAGUS buat belajar — lo berjuang dikit, dan perjuangan itu justru bikin informasi nempel. Lawannya: undesirable difficulty — kesulitan yang cuma buang-buang waktu. |
| **Feynman Technique** | Teknik dari Richard Feynman (fisikawan): jelasin konsep pake bahasa sederhana seakan-akan ke anak kecil. Kalo lo nggak bisa, lo belom ngerti. |
| **Socratic Method** | Metode ngajar pake tanya-jawab. Guru nggak ngasih jawaban, cuma nanya terus sampe lo nemu sendiri. |
| **Zeigarnik Effect** | Otak lo lebih inget tugas yang BELUM SELESAI daripada yang udah selesai. Ini kenapa "mulai aja dulu" lebih gampang daripada "selesaiin semuanya." |
| **Metacognition** | "Mikir tentang mikir." Kemampuan lo buat sadar: "gue ngerti apa? gue nggak ngerti apa?" Makin bagus metacognition lo, makin efektif lo belajar. |

### 🤖 Istilah AI & Tools

| Istilah | Artinya (Bahasa Lo) |
|---|---|
| **Tutorial Hell** | Jebakan di mana lo cuma bisa ngoding kalo ngikutin tutorial. Begitu sendiri, blank. Umum di era 2019-2023. |
| **Vibe Coding Hell** | Evolusi tutorial hell di era AI. Lo "bisa" bikin banyak hal karena Cursor/Copilot/ChatGPT yang nulis kode — tapi lo nggak ngerti apa-apa di dalamnya. Lebih bahaya karena lo NGERASA jago. |
| **SURVIVE Mode** | Satu dari 3 mode dalam 1 Tugas (Bagian 1). Komponen yang lo UDAH BISA: setup, boilerplate, routing dasar. AI generate → lo review paham. Time budget: ~20%. |
| **STRETCH Mode** | Mode paling penting. 1-2 konsep BARU yang jadi target belajar lo di tugas ini. LO yang ngetik kode, AI cuma navigasi + jelasin + koreksi. Nggak boleh AI generate kode utuh. Time budget: ~60%. |
| **PROVE Mode** | Mode validasi. Lo kerjain komponen SENDIRI dari scratch — tanpa AI sama sekali. Baru setelah selesai, AI review. Kalo nge-blank, jujur: itu bukan SURVIVE, pindahin ke STRETCH. Time budget: ~20%. |
| **Learning Target** | Template wajib tulis sebelum mulai tugas (Bagian 1): 🎯 STRETCH (target belajar), ⚡ SURVIVE (udah bisa), ✅ PROVE (mau buktiin). Bikin lo jujur sama gap pengetahuan sendiri. |
| **Golden Hours** | Slot Sabtu pagi (09:00-12:00) — waktu paling berharga buat STRETCH + PROVE. Energi penuh, pikiran fresh, nggak ada interupsi bootcamp. 3 jam golden = setara 6 jam weekday malam exhausted. JANGAN dipake buat boilerplate. |
| **Bootcamp-Weekday** | Dua skenario weekday di Bagian 4: selesai jam 4 sore (ada slot Deep Study 45 menit + SURVIVE 90 menit) vs stretch sampai jam 6 sore (cuma bisa 1 sesi deep: SURVIVE ATAU Deep Study). Istirahat 90 menit non-negotiable di kedua skenario. |
| **Learning Manifest** | Sistem tracking di Bagian 4: folder `~/belajar-tracker/` dengan file per phase. Format: ✅ UDAH BISA / 🎯 LAGI BELAJAR / ❌ STUCK — diorganisir per GC milestone. Bisa lo tunjukin ke instruktur pas 1-on-1 biar mereka scan 30 detik dan langsung tau gap lo. |
| **Repo Latihan vs Repo Tugas** | Aturan di Bagian 1: Phase 0-2 awal = repo tugas no AI, latihan di `~/latihan/`. Phase 2 Week 3+ = AI boleh di tugas (kecuali livecode), tapi HARUS 3-mode — jangan joki mikir. Post-Tugas Review: copy ke `~/review/` buat belajar dari gap. |
| **Post-Tugas Review** | Skenario B di Bagian 1: lo udah ngumpulin tugas, abis itu copy repo ke `~/review/`, lalu pake 3-mode buat belajar dari tugas itu — terutama bagian yang lo stuck pas nugas (baik pas no-AI phase awal maupun pas AI-allowed phase lanjut). Belajar dari gap sendiri. |
| **Sycophant Problem** | AI selalu setuju sama lo. Efek dari sifat non-deterministik: AI di-train buat helpful dan pleasing, jadi dia ngikutin arah prompt lo. Lo nanya "benar kan X?" AI jawab "benar!" Lo nanya "tapi kan Y?" AI jawab "benar juga!" Bahaya buat belajar. |
| **Non-Deterministik** | Sifat fundamental AI: outputnya nggak konsisten. Prompt yang sama bisa ngasih jawaban berbeda tiap kali. Kenapa? Karena AI nggak punya "jawaban bener" — dia cuma nebak token berikutnya secara probabilistik. Ini kenapa lo HARUS verifikasi. AI bukan database, bukan kalkulator, bukan guru. Dia vending machine. |
| **AI Hallucination / Halusinasi** | AI ngarang jawaban yang keliatannya meyakinkan tapi salah. Efek langsung dari sifat non-deterministik + probabilistic. Misal: AI nyebutin fungsi `express.parseJSON()` — padahal itu nggak ada. Selalu verifikasi ke dokumentasi resmi. |
| **Prompt Engineering** | Skill nulis instruksi ke AI yang efektif. Bukan cuma "bikinin X", tapi gimana cara nanya yang bikin AI ngasih jawaban yang lo butuhin. |
| **Sparring Partner** | Metafora: AI bukan joki yang ngerjain semuanya, tapi partner latihan yang ngelawan balik, ngasih feedback, dan bikin lo tambah jago. |
| **Agent Mode** | Fitur AI di mana AI nggak cuma jawab pertanyaan, tapi bisa ngejalanin aksi: bikin file, run command, debug sendiri, iterasi. Bahaya buat pemula karena lo skip proses berpikir. |
| **AI Autocomplete** | Fitur "tab to complete" di Cursor/GitHub Copilot — AI nyaranin baris berikutnya. Matiin pas jam belajar karena lo nggak mikir, lo cuma nerima saran. |
| **NotebookLM** | Tools gratis dari Google. Lo upload dokumen/artikel/video, AI bikin knowledge base, rangkuman, quiz, bahkan audio summary. |
| **Perplexity AI** | Search engine pake AI yang ngasih jawaban + sumber. Lebih cepet dari Google buat research. |
| **Cursor / Copilot** | AI coding assistant yang terintegrasi di code editor. Berguna buat engineer, berbahaya buat pelajar kalo dipake tanpa kontrol. |

### 💻 Istilah Teknis (yang Mungkin Muncul di Modul)

| Istilah | Artinya (Bahasa Lo) |
|---|---|
| **async/await** | Cara modern nulis kode asynchronous di JavaScript. Lo "nunggu" sesuatu selesai (await) tanpa nge-block semua kode lain. Gantinya `.then()` jadul. |
| **Promise** | Object di JavaScript yang ngewakilin "janji" — nilai yang belum ada sekarang tapi bakal ada nanti (berhasil atau gagal). |
| **try/catch** | Cara nangkap error di JavaScript. "Coba jalankan ini (try), kalo gagal tangkap errornya (catch)." |
| **API (Application Programming Interface)** | Cara dua aplikasi ngomong satu sama lain. REST API: API yang pake HTTP (GET, POST, PUT, DELETE). |
| **Endpoint / Route** | URL spesifik di API. Misal: `GET /users` artinya "ambil semua user." |
| **Middleware** | Fungsi yang jalan SEBELUM request nyampe ke route handler. Contoh: cek login dulu (auth middleware) sebelum kasih akses ke data. |
| **JWT (JSON Web Token)** | Cara authentication: server kasih "token" ke user setelah login, user kirim token itu di setiap request berikutnya buat buktiin identitasnya. |
| **ORM (Object-Relational Mapping)** | Tools yang bikin lo bisa ngakses database pake kode JavaScript (bukan SQL mentah). Sequelize, Prisma, TypeORM — contoh ORM. |
| **Stack Trace** | Daftar lengkap error yang nunjukin jejak: error mulai dari file mana, fungsi apa, baris ke berapa. Lo harus BACA ini. |
| **Root Cause** | Penyebab ASLI dari bug — bukan gejalanya. "App crash" itu gejala. "Variable user undefined karena query database return null" itu root cause. |
| **Refactor** | Nulis ulang kode biar lebih rapi, lebih cepet, lebih gampang dibaca — tanpa ngubah fungsinya. |
| **Edge Case** | Situasi ekstrim yang jarang terjadi. Misal: user input angka negatif di form umur, atau upload file 2GB. Kode lo harus handle ini. |
| **Boilerplate** | Kode standar yang selalu sama di setiap project. Ngebosenin tapi perlu. |
| **Dependency** | Library atau package yang project lo butuhin buat jalan. Di Node.js, ini yang ada di `package.json`. |

---

## Part 2: BACA ULANG MODUL INI — PAKE TEKNIK DARI MODUL INI

Ini bagian paling penting. Lo udah baca 4 bagian + kamus. Sekarang lo bakal baca ulang — tapi dengan teknik yang lo pelajari.

### Kenapa Ini Penting

Lo baru aja ngonsumi ~40K karakter tentang cara belajar. Tanpa active processing, 70% bakal ilang besok. Dan itu ironi tingkat dewa: lo baca modul tentang cara belajar efektif, tapi lo sendiri nggak belajar secara efektif.

Jadi sekarang lo bakal praktekin semua workflow ke modul ini sendiri. Ini **meta-learning**: pake teknik modul buat belajar modul.

---

### Latihan 1: Compress & Structure (Workflow D)

Baca ulang INDEX.md. Kali ini jangan cuma scan. Lo bakal bikin **satu halaman rangkuman** pake bahasa lo sendiri.

**Instruksi:**

1. Buka notepad atau file kosong. Judulin: "RANGKUMAN: AI Itu Vending Machine Informasi Non-Deterministik, Bukan Joki Mikir"
2. Untuk setiap bagian (0-4), tulis:
   - **Ide utama:** Satu kalimat. Apa inti bagian ini?
   - **Konsep kunci:** 3-5 poin penting yang lo inget (tutup modulnya dulu, coba recall)
   - **Yang gue bisa pake besok:** Satu hal konkret yang langsung lo terapin
3. Baru setelah lo tulis, lo boleh buka modul lagi buat ngecek: ada yang kelewat?
4. Kalo ada yang kelewat, catet — itu gap pemahaman lo.

**Target waktu:** 20 menit.

---

### Latihan 2: Feynman AI (Workflow B) — Jelasin Isi Modul ke AI

Sekarang lo bakal jelasin isi modul ini ke AI sebagai "guru killer."

**Instruksi:**

1. Buka ChatGPT/Claude.
2. **Paste isi modul ke AI dulu sebagai referensi.** Lo bisa copy-paste dari file-file di folder modul ini, atau kasih AI akses. Prompt:
```
"Ini isi modul 'AI Itu Vending Machine Informasi Non-Deterministik, Bukan Joki Mikir' tentang cara
belajar dengan AI. Lo baca dulu ya. Jangan respon apa-apa,
cukup bilang 'oke udah baca' kalo udah selesai.

[PASTE ISI MODUL — bisa bertahap kalo kepanjangan:
 mulai dari INDEX.md, 00-prolog.md, 01-mental-model.md,
 02-workflow-belajar.md, 03-bootcamp-survival.md,
 04-habit-loop.md. Bagian 5 (05-meta.md) nggak usah.]"
```

3. Setelah AI konfirmasi "oke udah baca," tutup modul lo. Tutup semua tab.
4. Pake prompt ini:

```
"Gue bakal jelasin isi modul 'AI Itu Vending Machine Informasi Non-Deterministik, Bukan Joki Mikir'
pake bahasa gue sendiri. Lo udah baca modulnya tadi.

Lo jadi guru killer yang brutal. Bandingin penjelasan gue
dengan isi modul yang lo baca. Koreksi kalo pemahaman gue
dangkal atau salah. Jangan basa-basi.

Modul ini isinya 5 bagian:

Bagian 0: [LO JELASIN INTINYA — jangan liat modul]
Bagian 1: [LO JELASIN INTINYA]
Bagian 2: [LO JELASIN INTINYA + SEBUTIN 5 WORKFLOW]
Bagian 3: [LO JELASIN INTINYA]
Bagian 4: [LO JELASIN INTINYA]

Setelah gue jelasin semua, lo kasih feedback:
- Mana yang pemahaman gue udah solid?
- Mana yang masih dangkal / ada gap?
- Konsep apa yang gue skip atau salah?"
```

5. Jelasin dari ingatan. Jangan ngintip.
6. Baca feedback AI. Karena AI punya konteks modulnya, feedback-nya bakal AKURAT — dia bisa bandingin penjelasan lo dengan isi asli modul.
7. Catet bagian yang lo skip atau salah. Balik ke bagian itu di modul, baca ulang.

**Target waktu:** 20 menit (5 menit setup paste modul, 15 menit jelasin + feedback).

---

### Latihan 3: Quiz Yourself (Workflow C) — Tes Pemahaman Modul

Sekarang lo bakal dites — tentang isi modul ini sendiri.

**Instruksi:**

1. **Paste isi modul ke AI dulu sebagai referensi.** Sama kayak Latihan 2 — AI harus tau isi modulnya biar soal yang dia bikin AKURAT dan SPESIFIK.

2. Prompt AI:

```
"Ini modul 'AI Itu Vending Machine Informasi Non-Deterministik, Bukan Joki Mikir' yang udah lo baca:

[LO BISA SKIP PASTE KALO LANGSUNG LANJUT CHAT YANG SAMA
 DARI LATIHAN 2 — AI udah punya konteks]

Bikinin 15 soal tentang isi modul ini. Mencakup:

5 soal gampang:
  - Definisi: apa itu tutorial hell? vibe coding hell?
    illusion of competence? active recall? spaced repetition?

5 soal medium:
  - Scenario: 'Budi ikutin semua tutorial tapi nggak bisa
    ngoding sendiri.' Debug: apa yang salah dan workflow
    mana yang harus Budi terapin?
  - Bedain: recognition vs recall, tutorial hell vs vibe coding hell
  - Aplikasi: gimana cara maksa AI biar nggak sycophant?

5 soal susah:
  - Edge case: 'Dina udah terapin spaced repetition tapi
    masih lupa. Debug: apa yang mungkin salah?'
  - Tradeoff: kapan SURVIVE, kapan STRETCH, kapan PROVE?
  - META: jelasin kenapa Post-Tugas Review (Bagian 1,
    Skenario B) lebih aman daripada pake AI pas nugas.

PASTIKAN soal lo spesifik ke isi modul, bukan generic.
JANGAN kasih jawaban dulu."
```

3. Lo jawab semua soal. Tulis jawaban lo.
4. Baru setelah selesai semua, suruh AI koreksi + jelasin.
5. Catet soal yang lo salah. Itu yang harus lo pelajari ulang.

**Target waktu:** 20-30 menit.

---

### Latihan 4: Setup Spaced Repetition buat Modul Ini

Lo udah tau Ebbinghaus curve. Jangan biarin 70% ilang dalam 24 jam.

**Instruksi:**

1. Prompt AI:

```
"Lo jadi spaced repetition scheduler gue.
Gue baru baca modul 'AI Itu Vending Machine Informasi Non-Deterministik, Bukan Joki Mikir' tentang
cara belajar dengan AI. Ini isinya secara garis besar:

[LO TULIS RANGKUMAN DARI LATIHAN 1 DI SINI]

Bikinin jadwal review 30 hari:

Hari 1 (besok): kasih 5 pertanyaan recall tentang
  konsep utama modul ini. Jangan kasih jawaban.
  
Hari 3: bikinin 10 soal yang menguji pemahaman gue.
  Kombinasi definisi, scenario, dan 'kenapa'.
  
Hari 7: suruh gue jelasin ulang SELURUH isi modul
  ke lo sebagai guru killer. Tantang gue di bagian
  yang gue skip / kurang dalam.
  
Hari 14: kasih gue 3 case study baru — situasi
  belajar yang BELUM disebut di modul — dan tanya
  workflow mana yang cocok + kenapa.
  
Hari 30: suruh gue bikin 'versi pendek' modul ini
  buat ngajarin temen gue. Maks 1 halaman.
  Review hasilnya dan kasih feedback."
```

2. Simpen jadwal ini. Copy ke calendar atau reminder app.
3. BENERAN jalanin tiap review sesuai jadwal. Jangan skip.

---

### Latihan 5: Ajarin Temen Lo (The Ultimate Test)

Feynman: kalo lo nggak bisa jelasin ke orang lain, lo belom ngerti.

**Instruksi:**

1. Cari satu temen bootcamp yang belom baca modul ini.
2. Jelasin ke dia dalam 10 menit: inti dari modul ini apa, kenapa penting, gimana cara terapinnya.
3. Pake analogi. Pake bahasa sehari-hari. Jangan pake jargon.
4. Suruh dia nanya balik. Kalo lo nggak bisa jawab pertanyaannya — itu gap lo.
5. Catet pertanyaan yang lo nggak bisa jawab. Balik ke modul. Pelajari lagi.

**Kalo nggak ada temen:** Pake AI. Dua tahap:

**Tahap 1 — Tes Kejelasan (AI nggak dikasih modul):**
```
"Lo jadi temen gue yang belom pernah baca modul ini.
Gue bakal jelasin 'AI Itu Vending Machine Informasi Non-Deterministik, Bukan Joki Mikir' ke lo
dalam 10 menit. Lo tanya balik kalo ada yang nggak
masuk akal, dan lo challenge kalo penjelasan gue
nggak jelas atau terlalu jargon-y.

Gue mulai: [LO JELASIN]"
```
→ Ini tes apakah penjelasan lo accessible. Kalo "temen" lo bingung,
  penjelasan lo kurang jelas.

**Tahap 2 — Tes Akurasi (AI dikasih modul):**
Setelah Tahap 1, kasih modul ke AI:
```
"Sekarang lo baca modul aslinya: [PASTE MODUL].
Bandingin sama penjelasan gue tadi. Mana yang gue
jelasin kurang akurat? Mana yang gue skip? Mana yang
penjelasan gue malah misleading?"
```
→ Ini tes apakah penjelasan lo AKURAT. AI bisa bandingin
  karena sekarang dia punya reference.

---

## Kenapa Ini Semua Penting

Lo mungkin mikir: "ini berlebihan, masa baca modul doang harus review 5x?"

Ingat apa yang lo pelajari di Bagian 0:

> Kalo lo cuma baca modul ini sekali dan lanjut hidup... besok lo udah lupa 70%.

Dan ironisnya: lo baca modul tentang gimana caranya belajar yang bener... tapi lo nggak terapin tekniknya ke proses baca modul ini sendiri. Itu kayak lo beli buku diet terus lo baca sambil makan pizza — bukunya bener, tapi lo nggak ngelakuin apa yang ditulis.

**Lo harus praktekin ini. ke modul ini sendiri. Sekarang.**

---

## Ceklis Final — Centang Semua Sebelum Lo Tutup Modul

- [ ] **Latihan 1**: Udah bikin rangkuman 1 halaman dari ingatan
- [ ] **Latihan 2**: Udah jelasin isi modul ke AI guru killer
- [ ] **Latihan 3**: Udah jawab 15 soal quiz dan catat yang salah
- [ ] **Latihan 4**: Udah setup spaced repetition schedule 30 hari
- [ ] **Latihan 5**: Udah jelasin ke temen (atau AI)
- [ ] **Kamus**: Udah bookmark halaman ini buat referensi cepet

**Kalo ada yang belum dicentang: lo belom selesai.** Balik dan kerjain.

---

⬅️ Kembali ke [Bagian 4: Bangun Kebiasaan Belajar](04-habit-loop.md) | Ke [APPENDIX](APPENDIX.md) ➡️ | Kembali ke [INDEX](INDEX.md)
