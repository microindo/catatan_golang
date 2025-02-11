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


# 📌 Tipe Data dalam Golang

## 📌 1. Tipe Data Numerik

| **Kategori** | **Tipe Data** | **Ukuran** | **Contoh Deklarasi** |
|-------------|--------------|------------|----------------------|
| **Bilangan Bulat (Integer)** | `int8`, `int16`, `int32`, `int64` | 8-bit hingga 64-bit | `var x int32 = 100` |
| | `int` | Sesuai arsitektur CPU | `x := 42` |
| **Bilangan Bulat Tanpa Tanda (Unsigned Integer)** | `uint8`, `uint16`, `uint32`, `uint64` | 8-bit hingga 64-bit | `var y uint16 = 500` |
| | `uint` | Sesuai arsitektur CPU | `var z uint = 25` |
| **Bilangan Desimal (Floating-Point)** | `float32`, `float64` | 32-bit, 64-bit | `var pi float64 = 3.14` |
| **Bilangan Kompleks** | `complex64`, `complex128` | 64-bit, 128-bit | `var c complex64 = complex(2, 3)` |

---

## 📌 2. Tipe Data Lainnya

| **Kategori** | **Tipe Data** | **Ukuran** | **Contoh Deklarasi** |
|-------------|--------------|------------|----------------------|
| **Boolean** | `bool` | 1-bit (true/false) | `var aktif bool = true` |
| **String** | `string` | Dinamis | `var nama string = "Ahmad"` |
| **Karakter (Unicode)** | `byte` (alias `uint8`), `rune` (alias `int32`) | 8-bit, 32-bit | `var huruf rune = 'A'` |
| **Array (Ukuran Tetap)** | `[N]T` | Sesuai tipe elemen | `var arr [3]int = [3]int{1, 2, 3}` |
| **Slice (Ukuran Dinamis)** | `[]T` | Dinamis | `var data = []int{1, 2, 3}` |
| **Map (Key-Value)** | `map[TKey]TValue` | Dinamis | `var m map[string]int = map[string]int{"Ahmad": 25}` |
| **Struct (Kumpulan Data)** | `struct` | Dinamis | `type Person struct {Name string; Age int}` |
| **Interface (Tipe Apa Saja)** | `interface{}` | Dinamis | `var obj interface{}` |

---

## 📌 3. Contoh Penggunaan

```go
package main

import "fmt"

func main() {
    var angka int = 10
    angkaDesimal := 3.14
    nama := "Ahmad"
    aktif := true

    fmt.Println("Angka:", angka)
    fmt.Println("Desimal:", angkaDesimal)
    fmt.Println("Nama:", nama)
    fmt.Println("Status:", aktif)
}
```

