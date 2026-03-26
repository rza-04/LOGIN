# Login + Dashboard dengan Session

Project sederhana menggunakan **Express + express-session**.

## Fitur
- Halaman login (`/login`)
- Halaman dashboard terlindungi (`/dashboard`)
- Session server-side
- Logout (`/logout`)

## Akun Demo
- Username: `admin`
- Password: `admin123`

## Jalankan Project
1. Install Node.js LTS terlebih dahulu.
2. Install dependency:
   ```bash
   npm install
   ```
3. Jalankan server:
   ```bash
   npm start
   ```
4. Buka di browser: `http://localhost:3000`

## Alur Session
- Jika login berhasil, user disimpan di `req.session.user`.
- Route dashboard diproteksi middleware `requireAuth`.
- Setelah logout, session dihapus dan cookie session dibersihkan.
