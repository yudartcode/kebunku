# Kebun Yuda

Portofolio L Yuda Rahmani Karnaen, full stack developer, dalam bentuk kebun pixel art yang bisa dijelajahi. Proyek tersimpan di bangunan, keahlian tumbuh di ladang, dan seluruh isi CV juga tersedia sebagai teks biasa di bawah gim bagi yang ingin langsung membaca.

**Demo:** [tambahkan alamat situs di sini]

## Yang ada di kebun

| Tempat | Isi |
| --- | --- |
| Rumah | Profil singkat |
| Lumbung | Proyek yang sudah dibangun |
| Bengkel | Kegiatan development sehari-hari |
| Kebun bibit | Proyek yang sedang dikerjakan |
| Ladang | 12 keahlian yang bisa dipanen |
| Kotak surat | Kontak |

Ada juga beberapa hal kecil untuk ditemukan:

- Anak yang bermain bola di halaman, ibu yang memasak di balik jendela dapur, dan ayam yang berkeliaran. Semuanya bisa disapa.
- Musim dan cuaca mengikuti tanggal pengunjung: Musim Hujan pada November sampai Maret, Musim Kemarau pada bulan lainnya.
- Terang dan gelapnya kebun mengikuti jam pengunjung.
- Bulan purnama naik setelah semua keahlian dipanen.
- Musik latar bernada slendro, dibuat langsung di browser. Bisa dinyalakan lewat tombol Musik.

## Cara bermain

| Aksi | Keyboard | Layar sentuh atau mouse |
| --- | --- | --- |
| Berjalan | Tombol panah atau WASD | Ketuk atau klik tujuan |
| Berinteraksi | E, Spasi, atau Enter | Ketuk atau klik objeknya |
| Menutup dialog | Esc | Tombol Tutup |
| Pergi ke suatu tempat | - | Tombol di bawah layar gim |

## Teknologi

- HTML, CSS, dan JavaScript murni dalam satu file, tanpa framework dan tanpa proses build
- Canvas 2D untuk semua grafis, digambar lewat kode tanpa file gambar
- Web Audio API untuk musik dan efek suara
- `localStorage` untuk menyimpan hasil panen pengunjung
- Google Fonts untuk Pixelify Sans dan Bitter

## Menjalankan secara lokal

Buka `index.html` langsung di browser, atau jalankan server lokal:

```bash
python3 -m http.server 8000
```

Lalu buka `http://localhost:8000`.

## Mengubah isi

Semua isi portofolio ada di bagian atas tag `<script>` di `index.html`, di bawah komentar `Isi portofolio`. Perubahan di sana berlaku untuk gim dan catatan sekaligus.

| Konstanta | Isi |
| --- | --- |
| `KONTAK` | Jalur kontak |
| `PROYEK` | Daftar proyek. `tempat` menentukan bangunannya, `tahap` menentukan statusnya (`tumbuh` atau `panen`) |
| `KEGIATAN` | Kegiatan development di bengkel |
| `KERJA` | Riwayat kerja |
| `TANAMAN` | Keahlian di ladang beserta posisi petaknya |

Profil, pendidikan, dan bahasa ditulis langsung di HTML, di bagian `Si Pemilik Kebun`. Dialog rumah ada di objek `PLACES`.

## Deploy

Karena hanya berupa satu file statis, situs ini bisa dipasang di hosting statis apa pun.

**GitHub Pages:** buka Settings → Pages, pilih **Deploy from a branch**, lalu pilih cabang `main` dan folder `/ (root)`.

**Netlify:** seret folder proyek ini ke [app.netlify.com/drop](https://app.netlify.com/drop).

## Catatan

Kebun ini terinspirasi dari gim bertani klasik. Semua karakter, grafis, dan musiknya dibuat khusus untuk proyek ini, tanpa aset dari gim mana pun.

## Kontak

[LinkedIn](https://www.linkedin.com/in/yudakarnaen/)
