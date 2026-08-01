# Appendix: Senjata Tambahan

Ini referensi cepet. Simpen, bookmark, balik pas lo butuh.

---

## Prompt Template Library

Copy-paste prompt ini dan isi placeholder-nya.

### Template 1: Belajar Konsep Baru
```
"Gue mau belajar [TOPIK] dari nol.
Asumsi: gue cuma tau [BASIC_KNOWLEDGE].
Tolong:
1. Jelasin dgn analogi sederhana (bukan jargon teknis)
2. Tunjukin 3 common mistakes pemula
3. Kasih 5 pertanyaan buat ngetes pemahaman gue nanti
4. JANGAN kasih kode. Konsep dulu."
```

### Template 2: Cek Pemahaman (Feynman)
```
"Gue bakal jelasin [TOPIK] pake bahasa gue sendiri.
Lo jadi guru killer yg brutal. Koreksi semua kesalahan.
Jangan basa-basi. Jangan bilang 'good job'.
Gue mulai: [JELASIN]"
```

### Template 3: Debugging
```
"Error: [PASTE FULL ERROR + STACK TRACE]
Kontext: [APA YG LO LAGI KERJAIN]
Udah gue coba: [A], [B], [C]
Gue curiga: [TEBAKAN]
1. Bener nggak tebakan gue? Kalo nggak, di mana?
2. Root cause-nya apa?
3. Fix spesifik (jangan rewrite semua)"
```

### Template 4: Breakdown Tugas
```
"Tugas gue: [PASTE SOAL]
Tolong breakdown jadi step kecil tanpa kode:
1. [X step]
Untuk setiap step, tandain:
- [✓] Kalo gue harusnya udah bisa sendiri
- [?] Kalo gue mungkin perlu review
- [!!] Kalo gue harus belajar dari nol
JANGAN kasih kode."
```

### Template 5: Code Review Brutal
```
"Review kode gue dengan brutal. Cari:
1. Security holes
2. Performance issues
3. Bad practices
4. Edge cases yg gue miss
5. Naming yg jelek
6. Logic yg bisa disederhanakan
Jangan puji. Kritik langsung. Kode gue: [PASTE]"
```

### Template 6: Pair Programming
```
"Kita pair-programming buat [FEATURE].
Aturan:
- GUE yg ngetik, lo cuma navigasi + tanya
- Stuck? Kasih hint dulu, bukan solusi
- Udah 3x gagal? Baru kasih kode minimal
- Setiap step, tanya: 'ngerti kenapa pake ini?'
Mulai: step pertama apa?"
```

### Template 7: Quiz Generator
```
"Gue abis belajar [TOPIK] dari resource: [LINK/TEXT]
Bikinin 10 soal:
3 gampang (definisi)
4 medium (penerapan)
3 susah (edge cases + tradeoff)
JANGAN kasih jawaban dulu."
```

### Template 8: Spaced Repetition Scheduler
```
"Lo jadi spaced repetition scheduler gue.
Ini yg gue pelajari hari ini: [TOPIK/DETAIL]
Bikinin jadwal review:
- Hari 1 (besok): gue harus recall apa? kasih pertanyaan
- Hari 3: bikinin quiz singkat
- Hari 7: gue jelasin balik, lo jadi guru killer
- Hari 14: kasih problem baru yg pake konsep ini
- Hari 30: suruh gue bikin mini-presentation
Simpen jadwal ini. Ingetin gue pas waktunya."
```

### Template 9: Accountability Partner
```
"Lo jadi accountability partner gue buat belajar [SKILL].
Tiap gue cerita progress:
1. Tanya: 'beneran ngerti atau copy-paste?'
2. Tantang: 'coba jelasin balik sekarang'
3. Kalo gue skip sesuatu, ingetin minggu depan
4. Kalo gue kelamaan nggak update, tanya 'kenapa?'
Mulai: gue baru selesai [APA]..."
```

### Template 10: Analogi Generator
```
"Jelasin [TOPIK] pake analogi. JANGAN pake jargon teknis.
Target: bisa gue jelasin ke anak SMA.
Kalo analogi pertama kurang pas, coba analogi berbeda
sampe yg bener-bener 'klik' di otak gue."
```

### Template 11: Socratic Drill
```
"Lo jadi guru Socratic buat topik [TOPIK].
Lo nggak ngasih jawaban — lo cuma nanya.
Mulai dari pertanyaan gampang, naik terus.
Kalo gue jawab salah, tanya lagi dari angle beda.
Jangan kasih tau jawabannya. Maksa gue mikir."
```

---

## Curated Resource Links

### Tentang Cara Belajar

| Resource | Link | Best For |
|---|---|---|
| Dan Koe — How To Learn 10X Faster With AI | thedankoe.com/letters/how-to-learn-anything-10x-faster-than-anyone-with-ai/ | Mindset + framework |
| Nitin Sharma — 6 AI Learning Workflows | aimadesimple0.substack.com (post 187367499) | Workflow konkret |
| Boot.dev — Vibe Coding Hell | boot.dev/blog/education/vibe-coding-hell | Kenapa AI bikin lo nggak belajar |
| freeCodeCamp — Escape Tutorial Hell | freecodecamp.org/news/how-to-learn-from-coding-tutorials-and-avoid-tutorial-hell | Cara bener pake tutorial |

### Tentang Active Recall & Spaced Repetition

| Resource | Link | Best For |
|---|---|---|
| JungleAI — Active Recall with AI | jungleai.com/blog/how-to-improve-your-active-recall-practice-with-ai | Tools untuk active recall |
| Recallify — Spaced Repetition Science | recallify.ai/boost-memory-with-active-recall-and-spaced-repetition | Evidence + teknik |
| Dunlosky et al. (2013) — Learning Techniques | journals.sagepub.com (search "Dunlosky improving students learning") | Meta-review 10 teknik belajar |

### Tools Rekomendasi

| Tool | Fungsi | Gratis? |
|---|---|---|
| ChatGPT / Claude | Sparring partner, quiz generator, scheduler | Free tier cukup |
| Perplexity AI | Cari resources + deep research | Free tier cukup |
| NotebookLM | Knowledge base dari banyak resource + quiz + audio summary | Gratis (Google) |
| Wisdolia | Auto-generate flashcard dari PDF/notes/YouTube | Freemium |
| Anki | Flashcard app dengan spaced repetition built-in | Gratis (open source) |

---

## Rules Tambahan

1. **Selalu verifikasi ke dokumentasi resmi.** AI bisa halusinasi. Kalo AI ngasih info teknis, cek ke docs resmi (expressjs.com, react.dev, nodejs.org, dll).

2. **Jangan pake Agent Mode / Cursor Compose buat belajar.** Tools ini dirancang buat produktivitas engineer yang UDAH BISA, bukan buat belajar. Lo skip process berpikir.

3. **AI autocomplete: matiin.** Fitur "tab to complete" di Cursor/Copilot itu belajar killer. Lo nggak mikir, lo cuma terima saran. Matiin pas jam belajar.

4. **Jam belajar ≠ jam pake AI.** Target lo: makin lama, makin dikit pake AI. Kalo lo masih prompt AI 50x per jam setelah 3 bulan, ada yang salah.

5. **Kalo bingung, balik ke INDEX.** Modul ini reference loop. Lo bisa balik kapan aja.

---

⬅️ Kembali ke [Bagian 5: Kamus + Baca Ulang](05-meta.md) | Kembali ke [INDEX](INDEX.md)
