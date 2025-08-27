## Post Batal Obat -  Pembatalan di CMS dan Otomatis

## Method POST
### Request
```json
{
    "data":{
        "kodeprovider" : "212",
        "kode_branch": "1",
        "order_id": "MED-001",
        "alasan": "Batal membeli obat"
    }
}
```

### Response
```json
{
    "code": 200,
    "status": "Ok",
    "pesan": "Berhasil"
}
```

## Notes
- Digunakan untuk melakukan pembatalan registrasi atau transaksi obat ke Healthical
- Kode provider dan kode branch di tampilkan dalam request
- API akan diimplementasikan di CMS
- API dbutuhkan hanya untuk Post data ke Healthical
- Pembatalan Obat disinkronkan stoknya ke Healthical