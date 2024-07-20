# Capstone Project: Backend Shopify-Like Application

Shopify merupakan salah satu platform e-commerce yang paling banyak digunakan. Platform ini memungkinkan kita untuk membangun web e-commerce secara mudah dan komprehensif. Secara teknis, Shopify menyediakan antarmuka grafis (frontend) untuk memudahkan pengguna awam serta antarmuka web service untuk memudahkan developer melakukan otomatisasi dan integrasi aplikasi. Web service yang disediakan pun tersedia dalam beberapa bentuk, salah satunya adalah dalam bentuk REST API yang dokumentasinya dapat diakses di REST Admin API.

## Tugas Saya

Tugas Anda adalah membuat REST API yang sesuai (mirip) dengan spesifikasi dokumentasi Shopify tersebut menggunakan bahasa pemrograman dan framework yang Anda kuasai, serta mengikuti ketentuan berikut.

### Containerization

Aplikasi dikembangkan berbasis container menggunakan Docker dan minimal terdiri dari dua service yaitu:
- **Application**: untuk deployment aplikasinya.
- **Database**: untuk deployment basis data penyimpanan datanya.

Anda bebas menggunakan bahasa pemrograman serta framework apapun untuk mengembangkan application service-nya. Begitu juga pada Database service, Anda bebas menggunakan DBMS apapun, baik relasional maupun non-relasional.

### Endpoint dan Skema Basis Data

- Ada satu tabel untuk menyimpan data pengguna dan otentikasi.
- Minimal ada empat tabel tambahan dengan memilih dari list skema yang tersedia pada REST API tersebut.
- Pada tabel pengguna, berikan minimal 20 sample data.
- Pada masing-masing tabel tambahan, berikan minimal 50 sample data.
- Terdapat satu tabel yang memiliki sample data minimal 500 data.
- Pastikan tersedia endpoint untuk `login`, `register`, `auth`, dan `refresh token`.
- Buat implementasi dari minimal 20 endpoint (tidak termasuk endpoint untuk otentikasi) yang relevan dengan tabel yang dipilih sebelumnya.
- Selain untuk kebutuhan otentikasi dan token, usahakan alamat endpoint dan skema request dan response dibuat semirip mungkin dengan spesifikasi yang ada di Shopify.
- Jika ada spesifikasi yang terpaksa tidak sesuai, berikan alasan kenapa dibuat berbeda.
- Khusus untuk kebutuhan otentikasi, tidak harus sama dengan Shopify tapi diperbolehkan menggunakan standar JWT saja.
- Pada saat pemilihan tabel, usahakan juga memilih tabel yang relevan dengan relasi tabel lain sehingga tidak banyak membuat spesifikasi yang berbeda.

### Repository dan Deployment

- Source code aplikasi, termasuk skrip containerisasi dan migrasi diupload pada repository git.
- Submitkan hanya link repository GIT, beserta penjelasan di beberapa bagian yang berbeda dari spesifikasi awal (jika ada).
- Lebih baik jika diberikan file `README.md` untuk menjelaskan langkah instalasi dan menjalankan aplikasi.
- Deploy aplikasi yang telah dibuat menggunakan VPS online, baik yang gratisan maupun yang berbayar.
- Tidak wajib menggunakan nama domain, boleh cukup diberikan alamat IP public saja.

