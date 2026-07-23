# RZAA STORE — Price List

Landing page jasa penyediaan nomor fresh (WhatsApp, Shopee, Tokopedia, Lazada, TikTok, Grab, Gojek). Static site, single file, tema dark terminal/glassmorphism, ada sound effect pas item di-klik dan auto-generate link WhatsApp sesuai layanan yang dipilih.

## Struktur

```
.
└── index.html
```

Semua HTML, CSS, JS ada dalam satu file `index.html` — gak butuh build step, gak butuh dependency apa pun.

## Jalanin lokal

Tinggal buka `index.html` di browser, atau kalau mau lewat local server:

```bash
npx serve .
```

## Push ke GitHub

```bash
git init
git add .
git commit -m "init: RZAA STORE price list"
git branch -M main
git remote add origin https://github.com/USERNAME/NAMA-REPO.git
git push -u origin main
```

Ganti `USERNAME/NAMA-REPO` sesuai repo GitHub yang lo buat.

## Deploy ke Vercel

1. Buka [vercel.com/new](https://vercel.com/new)
2. Pilih **Import Git Repository**, connect akun GitHub lo kalau belum
3. Pilih repo yang barusan di-push
4. Framework preset: pilih **Other** (soalnya ini static HTML biasa, bukan Next.js/dll)
5. Build command & output directory: kosongin aja / biarin default, Vercel otomatis serve `index.html`
6. Klik **Deploy**

Selesai — nanti dapet URL `nama-project.vercel.app`.

## Catatan

Nomor WhatsApp tujuan ada di `index.html`, cari variabel `WA_NUMBER` kalau mau ganti.
