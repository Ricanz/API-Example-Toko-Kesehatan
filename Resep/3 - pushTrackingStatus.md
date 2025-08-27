## Push Tracking Status - Notification

## Method POST
### Request
```json
{
    "nomor_registrasi": "REG-001",
    "nomor_transaksi": "TRX-001",
    "no_rm": "00072363",
    "status": "pending_payment",
    // prepared => Obat Disiapkan
    // refused => Obat Dibatalkan
    // pending_payment => Transaksi Menunggu Pembayaran
    // settlement => Transaksi Telah Dibayar
    // cancel => Transaksi Dibatalkan
    "deskripsi": "Transaksi Menunggu Pembayaran"
}
```

### Response
```json
{
    "code": 200,
    "status": "Ok",
    "pesan": "Berhasil",
    "data": null
}
```

## Notes
- Digunakaan untuk melakukan push data dari Healthical ke  Mobile pasien
