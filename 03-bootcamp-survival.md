# Bagian 3: Pola Khusus Bootcamp — Ngadepin Tugas Sesuai Phase

## ⚠️ REALITAS: Aturan AI Tergantung Phase Lo

```
Phase 0, Phase 1, Phase 2 (minggu 1-2):
  ❌ Nggak boleh pake AI di tugas. Sama sekali.

Phase 2 (minggu 3+) dan Phase 3:
  ✅ AI BOLEH di tugas — kecuali livecode.
  ❌ Livecode: nggak boleh AI. Selalu.
```

**Cara aman di semua phase:**

```
✅ BOLEH DI SEMUA PHASE:
  - AI buat BELAJAR MANDIRI di folder ~/latihan/
  - Abis ngumpulin tugas → copy ke ~/review/ → AI sparring partner
  - AI di chat browser buat nanya "jelasin konsep X", bukan "bikinin"

✅ BOLEH MULAI PHASE 2 WEEK 3+:
  - AI buat bantu ngerjain tugas — tapi lo HARUS pake 3-mode
    (SURVIVE/STRETCH/PROVE dari Bagian 1)
  - AI buat debugging, refactor, review

❌ JANGAN DI SEMUA PHASE:
  - AI pas livecode
  - Joki mikir: AI generate kode → lo copy-paste → lo nggak ngerti
  - Commit kode auto-generated ke GitHub (ada jejaknya)
```

**Kenapa bagian ini tetap penting:** Template prompting di bawah ini berguna buat semua phase — buat memahami soal, buat review tugas, dan buat pastiin lo nggak joki mikir di phase di mana AI legal.

---

## Real Talk: Lo Diburu Deadline

Gue ngerti. Bootcamp itu cepet. Tugas numpuk. Deadline besok. Lo panik.

Tapi ingat: **lo nggak bisa pake AI. Dan itu bagus.** Karena kalo lo bisa pake AI, lo bakal survive minggu ini... tapi gagal di livecode, gagal di interview, gagal di kerjaan.

Tugas bootcamp tanpa AI = simulasi kerja beneran. Di kerjaan lo nggak selalu bisa copy-paste ke ChatGPT (ada policy perusahaan, ada kode proprietary, ada konteks yang AI nggak ngerti).

**Kerjain tugas SEBISA LO.** Kalo stuck, catet. Itu gap lo. Nanti lo belajar dari gap itu — pake teknik di modul ini, di folder terpisah.

---

## Langkah 0: Baca Soal dengan Benar

60% masalah bootcamp student: mereka nggak baca soal.

Mereka scan, liat keyword ("REST API", "auth", "database"), langsung copy ke AI.

Luangin 10-15 menit:

1. **Baca soal 2x.** Scan, lalu detail.
2. **Tulis ulang requirements pake bahasa lo.** Ini maksa lo MEMPROSES.
3. **Identifikasi: mana yang lo udah tau?**
   ```
   GET /users → gue TAU
   Validasi input → gue PERNAH liat
   Association many-to-many → gue BELUM PERNAH
   ```
4. **Breakdown jadi steps kecil:**
   ```
   1. Init project + install deps
   2. Setup Express server
   3. Bikin model User
   4. Route GET /users
   5. Route GET /users/:id
   6. ...dst
   ```

Ini bukan buang waktu. Ini bikin lo lebih cepet karena lo tau persis apa yang lo kerjain.

---

## Prompting untuk Tugas: 3 Template

### Template A: Nggak Ngerti Requirement
```
"Gue lagi ngerjain tugas bootcamp. Ini soalnya:

[PASTE SOAL]

Gue nggak minta kode. Tolong:
1. Jelasin ulang requirement dalam bahasa gampang
2. Breakdown jadi 5-7 step kecil
3. Tandain step yang tricky buat pemula
4. Kasih tau: step mana yang harus gue pelajari lebih dalem dulu"
```

### Template B: Stuck di Satu Step
```
"Gue lagi ngerjain [KONTEKS]. Udah sampe step [X], stuck di [Y].

Yang gue udah coba:
- [A]
- [B]
- [C]

Error: [PASTE ERROR FULL]
Gue curiga masalahnya di [TEBAKAN].

JANGAN kasih kode full. Tolong:
1. Jelasin konsep yang perlu gue ngerti
2. Kasih hint: first step yang harus gue coba
3. Kalo masih stuck, baru kasih kode MINIMAL (cuma bagian relevan)"
```

### Template C: Selesai Tapi Nggak Yakin Paham
```
"Gue selesai ngerjain [TUGAS]. Gue mau mastiin ngerti.

Ini struktur kode gue (bukan full kode):
[LO JELASIN STRUKTUR]

Tolong:
1. Tanya 5 pertanyaan yang ngetes pemahaman gue
2. Gue jawab, lo kasih feedback
3. Kalo salah, kasih hint dulu — jangan jawaban langsung"
```

