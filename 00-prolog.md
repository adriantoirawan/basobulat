# Bagian 0: Prolog — Kenapa Lo Ngerasa Belajar Tapi Nggak Ngerti

## "Gue Udah Nonton 20 Jam Tutorial, Kok Masih Nggak Bisa?"

Pernah ngalamin ini?

- Nonton tutorial 2 jam tentang React. Besoknya nggak inget apa-apa.
- Ngerjain tugas dengan bantuan ChatGPT. Nilai 100. Tapi lo nggak bisa jelasin balik kodenya ngapain aja.
- Baca dokumentasi, nonton course, ikutin coding-along... tapi pas disuruh bikin sesuatu dari scratch, blank total.
- Pake Cursor atau Copilot tiap hari. Bisa "bikin" banyak project. Tapi lo nggak ngerti apa-apa di dalamnya.
- Temen lo keliatannya cepet banget paham, lo ngerasa ketinggalan terus.

Ini bukan berarti lo bego. Ini bukan berarti lo "nggak bakat ngoding."

Ini terjadi karena lo **nggak pernah beneran belajar.** Lo cuma **ngonsumi informasi** — atau lebih parah lagi, lo nyuruh AI ngonsumi dan nulis buat lo.

---

## Dari Tutorial Hell ke Vibe Coding Hell

Ada evolusi penderitaan di dunia belajar ngoding. Pahami ini:

### Era 2019-2023: Tutorial Hell

Dulu, musuh utama orang belajar ngoding adalah "tutorial hell." Ciri-cirinya:

- Lo berhasil ngikutin banyak tutorial, tapi nggak bisa bikin apa-apa sendiri
- Lo lebih banyak nonton video tentang ngoding daripada beneran ngoding
- Lo punya pengetahuan "flashcard-level" — tau istilah-istilah keren, tapi nggak ngerti apa yang terjadi di bawahnya
- Lo marathon 6 jam video, coding-along, ngerasa paham... terus freeze pas disuruh nulis dari scratch

Solusinya dulu simpel: tutup YouTube, buka VS Code, mulai ngetik sendiri.

### Era 2024-sekarang: Vibe Coding Hell

Sekarang musuhnya berevolusi. Lane Wagner dari Boot.dev nge-coin istilah ini. Cirinya:

- Lo nggak bisa ngoding tanpa Cursor atau Copilot
- Lo "bikin" tower defense game keren... tapi cuma jalan di `http://localhost:3000` dan lo nggak ngerti kenapa ada 6000+ baris kode
- Lo lebih sering chat sama AI agent daripada nulis kode sendiri
- Lo ngerasa productive karena "bikin banyak hal" — padahal AI yang bikin, lo cuma prompt
- Kode lo jalan... tapi lo nggak bisa jelasin gimana caranya

Dan ini **jauh lebih bahaya** dari tutorial hell.

Kenapa? Karena di tutorial hell, lo setidaknya SADAR lo nggak bisa apa-apa. Di vibe coding hell, lo ngerasa JAGO karena lo "bisa bikin banyak hal." Padahal lo cuma jago nge-prompt.

**Riset 2026** dari arXiv (2507.09089): developer yang pake AI merasa 20-25% lebih produktif. Tapi pengukuran objektif nunjukin mereka justru **19% lebih lambat.** AI bikin lo ngerasa produktif — tapi realitanya lo melambat.

---

## Illusion of Learning: Otak Lo Nipu Lo Sendiri

Ada fenomena di psikologi kognitif namanya **illusion of competence** atau **fluency illusion**.

Sederhananya: otak lo nggak bisa bedain antara *"gue familiar sama ini"* dan *"gue NGERTI ini."*

Pas lo nonton tutorial dan ngikutin coding-along...
- Semua keliatan masuk akal
- Lo ngerasa "oh iya gue paham kok"
- Lo ngangguk-ngangguk sepanjang video

Pas lo pake Cursor dan liat AI nulis kode buat lo...
- Kode keliatan bersih dan rapih
- Lo ngerasa "oh gue yang bikin ini"
- Lo commit, push, pamer ke temen

Tapi itu cuma **recognition**, bukan **recall**.

Recognition = lo liat sesuatu dan ngerasa "gue pernah liat ini." Kayak lo liat muka temen dan tau itu siapa.

Recall = lo bisa narik informasi dari otak lo tanpa ada trigger. Kayak lo bisa gambar ulang muka temen lo dari ingatan.

Belajar yang beneran = recall. Bukan recognition. Dan AI lo pake dengan cara yang **justru menghilangkan recall.**

---

## Kenapa Lo Lupa 70% dalam 24 Jam

Ini bukan opini. Ini sains.

Tahun 1885, Hermann Ebbinghaus nemuin **Forgetting Curve:**

```
Setelah 20 menit: lo lupa ~42% dari yang lo pelajari
Setelah 1 jam:    lo lupa ~56%
Setelah 1 hari:   lo lupa ~70%
Setelah 1 minggu: lo lupa ~77%
```

Itu kalo lo cuma **sekali terekspos informasi** tanpa review.

