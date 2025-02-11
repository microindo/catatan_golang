# Deklarasi Variabel
Untuk mendeklarasikan variable digunakan beberapa model seperti tabel berikut
| Syntax | Penjelasan | Contoh |
|----------|--------|-----------|
| var nama string	| Bisa dideklarasikan tanpa nilai awal |	var umur int |
var nama = "Ahmad" |	Bisa tanpa tipe data eksplisit |	var umur = 25 |
nama := "Ahmad"	| Paling singkat, otomatis menentukan tipe data	| umur := 25 |
var (nama, umur = "Ahmad", 25)	| Bisa deklarasi banyak variabel sekaligus |	var (kota = "Lombok") |


# Deklarasi Konstanta
Constant/konstanta adalah jenis variabel yang nilainya tidak bisa diubah. Inisialisasi nilai hanya dilakukan sekali di awal, setelah itu variabel tidak bisa diubah nilainya.

```go
const judul = "Ini Judul"
```