---

## Pair Programming dengan AI — Lo Ngetik, AI Navigasi

Lo yang ngetik kode. AI yang navigasi. Bukan sebaliknya.

### Prompt Starter:

```
"Kita pair-programming buat [FEATURE].
Aturan:
- GUE yang ngetik kode, lo cuma navigasi + tanya
- Kalo gue stuck, lo kasih HINT, bukan solusi
- Kalo gue udah coba 3x masih gagal, baru kasih kode minimal
- Setiap step, tanya: 'ngerti kenapa kita pake ini?'

Mulai: gue mau bikin [FEATURE], step pertama apa?"
```

### Contoh Interaksi:

```
AI:   "Step 1: Setup route handler buat POST /users.
       Lo tau nggak gimana cara extract body dari request?"
LO:   "Pake req.body?"
AI:   "Betul. Tapi lo udah setup middleware-nya belum?"
LO:   "...belum. Oh iya, express.json()!"
AI:   "Yes. Kenapa itu perlu?"
LO:   "Karena Express default-nya nggak parse JSON body..."
AI:   "Bagus. Sekarang tulis kodenya, gue liatin."
```

Bukan "AI generate 200 baris, lo ngangguk."

---

## Debugging dengan AI — Lo Usaha Dulu

```
STEP 1: BACA ERROR MESSAGE SAMPAI HABIS.
  "Cannot read properties of undefined (reading 'name')"
  → Ada variable yang lo kira ada isinya, padahal undefined.

STEP 2: COBA MINIMAL 2 SOLUSI SENDIRI.
  "Oh error di user.name, berarti user-nya undefined.
   Coba gue trace di mana define user..."

STEP 3: KALO MASIH STUCK, BARU TANYA AI.

Prompt:
  "Error: [PASTE FULL ERROR + STACK TRACE]
   Yang udah gue coba:
   - [A] → hasilnya [X]
   - [B] → hasilnya [Y]
   Gue curiga di [TEBAKAN].
   
   1. Bener nggak tebakan gue? Kalo nggak, di mana?
   2. Kenapa error ini terjadi? Root cause.
   3. Gimana fix-nya? Kasih tau bagian SPESIFIK, bukan rewrite semua.
   4. Gimana detect ini lebih cepet next time?"
```

Kenapa harus tulis "yang udah gue coba"? Karena:
- AI nggak nyaranin yang udah lo coba
- Lo nunjukin effort — dan ke diri sendiri
- Kadang pas nulis "yang udah gue coba" lo nemu jawabannya sendiri

---

## Deadlines vs Learning: Keputusan Sadar

Ada kalanya deadline mepet. Lo butuh submit.

**Bikin keputusan sadar:**

```
"Gue pake AI buat bantu ngerjain ini karena deadline 2 jam lagi.
 TAPI gue catet bagian yang gue nggak ngerti, dan
 gue jadwalin belajar ulang weekend ini."
```

Lalu BENERAN jadwalin:
```
TODO:
- [ ] Belajar ulang JWT auth (skip pas tugas)
- [ ] Belajar ulang association many-to-many (AI generate pas tugas)
```

Kalo lo skip lagi — lo bukan nunda, lo emang nggak mau belajar. Good luck di livecode.

---

## Vibe Coding Check: Cepet-Cepet Sebelum Submit

Sebelum submit, tanya diri sendiri:

1. Bisa nggak gue jelasin setiap file di project ini fungsinya apa?
2. Bisa nggak gue jelasin flow data: dari mana request masuk, gimana diproses, balik ke mana?
3. Ada baris kode yang gue "terima aja" tanpa ngerti? (Kalo ada, catet buat dipelajari)
4. Kalo besok disuruh nambahin fitur kecil, gue bisa tanpa AI?

Kalo ada "nggak" — lo di vibe coding hell buat tugas ini. Catet, jadwalin belajar, jangan pretend lo ngerti.

---

## Coba Sendiri: Revisi Tugas Terakhir

1. **Baca kode lo.** Tanpa AI. Bisa jelasin setiap baris?
2. **Tandain yang lo nggak ngerti.** Pasti ada.
3. **Workflow B (Feynman AI)** buat jelasin bagian itu.
4. **Tulis ulang dari scratch.** Tanpa liat kode lama. Tanpa AI.
5. **Bandingin.** Mana yang lebih lo ngerti?

---

⬅️ Kembali ke [Bagian 2: 5 Workflow Belajar](02-workflow-belajar.md) | Lanjut ke [Bagian 4: Bangun Kebiasaan Belajar](04-habit-loop.md) ➡️
