## Get Order Request - Take Photo

## Method POST
### Request
```json
{
    "data":{
        "kodeprovider" : "212",
        "kode_branch": "1",
        "no_rm": "00072363"
    }
}
```

### Response
```json
{
    "code": 200,
    "status": "Ok",
    "pesan": "Berhasil",
    "response": {
        "nomor_registrasi": "MED-001"
    }
}
```

## Notes
- Digunakan untuk mengirimkan informasi ada registrasi obat ke Healthical
- Informasi yang dibutuhkan berupa `Notifikasi` di aplikassi Healthical
- Kode provider dan kode branch di tampilkan dalam request
- API akann diimplementasikan di Mobile
- API dbutuhkan hanya untuk Get data ke Mobile