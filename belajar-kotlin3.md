### 🔹 **Latihan 1: Fungsi dan Percabangan**

Buat fungsi `cekNilai(nilai: Int): String` yang mengembalikan kategori nilai:

* `>= 90` → "A"
* `80 - 89` → "B"
* `70 - 79` → "C"
* `< 70` → "D"

```kotlin
fun cekNilai(nilai: Int): String {
    return when {
        nilai >= 90 -> "A"
        nilai in 80..89 -> "B"
        nilai in 70..79 -> "C"
        else -> "D"
    }
}

fun main() {
    println(cekNilai(85)) // Output: B
}
```

---

### 🔹 **Latihan 2: Class & Object**

Buat class `Mahasiswa` dengan properti `nama`, `nim`, dan method `perkenalan()`.

```kotlin
class Mahasiswa(val nama: String, val nim: String) {
    fun perkenalan() {
        println("Halo, saya $nama dengan NIM $nim")
    }
}

fun main() {
    val mhs = Mahasiswa("Rani", "2212001")
    mhs.perkenalan()
}
```

---
