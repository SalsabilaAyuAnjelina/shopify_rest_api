
# PERHATIKAN SESUAI INTRUKSI

**_Dibawah ini adalah Cara menjalankan Dockerfile, Docker-compose dan POSTMAN_**

### Persiapan Awal
Masuk ke direktori aplikasi

```bash
cd shopify-salsabilaayu
```

Sebelum menjalankan proyek, pastikan untuk menginstal semua dependensi dengan perintah berikut:

```bash
npm install
```

Untuk memverifikasi bahwa npm telah terinstal dengan benar, gunakan perintah:

```bash
npm -v
```

### Menjalankan Docker

##### 1. Sesuaikan File `/src/app.module.ts` 
TypeScript (TS) adalah superset dari JavaScript yang menambahkan fitur-fitur seperti tipe statis. Pastikan untuk menyesuaikan file ini sesuai kebutuhan aplikasi Anda.

##### 2. Menjalankan Perintah Docker
###### Build Docker Images
Perintah berikut akan membangun image untuk setiap layanan yang didefinisikan di dalam docker-compose.yml:
```bash
docker-compose build
```

###### Start Services
Setelah image berhasil dibangun, perintah berikut akan membuat dan menjalankan container untuk semua layanan dalam mode detached (di latar belakang):
```bash
docker-compose up -d
```

Anda dapat melihat daftar semua container yang sedang berjalan dengan perintah berikut:
```bash
docker ps
```

Untuk menampilkan semua container, termasuk yang sudah berhenti, gunakan perintah:
```bash
docker ps -a
```

###### Menampilkan Semua Images
Untuk melihat semua images, termasuk yang tersembunyi, gunakan perintah:
```bash
docker images -a
```

###### Opsi Lain
Selain melalui terminal, container yang sedang berjalan juga dapat dilihat melalui aplikasi Docker Desktop.

##### 3. Menjalankan docker-compose
Perintah ini akan memulai semua layanan yang didefinisikan dalam `docker-compose.yml`:
```bash
docker-compose up
```

### Menggunakan POSTMAN
Pastikan semua layanan telah berjalan dengan benar sebelum menggunakan POSTMAN untuk menguji endpoint-endpoint API.
