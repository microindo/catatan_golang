# Bare Code 
Bare Coda adalah code minimal yang harus ada untuk menjalankan program dengan golang.
Pada Program minimum ini, setidaknya menjalankan fungsi main() yang menjadi titik awal eksekusi program

``go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
``

## Penjelasan
| Syntax | Penjelasan |
|----------|--------|
| package main |Setiap program eksekusi di Golang harus berada dalam paket main, jika tidak, maka program akan dikompilasi menjadi binary executable |
| import "fmt" | Package fmt digunakan untuk menampilkan output ke terminal (Console) |
| func main() | Fungsi main() adalah titik awal eksekusi program, Setiap program Go harus memiliki fungsi main(), kecuali jika program tersebut hanya berupa library.|
| fmt.Println("Hello, World!") | Mencetak "Hello, World!" di layar (console) |


