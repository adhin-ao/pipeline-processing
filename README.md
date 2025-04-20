
🔧 Penjelasan Pipeline Processing:
Dalam konteks komputer, pipeline processing sering digunakan di CPU, data processing, atau komputasi paralel.

Contoh:
Pada CPU, pipeline umum terdiri dari tahapan:

1. Fetch: Mengambil instruksi dari memori.
2. Decode: Menerjemahkan instruksi.
3. Execute: Menjalankan instruksi.
4. Memory Access: Mengakses data dari memori.
5. Write Back: Menyimpan hasil ke register.

Instruksi yang berbeda bisa masuk ke tahapan berbeda pada saat bersamaan. Jadi ketika instruksi pertama masuk ke tahap Execute, instruksi kedua mungkin baru saja masuk tahap Decode.

⚠️ Masalah dalam Pipeline Processing:
1. Data Hazard
 - Ketika instruksi berikutnya bergantung pada hasil dari instruksi sebelumnya yang belum selesai.
 - 🔧 Solusi: Menggunakan teknik seperti data forwarding atau stalling.
   
2. Control Hazard
- Terjadi saat ada instruksi percabangan (seperti if atau jump) yang membuat pipeline bingung harus mengambil instruksi selanjutnya dari mana.
- 🔧 Solusi: Menggunakan branch prediction atau delayed branching.

3. Structural Hazard
- Ketika dua instruksi butuh menggunakan hardware yang sama di waktu bersamaan.
- 🔧 Solusi: Menambahkan unit hardware yang cukup atau mendesain ulang pipeline agar lebih efisien.
  
4. Pipeline Stall (Bubble)
- Ketika pipeline harus berhenti sejenak karena ada ketergantungan data atau kontrol.
- 🔧 Solusi: Mengisi dengan "NOP" (No Operation) atau menggunakan teknik out-of-order execution.

✅ Keuntungan Pipeline Processing:
Meningkatkan throughput (jumlah instruksi yang diproses per satuan waktu).

Lebih efisien dibanding memproses instruksi satu per satu.

1. GeeksforGeeks – Pipelining in Computer Architecture
- Penjelasan lengkap tentang jenis-jenis hazard, solusi, dan konsep dasar pipelining.

- 🔗 https://www.geeksforgeeks.org/computer-organization-and-architecture-pipelining-set-2-dependencies-and-data-hazard

 2. Wikipedia – Pipeline (Computing)
- Memberi gambaran menyeluruh tentang sejarah, jenis pipeline, dan penerapannya di dunia nyata.

- 🔗 https://en.wikipedia.org/wiki/Pipeline_(computing)
