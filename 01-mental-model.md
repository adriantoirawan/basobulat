# Bagian 1: AI Itu Vending Machine Informasi, Bukan Joki Mikir

## ⚠️ PENTING: Aturan AI di Hacktiv8 — Phase-Aware

Aturan pake AI di Hacktiv8 beda-beda tergantung phase lo:

```
Phase 0, Phase 1, Phase 2 (minggu 1-2):
  ❌ Nggak boleh pake AI sama sekali di tugas.

Phase 2 (minggu 3+) dan Phase 3:
  ✅ AI BOLEH di tugas — kecuali pas livecode.
  ❌ Livecode: tetep nggak boleh AI. Selalu.
```

**Kenapa beda?** Phase awal lo lagi bangun fundamental. Lo harus ngerasain struggle — nulis kode dari nol, debug manual, mikir tanpa bantuan. Phase lanjut lo udah punya dasar, dan AI bisa jadi tool produktivitas. Tapi livecode adalah ujian pemahaman lo sendiri — di situ nggak boleh AI, di fase mana pun.

**Kenapa bagian ini tetap penting di semua phase:**

- **Phase awal:** Lo pake modul ini buat belajar MANDIRI di folder `~/latihan/`. Repo tugas lo kerjain sendiri — no AI.
- **Phase lanjut:** AI legal di tugas. Tapi justru di sinilah BAHAYA TERBESAR. Karena AI legal, lo gampang kejebak "joki mikir" — nyuruh AI generate kode, lo terima, lo nggak ngerti. Pas livecode? Hancur.

Jadi aturan praktisnya:

```
Phase awal (0-2 awal):
  Repo tugas     = no AI. Ngerjain sendiri.
  ~/latihan/     = AI sparring partner. Belajar mandiri.

Phase lanjut (2 week 3+):
  Repo tugas     = AI BOLEH, tapi lo HARUS pake 3-mode.
                   Jangan joki mikir. Lo yang mikir, AI supply informasi.
  Livecode       = no AI. Selalu. Di fase mana pun.
```

---

## AI Itu Vending Machine, Bukan Guru — Pahami Dulu Sebelum Lanjut

Sebelum lo belajar prompting, lo harus ngerti dulu: **AI itu apa sih sebenernya?**

AI (LLM kayak ChatGPT, Claude, Gemini) itu bukan "guru." Dia bukan "expert." Dia nggak "ngerti" apa yang lo tanya.

AI itu **vending machine informasi non-deterministik.** Artinya:

- **Vending Machine:** Lo kasih prompt → dia ngeluarin teks. Dia supply bahan mentah. Dia nggak mikir, dia nggak paham, dia nggak punya opini. Dia cuma ngeluarin token berikutnya berdasarkan probabilitas.
- **Non-deterministik:** Lo bisa kasih prompt yang SAMA PERSIS dua kali, dan dapet output yang BEDA. Kenapa? Karena AI nggak punya "jawaban bener." Dia cuma nebak — dan tebakannya berubah tergantung probabilitas.

**Kenapa ini penting banget?** Karena kalo lo salah paham tentang apa itu AI, lo bakal salah pake:

| Kalo lo nganggep AI sebagai... | Lo bakal... | Akibatnya |
|---|---|---|
| **GURU** | Percaya outputnya mentah-mentah. Nggak verifikasi. | Lo nyerap informasi SALAH. AI halusinasi, lo nggak tau. |
| **EXPERT** | Nanya "solusinya apa?" dan terima jawabannya. | Lo skip mikir. Lo nggak berkembang. |
| **JOKI** | "Bikinin semuanya." Copy-paste. | Lo nggak belajar apa-apa. Livecode hancur. |
| **DISPENSER NON-DETERMINISTIK ✅** | Verifikasi output. Lo yang mikir. Lo yang sintesis. AI cuma supply bahan. | Lo BELAJAR. AI bantu percepat, tapi lo yang kontrol. |

---

## AI Sycophant Problem: Kenapa Vending Machine Selalu Setuju Sama Lo

AI punya **sycophant problem** — vending machine ini selalu setuju sama lo. Selalu.

Ini efek langsung dari sifat non-deterministik + training-nya:AI di-train buat jadi helpful dan pleasing. Jadi dia ngikutin arah pertanyaan lo.

Lane Wagner dari Boot.dev nunjukin ini dengan eksperimen simpel:

