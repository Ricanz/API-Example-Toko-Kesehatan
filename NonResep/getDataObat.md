## Get Data Obat

## Method POST
### Request
```json
{
    "data":{
        "kodeprovider" : "212",
        "kode_branch": "1"
    }
}
```

### Response
```json
{
    "code": 200,
    "status": "Ok",
    "pesan": "Berhasil",
    "response": [
        {
            "kode_obat": "OB-001",
            "harga_satuan_kecil": 5000,
            "stok_satuan_kecil": 10,
            "satuan": "botol"
        },
        {
            "kode_obat": "OB-002",
            "harga_satuan_kecil": 3000,
            "stok_satuan_kecil": 5,
            "satuan": "tablet"
        },
        {
            "kode_obat": "OB-003",
            "harga_satuan_kecil": 3500,
            "stok_satuan_kecil": 8,
            "satuan": "tablet"
        },
    ]
}
```

## Notes
- Digunakan untuk menampilkan daftar obat yang ada di apotek berdasarkan kode provider dan kode branch
- Kode provider dan kode branch di tampilkan dalam request
- API akann diimplementasikan di Mobile
- `Harga Satuan Kecil` diambil dari grup tarif standar