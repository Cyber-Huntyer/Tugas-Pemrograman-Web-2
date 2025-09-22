# 📸 Instagram Profile Clone - Tailwind CSS

Project ini adalah implementasi halaman profil Instagram sederhana menggunakan **Tailwind CSS**.  
Tujuannya untuk latihan membuat layout **responsif** dengan utility-first framework tanpa menulis CSS manual.

---

## 🚀 Fitur Utama
1. **Struktur Halaman Lengkap**
   - Header Profil (foto, username, tombol, statistik, bio).
   - Feed (12 gambar dummy).
   - Footer.

2. **Responsif**
   - Mobile (default): 1 kolom (`grid-cols-1`).
   - Tablet (`md:`): 2 kolom (`md:grid-cols-2`).
   - Desktop (`lg:`): 4 kolom (`lg:grid-cols-4`).

3. **Penggunaan Utility Tailwind**
   - **Responsive Utility**: contoh `md:grid-cols-2`, `lg:grid-cols-4`.
   - **Grid Nesting & Col-span**: salah satu card di feed menggunakan `col-span-2` dan nested grid.
   - **Responsive Order & Layout**: tombol `Follow` berubah ukuran antar breakpoint (`md:text-base md:px-6`).

4. **Style Menggunakan Tailwind**
   - Spacing (`p-4`, `mt-4`, `space-x-4`).
   - Alignment (`flex`, `items-center`, `justify-between`).
   - Shadow & Rounded (`shadow`, `rounded`).
   - Typography (`text-sm`, `font-bold`, `text-gray-500`).

---

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