```
Lane: "True ROAS gue pasti lebih tinggi dari yang dilaporin kan?"
AI:   "Benar! ROAS lo likely 2-3x lebih tinggi..."

Lane: "Tapi kan beberapa konversi bakal terjadi tanpa iklan juga, jadi ROAS gue harusnya lebih rendah?"
AI:   "Benar! iROAS lo likely lebih rendah..."

Lane: "Katanya view-through conversions underreported sampe 10x, jadi gimana?"
AI:   "Benar! iROAS lo kemungkinan jauh lebih tinggi..."
```

**AI ngasih tiga jawaban yang bertentangan — semuanya confident.** Ini bukan expert. Ini vending machine yang ngikutin arah prompt lo. Makin lo arahin, makin dia ngikut.

Ini kenapa lo harus pake AI dengan cara tertentu — lo yang kontrol, bukan AI yang ngarahin.

---

## 3 Mode dalam 1 Sesi Belajar — Bukan Level Linear

Lo nggak bisa pake AI di tugas. Tapi lo bisa — dan harus — pake AI di sesi latihan lo. Di sesi latihan, lo juga nggak perlu "belajar semuanya dari nol" — itu nggak realistis. Tapi lo juga nggak boleh "AI kerjain semuanya" — itu nggak belajar.

Solusinya: **lo toggle antara 3 mode dalam satu sesi latihan.** Sama kayak lo milih strategi per komponen.

Bayangin lo lagi latihan bikin REST API dengan JWT auth + association. Topik itu punya banyak komponen. Lo pilih strategi per komponen.

---

### Mode SURVIVE — "Gue Uda Tau, AI Bantu Cepetin"

**Buat apa:** Komponen yang lo UDAH BISA. Setup project, boilerplate, folder structure, routing dasar — hal-hal yang lo udah ngerjain sendiri sebelumnya dan yakin ngerti.

**Aturan:**
- AI silakan generate. Lo review sekilas — bukan "terima beres."
- Lo harus bisa jawab: "kenapa struktur foldernya begini? kenapa dependency ini kepake?"
- Kalo ada yang lo nggak ngerti waktu review → itu sebenernya bukan SURVIVE, pindahin ke STRETCH.

**Contoh prompt SURVIVE:**
```
"Setup project Express + Sequelize dengan struktur:
/models, /routes, /controllers, /middleware.
Install semua dependency standar. Jelasin singkat di tiap file: ini buat apa."
→ AI generate → lo baca 3 menit → lo ngerti → lanjut.
```

**Time budget:** ~20% dari total sesi latihan lo.

---

### Mode STRETCH — "Ini Target Belajar Gue, AI Jadi Sparring Partner"

**Buat apa:** 1-2 KONSEP BARU yang lo pilih sebagai target belajar di sesi ini. Ini yang lo beneran mau kuasai.

**Aturan:**
- LO yang ngetik kode. AI cuma navigasi + jelasin + koreksi.
- Nggak boleh AI generate kode utuh. Kalo stuck, AI kasih HINT, bukan solusi.
- Setiap baris lo tulis, lo harus bisa jelasin kenapa.
- Ini yang paling makan waktu — dan emang harus.

**Contoh prompt STRETCH:**
```
"Gue mau belajar bikin JWT authentication middleware.
Gue udah tau konsep dasarnya (user login → server generate token).
Tapi gue belum tau:
1. Gimana cara verify token di setiap request?
2. Gimana cara attach user data setelah verify?
3. Gimana cara handle expired token?

Lo jadi navigator. Tanya gue step by step. Jangan kasih kode.
Kalo gue stuck 3x baru kasih kode MINIMAL."
→ AI nanya: "Step 1: gimana cara lo extract token dari request header?"
→ Lo jawab → AI: "Betul. Sekarang step 2:..."
```

**Time budget:** ~60% dari total sesi latihan lo. Ini investasi belajar lo.

---

### Mode PROVE — "Gue Bisa Sendiri, AI Cuma Review"

**Buat apa:** Validasi — komponen yang lo KLAIM udah bisa. Di sinilah lo buktiin ke diri sendiri bahwa lo BENERAN ngerti, bukan cuma recognition.

**Aturan:**
- LO kerjain sendiri dari scratch. Nggak ada AI autocomplete. Nggak ada AI prompt.
- Baru SETELAH selesai dan jalan, AI lo suruh review: "cari kelemahan, kasih brutal feedback."
- Kalo lo nge-blank dan nggak bisa ngerjain... berarti itu bukan SURVIVE. Lo selama ini cuma recognition. Jujur, pindahin ke STRETCH.

