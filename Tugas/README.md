# Form Pendaftaran Kursus

## Deskripsi
Proyek ini merupakan prototype form pendaftaran kursus berbasis website menggunakan HTML, CSS, dan JavaScript. Form ini memenuhi tugas individu (minimal lima tipe input, tiga jenis button, dan label yang terhubung) sekaligus studi kasus penerimaan mahasiswa baru (nama, email, password, nilai, dan tanggal lahir yang siap diintegrasikan dengan backend).

## Fitur
- Input nama lengkap (text)
- Input alamat email (email)
- Input password (password, minimal 8 karakter)
- Input nilai / skor (number, 0 sampai 100)
- Input tanggal lahir (date)
- Tombol Daftar Sekarang (submit)
- Tombol Reset Form (reset)
- Tombol Lihat Info (button)
- Pesan hasil validasi di bawah tombol
- Setiap field memiliki label, id, name, dan tipe input yang sesuai

## Daftar Field

| Label | id | name | Tipe input |
|---|---|---|---|
| Nama lengkap | nama | nama | text |
| Alamat email | email | email | email |
| Password | password | password | password |
| Nilai / skor | nilai | nilai | number |
| Tanggal lahir | tanggalLahir | tanggal_lahir | date |

## Teknologi
- HTML untuk membuat struktur form
- CSS untuk mengatur tampilan website
- JavaScript untuk mengatur interaksi form

## Struktur Folder
DW/
- index.html
- style.css
- DESKTOP.png
- MOBILE.png
- README.md

## Cara Menjalankan
1. Buka folder proyek di Visual Studio Code.
2. Buka file index.html.
3. Jalankan menggunakan Live Server atau browser.
4. Isi seluruh data pendaftaran.
5. Klik tombol Daftar Sekarang untuk memeriksa validasi. Jika semua field valid, muncul pesan "Form valid!".
6. Klik Lihat Info untuk menampilkan petunjuk pengisian, atau Reset Form untuk mengosongkan isian.

## Integrasi Backend
Form menggunakan method POST karena data pendaftaran tidak boleh tampil di URL. Atribut action masih berisi "#" dan dapat diganti dengan endpoint backend yang sebenarnya. Atribut name pada setiap field (nama, email, password, nilai, tanggal_lahir) menjadi key data yang diterima backend. Pada prototype ini pengiriman ke server dihentikan oleh JavaScript (preventDefault) dan hanya menampilkan hasil validasi.

## Responsif
Website dirancang agar dapat dibuka melalui desktop dan perangkat mobile. Pada layar kecil, padding form mengecil dan tombol tersusun vertikal.

## Catatan
Proyek ini masih berupa prototype frontend dan belum menggunakan database maupun backend. Validasi di browser (required, minlength, min, max) hanya pengaman awal, sehingga validasi tetap perlu dilakukan di sisi server.
