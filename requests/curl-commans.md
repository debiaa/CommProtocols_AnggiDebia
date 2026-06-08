# CURL Commands Documentation

Repository ini menggunakan Postman sebagai tools utama pengujian REST API. Berikut adalah contoh implementasi request menggunakan CURL yang setara dengan request pada Postman.

## GET Daftar Transaksi

```bash
curl -X GET http://localhost:8088/api/transactions
```

Fungsi:
Mengambil seluruh data transaksi dari server.

## GET Detail Transaksi

```bash
curl -X GET http://localhost:8088/api/transactions/1
```

Fungsi:
Mengambil detail transaksi berdasarkan ID transaksi.

## POST Menambah Transaksi

```bash
curl -X POST http://localhost:8088/api/transactions \
-H "Content-Type: application/json" \
-d '{
  "orderId":"ORD001",
  "method":"QRIS",
  "amount":150000,
  "status":"PAID"
}'
```

Fungsi:
Menambahkan data transaksi baru ke server menggunakan format JSON.
