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

### 🔹 **Latihan 3: Nullable & Null Safety**

Tuliskan program yang menerima nama user, tapi bisa juga null.

```kotlin
fun main() {
    var nama: String? = null
    println("Panjang nama: ${nama?.length ?: "Nama tidak tersedia"}")
}
```

---

### 🔹 **Mini Project: Kalkulator Sederhana**

Input: dua angka dan operator (`+`, `-`, `*`, `/`)
Output: hasil perhitungan

```kotlin
fun kalkulator(a: Double, b: Double, op: Char): Double {
    return when (op) {
        '+' -> a + b
        '-' -> a - b
        '*' -> a * b
        '/' -> if (b != 0.0) a / b else Double.NaN
        else -> Double.NaN
    }
}

fun main() {
    println(kalkulator(10.0, 2.0, '*')) // Output: 20.0
}
```

---
