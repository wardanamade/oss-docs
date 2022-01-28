# OSS Docs

Repositori untuk membuat panduan dokumentasi proyek sumber terbuka RistekUSDI. Repositori ini dibangun dengan [Jigsaw](https://jigsaw.tighten.co/) - sebuah framework untuk membuat website statis dengan platform Laravel yang dibangun oleh Tighten.

## Prasyarat

PHP versi 7.4, NodeJS versi 16.3 dan NPM versi 8.1. 

## Cara menjalankan

1. Lakukan git clone.
2. Jalankan perintah `git checkout --track -b doc-site origin/doc-site`. Perintah ini akan membuat branch lokal bernama `doc-site` dan akan melakukan fetch dan pull kode dari remote bernama `origin` dengan branch remote bernama `doc-site`.
3. Jalankan perintah `composer install` untuk menginstal composer dependencies.
4. Jalankan perintah `npm install` untuk menginstal npm dependencies.
5. Jalankan perintah `npm run watch` untuk menampilkan hasil di browser.

## Cara menambahkan halaman

Untuk menambahkan halaman baru silakan menuju folder `source/docs`. Halaman baru berbasis ekstensi markdown (.md) dan isian awal dengan format berikut.

```md
---
title: Judul
description: Deskripsi untuk meta tag
extends: _layouts.documentation
section: content
---
```

Nilai `_layouts.documentation` berarti layout diambil dari folder `source/_layouts` dengan file bernama `documentation.blade.php`.