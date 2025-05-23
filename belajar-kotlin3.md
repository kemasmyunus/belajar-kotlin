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