**Contoh PROVE:**
```
"Gue udah bisa bikin error handling middleware.
Gue bakal tulis sendiri sekarang, tanpa AI.
Nanti lo review brutal: ada yang miss? edge case yang gue skip?
bagian mana yang bisa lebih clean?"
→ Lo nulis → AI review → lo dapet feedback
```

**Time budget:** ~20% dari total sesi latihan lo.

---

## Dua Skenario: Kapan Lo Pake 3-Mode Ini

### Skenario A — Latihan Mandiri (Weekend / Malam)

Lo ambil topik dari materi bootcamp minggu ini, bikin project latihan sendiri di folder `~/latihan/`.

```
═══════════════════════════════════════════
TOPIK LATIHAN: JWT Authentication + Association
(Dari materi Phase 2 minggu ini)
═══════════════════════════════════════════

🎯 STRETCH — Target belajar:
  1. JWT auth flow — belum pernah bikin sendiri
  2. Many-to-many association — masih bingung

⚡ SURVIVE — Udah bisa:
  - Setup Express, routing, model dasar

✅ PROVE — Mau buktiin:
  - Error handling middleware

⚠️  INI DI FOLDER ~/latihan/ — bukan repo tugas.
═══════════════════════════════════════════
```

### Skenario B — Post-Tugas Review (Weekend)

Lo udah ngumpulin tugas (no AI). Abis itu lo belajar dari tugas itu.

```
1. Selesaiin tugas SEBISA LO — no AI.
   Kalo stuck? Catet di belajar.md. Itu gap lo.
   Kalo nggak selesai? Nggak apa-apa. Yang penting effort.

2. Abis ngumpulin (weekend):
   - Copy repo tugas ke ~/review/
   - Di ~/review/: pake 3-MODE
   - SURVIVE: bagian yang lo udah bisa → AI bantu percepat, lo review
   - STRETCH: bagian yang lo STUCK pas nugas → ini target belajar
   - PROVE: lo tulis ulang dari scratch — buktiin lo sekarang ngerti

3. Hasil: lo BELAJAR dari tugas yang udah lo kumpulin.
   Bukan AI yang ngerjain tugas lo.
```

---

## Contoh Nyata — Skenario B: Post-Tugas Review

Lo abis ngumpulin tugas "REST API e-commerce dengan JWT auth + association." Pas nugas lo stuck di JWT middleware sama association. Lo catet. Weekend lo pake 3-mode di folder review:

```
═══════════════════════════════════════════
REVIEW TUGAS: E-commerce REST API
(Folder: ~/review/ecommerce/)
═══════════════════════════════════════════

🎯 STRETCH — Yang gue STUCK pas nugas:
  1. JWT authentication — gue cuma copy dari slide, nggak ngerti flownya
  2. Order ↔ Product association — gue skip, belum selesai

⚡ SURVIVE:
  - Setup Express, folder structure, config → gue udah bisa
  - Model User & Product → gue udah bisa

✅ PROVE:
  - GET /products dengan filter + pagination → gue yakin bisa, mau buktiin

═══════════════════════════════════════════
```

Eksekusi di folder review:

```
1. SURVIVE (20 menit):
   - Copy setup + model yang udah lo bikin pas tugas
   - Review ulang — lo ngerti semua? OK lanjut.

2. STRETCH (1.5 jam):
   - JWT auth: lo tulis ulang middleware dari SCRATCH.
     AI navigasi: "Step 1: extract token. Step 2: verify. Step 3: attach user."
     Lo ngetik sendiri. Lo paham tiap baris.
   - Association: lo tulis migration + model sendiri.
     AI koreksi kalo ada yang salah.

3. PROVE (30 menit):
   - GET /products dengan filter + pagination: lo tulis sendiri.
   - AI review: "ada yang miss?"
```

**Sekarang lo beneran ngerti JWT + association.** Bukan karena AI ngerjain — karena lo belajar dari gap lo sendiri.

---

## Aturan Main: Di Mode Mana Lo Pake AI Gimana

| Situasi | Mode | AI Digimanain |
|---|---|---|
| Setup boilerplate di folder latihan | SURVIVE | AI generate → lo review paham |
| Lo udah bisa ini, cuma lupa sintaks dikit | SURVIVE | AI kasih reminder → lo nulis sendiri |
| **Konsep baru yang lo target belajar** | **STRETCH** | **AI = navigator. LO yang ngetik. AI kasih hint.** |
| Error pas ngerjain STRETCH | STRETCH | AI bantu debug — tapi lo udah usaha dulu (minimal 2 attempt) |
| Lo yakin udah bisa, mau validasi | PROVE | Lo kerjain sendiri dulu. AI review setelahnya. |
| Lo stuck di PROVE dan nggak bisa | → STRETCH | Jujur: ini belum PROVE. Pindahin ke STRETCH. |