Dan tebak? Cara kebanyakan orang "belajar" dengan AI persis kayak gitu: baca jawaban AI sekali, ngerasa paham, terus lanjut. Nggak ada review. Nggak ada active recall. Dalam 24 jam, 70% ilang.

Ebbinghaus juga nemuin solusinya: **spaced repetition.** Kalo lo review informasi di interval yang makin lebar (1 hari, 3 hari, 7 hari, 14 hari, 30 hari), forgetting curve lo jadi makin landai. Informasi yang tadinya ilang 70% dalam sehari, bisa jadi cuma ilang 10%.

Modul ini bakal ngajarin lo gimana implementasi spaced repetition dengan AI — bukan dengan Anki atau flashcard app manual yang ribet.

---

## Pattern Copy-Paste: Kenapa Lo Gagal di Livecode

Ini pattern yang paling sering gue liat:

```
1. Dapet assignment
2. Baca soal dengan cepat — "oh, ini tentang REST API"
3. Copy-paste soal ke ChatGPT
4. Copy-paste jawaban dari ChatGPT
5. Jalanin, kalo error copy-paste error ke ChatGPT
6. ChatGPT kasih fix, copy-paste lagi
7. Works, upload, selesai
8. Datang ke livecode, nggak bisa ngapa-ngapain
9. Bingung: "kemarin gue bisa kok"
```

**Kenapa ini nggak works?**

Karena lo ngilangin satu-satunya bagian dari proses yang bikin lo belajar: **perjuangan lo sendiri.**

Belajar terjadi pas lo:
- Baca error message dan mikir "ini kenapa ya"
- Nyari di dokumentasi dan nggak nemu-nemu
- Coba solusi pertama, gagal
- Coba solusi kedua, gagal juga
- Coba solusi ketiga, berhasil
- Mikir "OH GITU CARANYA"

Itu "OH GITU" moment — itu yang bikin informasi nempel. Bukan copy-paste.

---

## Konsumsi vs Pemahaman

Bayangin dua orang:

**Orang A (Vibe Coder):**
- Prompt Cursor: "bikinin dashboard admin"
- AI generate 2000 baris, works, lo push
- Lo ngerasa "gila gue hebat banget bisa bikin ini"
- Tapi lo nggak bisa jelasin satu pun fungsi di kode itu

**Orang B (Active Learner):**
- Nulis sendiri dari scratch, 200 baris
- Debugging sendiri, stuck 2 jam di satu error
- Akhirnya beres — dan sekarang beneran paham setiap baris

Mana yang beneran belajar?

Orang A ngerasa lebih produktif — punya 10 project di GitHub. Tapi pas interview teknis? Hancur. Orang B cuma punya 1-2 project kecil, tapi dia bisa jelasin semua, bisa extend, bisa refactor.

---

## Active vs Passive Learning

| Passive Learning | Active Learning |
|---|---|
| Nonton tutorial | Bikin project sendiri |
| Baca dokumentasi linear | Search dokumentasi pas stuck |
| Prompt AI "bikinin" | Prompt AI "jelasin kenapa" |
| Coding-along ngikutin video | Tulis ulang dari scratch |
| Copy-paste kode AI | Pair programming — lo ngetik, AI navigasi |
| Scroll resource | Tutup resource, test diri sendiri |
| Agent mode / Cursor compose | Matiin autocomplete, nulis manual |

---

## Coba Sendiri: Audit Cara Belajar Lo

Sebelum lanjut, jujur:

1. Minggu lalu, berapa jam lo habisin buat **nonton tutorial / scroll resource / prompt AI "bikinin"**?
2. Minggu lalu, berapa jam lo habisin buat **ngetik kode sendiri tanpa autocomplete AI**?
3. Dari tugas terakhir, bisa nggak lo jelasin ulang setiap baris kode — kenapa ada di situ?
4. Kalo lo disuruh ngerjain tugas yang sama lagi besok... tanpa Cursor... lo bisa?
5. Jujur: berapa persen kode di project terakhir lo yang lo **ngerti** vs yang **AI generate dan lo terima aja**?

Kalo jawaban nomor 2 jauh lebih kecil dari nomor 1 — lo punya masalah.
Kalo jawaban nomor 3 "nggak" — lo di vibe coding hell.
Kalo jawaban nomor 5 < 70% — lo harus baca modul ini sampe abis.

---

## Yang Bakal Lo Dapet dari Modul Ini

- Paham kenapa cara belajar lo sekarang nggak efektif — dari perspektif psikologi kognitif
- Tau beda tutorial hell vs vibe coding hell — dan gimana escape dari dua-duanya
- Punya mental model baru: AI sebagai sparring partner, bukan joki
- Bisa pake 5 workflow konkret buat belajar apa aja
- Bisa survive tugas bootcamp tanpa outsourcing thinking
- Punya sistem spaced repetition yang bikin informasi nempel permanen

Syaratnya: **lo harus praktekin.** Modul ini bukan buat dibaca doang.

---

⬅️ Kembali ke [INDEX](INDEX.md) | Lanjut ke [Bagian 1: Ganti Mental Model](01-mental-model.md) ➡️
