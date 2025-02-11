# Bare Code 
Bare Coda adalah code minimal yang harus ada untuk menjalankan program dengan golang.
Pada Program minimum ini, setidaknya menjalankan fungsi main() yang menjadi titik awal eksekusi program

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

### Penjelasan
| Syntax | Penjelasan |
|----------|--------|
| package main |Setiap program eksekusi di Golang harus berada dalam paket main, jika tidak, maka program akan dikompilasi menjadi binary executable |
| import "fmt" | Package fmt  package bawaan (built-in) di Golang yang digunakan untuk format dan manipulasi teks, seperti mencetak output ke terminal atau membaca input dari pengguna |
| func main() | Fungsi main() adalah titik awal eksekusi program, Setiap program Go harus memiliki fungsi main(), kecuali jika program tersebut hanya berupa library.|
| fmt.Println("Hello, World!") | Mencetak "Hello, World!" di layar (console) |


### Variasi Bare Code Lain
Jika ingin program yang lebih minimal, kita bisa menghilangkan import package, Program ini akan tetap valid, namun tidak menjalankan apapun

```go
package main

func main() {}
```

### Fungsi Utama dalam fmt
Menampilkan Output ke Terminal (Console)
| Syntax | Penjelasan |
|----------|--------|
| fmt.Print() | Menampilkan teks tanpa newline. |
| fmt.Println() | Menampilkan teks dengan newline otomatis. |
| fmt.Printf() | Menampilkan teks dengan format tertentu. |

Membaca Input dari Pengguna
| Syntax | Penjelasan |
|----------|--------|
| fmt.Scan() |  Membaca input tanpa format khusus. |
| fmt.Scanln() | Membaca input sampai newline. |
| fmt.Scanf() | Membaca input dengan format tertentu. |

### Variasi penulsian package
- **Import dengan tanda kurung**
  ```go
import (
    "fmt"
    "math"
    "strings"
)
```
- [x] Digunakan ketika mengimpor lebih dari satu package.
- [x] Membantu meningkatkan keterbacaan kode.
✅ Lebih rapi dan direkomendasikan untuk proyek besar.


