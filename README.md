# fullstack-apollo-express-postgresql-boilerplate

[![Status Pembuatan](https://travis-ci.org/the-road-to-graphql/fullstack-apollo-express-postgresql-boilerplate.svg?branch=master)](https://travis-ci .org/the-road-to-graphql/fullstack-apollo-express-postgresql-boilerplate) [![Slack](https://slack-the-road-to-learn-react.wieruch.com/badge.svg )](https://slack-the-road-to-learn-react.wieruch.com/) [![lencana Greenkeeper](https://badges.greenkeeper.io/the-road-to-graphql/fullstack -apollo-express-postgresql-boilerplate.svg)](https://greenkeeper.io/)

Server Apollo lengkap dengan proyek awal Klien Apollo dengan React dan Express. [Baca selengkapnya di tutorial ini untuk membuatnya sendiri](https://www.robinwieruch.de/graphql-apollo-server-tutorial/).

**Kelompok repositori fullstack universal:**

Aplikasi Server:

* [Node.js dengan Express + MongoDB](https://github.com/the-road-to-graphql/fullstack-apollo-express-mongodb-boilerplate)
* [Node.js dengan Express + PostgreSQL](https://github.com/the-road-to-graphql/fullstack-apollo-express-postgresql-boilerplate)

 Aplikasi Klien:

 * [Klien Bereaksi](https://github.com/the-road-to-graphql/fullstack-apollo-react-boilerplate)
 * [React Native Client](https://github.com/morenoh149/fullstack-apollo-react-native-boilerplate)

 ## Fitur Klien + Server

 * Bereaksi (buat-reaksi-aplikasi) dengan Klien Apollo * Kueri, Mutasi, Langganan
 * Node.js dengan Express dan Apollo Server * Pagination berbasis kursor
 * Database PostgreSQL dengan Sequelize * entitas: pengguna, pesan
 * Otentikasi * didukung oleh JWT dan penyimpanan lokal * Daftar, Masuk, Keluar
 * Otorisasi * titik akhir yang dilindungi (mis. verifikasi sesi yang valid) * resolver yang dilindungi (mis., berbasis sesi, berbasis peran) * rute yang dilindungi (mis. berbasis sesi, berbasis peran)
 * optimasi kinerja * contoh penggunaan pemuat data Facebook
 * Pengujian E2E

 ## Instalasi

 * `git klon git@github.com:the-road-to-graphql/fullstack-apollo-express-postgresql-boilerplate.git`
 * `cd fullstack-apollo-express-postgresql-boilerplate`
 * `sentuh .env`
 * `npm install`
 * isi *.env file* (lihat di bawah)
 * mulai database PostgreSQL
 * `npm mulai`
 * kunjungi `http://localhost:8000` untuk taman bermain GraphQL

 #### .env file

 Karena proyek boilerplate ini menggunakan PostgreSQL, Anda harus menginstalnya untuk mesin Anda dan mengaktifkan dan menjalankan database. Anda menemukan segalanya untuk penyiapan di sini: [Setup PostgreSQL dengan Sequelize in Express Tutorial](https://www.robinwieruch.de/postgres-express-setup-tutorial). Setelah Anda membuat database dan pengguna database, Anda dapat mengisi variabel lingkungan di file *server/.env*.

 ```
 DATABASE = basis data saya

 DATABASE_USER=postgres
 DATABASE_PASSWORD=postgres

 RAHASIA=asdlplplfwfwefwekwself.2342.dawasdq
 ```

 `RAHASIA` hanyalah string acak untuk otentikasi Anda. Amankan semua informasi ini dengan menambahkan file *.env* ke *.gitignore* file. Pihak ketiga tidak boleh memiliki akses ke informasi ini.

 #### Pengujian

 * sesuaikan skrip npm `test:run-server` dengan variabel lingkungan `TEST_DATABASE` di package.json agar sesuai dengan nama database pengujian Anda * untuk mencocokkannya dari package.json: `createdb mytestdatabase` dengan psql
 * satu terminal: npm run test: run-server
 * terminal kedua: npm run test:execute-test

 ## Ingin mempelajari lebih lanjut tentang React + GraphQL + Apollo?

 * Jangan lewatkan [Tutorial dan Kursus yang akan datang](https://www.getrevue.co/profile/rwieruch)
 * Lihat [Kursus Bereaksi] saat ini (https://roadtoreact.com)
