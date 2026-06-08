# CURL Commands

## GET Semua Transaksi

---

# 3. requests/postman-collection.json

Export collection Postman yang kamu gunakan:

1. Buka Postman
2. Klik Collection
3. Klik titik tiga (...)
4. Export
5. Pilih Collection v2.1
6. Simpan sebagai

```text
postman-collection.json
curl -X GET http://localhost:8088/api/transactions
curl -X GET http://localhost:8088/api/transactions/1
curl -X POST http://localhost:8088/api/transactions \
-H "Content-Type: application/json" \
-d '{
  "orderId":"ORD001",
  "method":"QRIS",
  "amount":150000,
  "status":"PAID"
}'
