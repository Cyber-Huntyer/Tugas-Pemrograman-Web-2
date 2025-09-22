## Pertanyaan Readme
1. **keputusan gap tiap breakpoint**
   - Supaya foto tampil satu per baris, karena layar HP kecil. User bisa scroll ke bawah dengan nyaman.
   - Tablet punya lebar lebih besar, jadi bisa menampilkan 2 foto berdampingan. Layout tetap rapi tanpa terlihat terlalu sempit.
   - Layar laptop/desktop jauh lebih lebar, sehingga 4 foto per baris membuat tampilan mirip Instagram asli.

2. **utility responsive Tailwind**
   - ada elemen feed yang col-span-2 di layar lebih besar, tapi tetap col-span-1 di mobile agar tidak rusak.
   - grid-cols-1 md:grid-cols-2 lg:grid-cols-4. otomatis menyesuaikan jumlah kolom sesuai ukuran layar.

3. **utility classes vs membuat Component CSS tersendiri.**
   - Trade-off: Tailwind lebih praktis & cepat untuk prototyping atau project kecil, sedangkan

   - CSS component lebih cocok jika project sangat besar dan butuh konsistensi dengan banyak developer.