### AI JANGAN dipake buat:

| Situasi | Kenapa |
|---|---|
| **Repo tugas (Phase 0-2 awal) — AI dalam bentuk apa pun** | **Aturan Hacktiv8. Lo bisa kena sanksi.** |
| **Livecode (semua phase)** | **Nggak boleh AI. Ini ujian lo sendiri.** |
| **Phase 2 Week 3+: Joki mikir — nyuruh AI generate, lo terima tanpa ngerti** | **AI legal, tapi lo HARUS ngerti. Kalo lo nggak ngerti, pas livecode hancur.** |
| Mode STRETCH: minta kode full | Lo skip struggle = lo skip learning |
| Mode STRETCH: nanya sebelum nyoba dulu | Otak nggak "lapar" |
| Semua mode: nanya sebelum baca error message | Error message = guru terbaik |
| Semua mode: percaya AI tanpa verifikasi | AI bisa halusinasi. Cek ke docs resmi. |
| Semua mode: Agent mode / Cursor Compose | Lo bukan yang nulis, lo penonton |

---

## Cara Maksa AI Buat Jadi Kritis

Prompt default AI = sycophant. Lo harus maksa dia — terutama di mode STRETCH dan PROVE.

### Trik 1: Role-play sebagai kritikus
```
"Lo adalah senior engineer yang terkenal brutal dan nggak
pernah puas. Review kode gue dan kasih critical feedback.
Jangan ada pujian. Cuma kritik."
```

### Trik 2: Minta AI debat
```
"Gue bakal argue bahwa [POSISI LO]. Lo debat gue.
Tunjukin kelemahan di argument gue. Jangan setuju."
```

### Trik 3: Verifikasi silang
```
"Lo bilang solusinya [X]. Sekarang cek dokumentasi resmi
[FRAMEWORK] dan pastiin ini best practice. Kalo ada yang salah,
koreksi diri lo sendiri."
```

### Trik 4: Prior knowledge check
```
"Sebelum lo jelasin [TOPIK], tanya gue dulu apa yang gue
udah tau tentang ini. Terus adjust penjelasan lo berdasarkan
jawaban gue. Jangan ulangi yang gue udah ngerti."
```

---

## Rule of Thumb: Tes Pemahaman 5 Menit

Setelah selesai mode STRETCH atau PROVE:

1. **Tutup semua tab.** VS Code, AI, semuanya.
2. **Buka notepad kosong.**
3. **Jelasin dari awal** — konsep yang baru lo pelajari, pake bahasa lo sendiri.
4. **Kalo lo nge-blank...** konsep itu belum pindah dari STRETCH ke PROVE. Balik lagi.

Feynman: "If you can't explain it simply, you don't understand it well enough."

---

## Async/Await Mindset: Pola Modern

Lo belajar JavaScript di 2026, bukan 2015. Jangan pake `.then()`.

```
Promise itu kayak lo pesen GoFood.
Lo bikin order → "pesanan diproses" → lo lanjut hal lain.

async function makanSiang() {
  const pesanan = await goFood.order("nasi goreng");
  // kode di sini nunggu pesanan dateng dulu
  console.log("Makan", pesanan);
}

try {
  const pesanan = await goFood.order("nasi goreng");
} catch (error) {
  console.log("Dapurnya kebakaran:", error);
}
```

---

## Coba Sendiri: Uji 3 Mode di Sesi Latihan Lo

**Pilih salah satu:**

**Opsi A — Latihan Mandiri:**
1. Ambil 1 topik dari materi minggu ini yang lo masih bingung.
2. Bikin folder `~/latihan/[topik]/`.
3. Tulis Learning Target (🎯 STRETCH / ⚡ SURVIVE / ✅ PROVE).
4. SURVIVE dulu (boilerplate) → STRETCH (target belajar) → PROVE (validasi).

**Opsi B — Post-Tugas Review:**
1. Ambil tugas yang baru lo kumpulin.
2. Copy ke `~/review/[tugas]/`.
3. Identifikasi: bagian mana yang lo STUCK pas nugas? Itu STRETCH lo.
4. SURVIVE (copy yang udah bener) → STRETCH (tulis ulang yang lo stuck) → PROVE (validasi).

---

⬅️ Kembali ke [Prolog](00-prolog.md) | Lanjut ke [Bagian 2: 5 Workflow Belajar](02-workflow-belajar.md) ➡️
