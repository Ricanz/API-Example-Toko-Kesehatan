## Get Order Resep - Get Info

## Method POST
### Request
```json
{
    "data":{
        "kodeprovider" : "212",
        "kode_branch": "1",
        "nomor_registrasi": "MED-001"
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
        "nomor_registrasi": "TRX-001",
        "detail": [
            {
                "kode_obat": "OB-001",
                "nama_obat": "Paracetamol",
                "satuan_kecil": 2,
                "jumlah": 4,
                "satuan": "tablet", // tablet,  botol, strip dan lain lain
                "signa": "1x1 sehari sesudah makan",
                "harga_obat": 10000,
                "racikan": "y" //  y untuk iya, n untuk tidak
            }
        ]
    }
}
```

## Notes
- Digunakan untuk menampilkan list data `Obat` yang sudah diregistrasikan di Healthical
- Kode provider dan kode branch di tampilkan dalam request
- API akann diimplementasikan di CMS
- API dbutuhkan hanya untuk Get data ke CMS