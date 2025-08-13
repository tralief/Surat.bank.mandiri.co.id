# Paket 'Terima Jadi' — Surat.bank.mandiri.co.id

File ini siap dideploy (hosting) agar bisa diakses online di `https://Surat.bank.mandiri.co.id`.

## Struktur
- `index.html` — halaman utama, sudah berisi tautan HTTPS dan informasi surat
- `qr-surat-bank-mandiri.png` — gambar QR yang menunjuk ke `https://Surat.bank.mandiri.co.id`
- `CNAME` — (opsional) untuk GitHub Pages custom domain
- `netlify.toml` — (opsional) untuk Netlify
- `vercel.json` — (opsional) untuk Vercel

## Cara Deploy (pilih salah satu)

### Opsi A — Netlify (paling mudah)
1. Buat akun di Netlify dan klik **Add new site → Deploy manually**.
2. Drag & drop seluruh isi folder ini ke Netlify.
3. Buka **Site settings → Domain management → Custom domains**, tambahkan `Surat.bank.mandiri.co.id`.
4. Di DNS domain Anda, buat **CNAME** untuk `Surat` yang mengarah ke subdomain Netlify yang diberikan (mis. `your-site.netlify.app`).
5. Tunggu propagasi DNS, Netlify akan aktifkan HTTPS otomatis (Let's Encrypt).

### Opsi B — Vercel
1. Login ke Vercel → **Add New… → Project → Import** folder ini.
2. Setelah deploy, buka **Settings → Domains**, tambahkan `Surat.bank.mandiri.co.id`.
3. Ikuti instruksi DNS (CNAME) yang ditampilkan Vercel.
4. HTTPS akan aktif otomatis setelah DNS benar.

### Opsi C — GitHub Pages
1. Buat repositori di GitHub dan unggah semua file.
2. Aktifkan **Settings → Pages → Deploy from branch** (root).
3. Pastikan file `CNAME` berisi `Surat.bank.mandiri.co.id`.
4. Tambahkan DNS **CNAME** `Surat` → `username.github.io` (atau target yang disarankan).
5. Tunggu propagasi; HTTPS bisa diaktifkan di Settings → Pages.

> Catatan: Anda harus memiliki akses DNS ke domain `bank.mandiri.co.id` untuk membuat subdomain `Surat`. Jika tidak, gunakan subdomain Anda sendiri yang tersedia.

