# Analisis HTTP dan JSON

## HTTP Method

### GET
Digunakan untuk mengambil data dari server tanpa mengubah data yang sudah ada.

Contoh:

GET /api/transactions

### POST
Digunakan untuk menambahkan data baru ke server.

Contoh:

POST /api/transactions

---

## Status Code

### 200 OK
Request berhasil diproses.

### 201 Created
Data berhasil dibuat.

### 400 Bad Request
Format request salah.

### 401 Unauthorized
Client belum memiliki hak akses.

### 404 Not Found
Resource tidak ditemukan.

### 500 Internal Server Error
Terjadi kesalahan pada server.

---

## Analisis JSON

| Field | Tipe Data | Keterangan |
|---------|---------|---------|
| id | Integer | ID transaksi |
| transactionId | String | ID transaksi unik |
| orderId | String | ID pesanan |
| method | String | Metode pembayaran |
| amount | Number | Nominal transaksi |
| status | String | Status pembayaran |
| paidAt | Null/String | Waktu pembayaran |
| channel | String | Jalur pembayaran |

JSON dipilih karena ringan, mudah dibaca manusia, dan didukung hampir semua bahasa pemrograman.
