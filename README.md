# Promo Ultah 🎂

Kumpulan birthday treat dari 49 brand di Indonesia, dalam satu halaman. Isi tanggal ultah lo, dan app ini langsung nunjukin promo mana yang bisa diklaim kapan, sampai kapan, dan kapan paling lambat lo harus udah daftar member.

## Fitur

- **Daftar promo**: cari brand atau hadiah, terus filter per kategori (makanan, minuman, dessert, lainnya), tanpa minimal belanja, gak perlu member, atau gratisan aja.
- **Tanggal ultah**: tiap promo dapet status *bisa diklaim*, *belum mulai*, atau *udah lewat*, plus pengingat batas daftar member (mis. Fore 3 bulan, Starbucks 1 bulan, Marugame 31 hari).
- **Jadwal klaim**: timeline semua periode promo dan daftar tanggal penting (mulai, hari terakhir, batas daftar member).
- **Checklist**: tandain promo yang udah diklaim tahun ini.
- **Tambah promo sendiri**: tambah, edit, atau hapus promo di luar daftar bawaan.

## Privasi

Gak ada server, akun, atau tracking. Tanggal ultah, checklist, dan promo tambahan cuma disimpen di `localStorage` browser masing-masing. Kalau data browser dihapus atau pindah device, datanya gak ikut.

## Data

Data awal diambil dari poster Promo Ultah yang beredar di medsos, lalu dicek ulang (19 Nov 2026) ke artikel 2026 (Tuwaga, IDN Times, ESB, Beautynesia, Disway, Bloomberg Technoz) dan akun resmi brand. Tiap promo punya label verifikasi dan link sumber di halaman detailnya. Kalau sumbernya beda-beda, promo itu dikasih tanda **⚠ Cek dulu**.

Syarat bisa beda per cabang dan bisa berubah kapan aja. Konfirmasi ke outlet sebelum pesan, dan jangan lupa bawa KTP.

### Update data

Semua data bawaan ada di array `BUILTIN` di `index.html`. Format periode:

- `w: {f: -7, t: 7}` = H-7 s.d. H+7 (offset hari dari tanggal ultah)
- `w: {m: 1}` = sebulan penuh di bulan ultah
- `l: 30` = member harus udah terdaftar min. 30 hari sebelum ultah
- `days: [1,2,3,4]` = cuma berlaku kalau ultah jatuh Senin–Kamis

## Jalanin

Cukup satu file statis. Buka `index.html` di browser, atau host di GitHub Pages (Settings → Pages → Deploy from branch → `main` / root).

Logo brand sengaja gak ditampilin; ikon di kartu cuma penanda.
