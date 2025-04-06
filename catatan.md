

# 📘 Belajar Kotlin dari Dasar

Panduan belajar Kotlin ini cocok untuk pemula yang ingin mengenal dan menguasai dasar-dasar bahasa Kotlin. Kotlin banyak digunakan untuk pengembangan aplikasi Android, tapi juga bisa digunakan di sisi backend, web, bahkan multiplatform.

---

## 1. Intro Kotlin

Kotlin adalah bahasa pemrograman modern yang dikembangkan oleh JetBrains. Kotlin berjalan di atas JVM (Java Virtual Machine), sehingga bisa digunakan bersama Java atau menggantikan Java.

### Kelebihan Kotlin:
- Ringkas (concise)
- Aman dari null (`null safety`)
- Interoperable dengan Java
- Cocok untuk Android Development

---

## 2. Hello World di Kotlin

Contoh kode pertama:
```kotlin
fun main() {
    println("Hello, World!")
}
```

Penjelasan:
- `fun` digunakan untuk mendefinisikan fungsi.
- `main()` adalah titik awal program Kotlin dijalankan.
- `println()` mencetak teks ke console dan pindah baris.

---

## 3. Perbedaan `val` dan `var` di Kotlin

- `val` digunakan untuk nilai tetap (immutable), tidak bisa diubah setelah dideklarasi.
- `var` digunakan untuk nilai yang bisa berubah (mutable).

```kotlin
val nama = "Kema" // tidak bisa diubah
var umur = 23     // bisa diubah
umur = 24
```

Pemilihan `val` disarankan jika nilai tidak perlu diubah, untuk mencegah bug.

---

## 4. Aturan Memberi Nama Variabel

Saat membuat variabel di Kotlin:
- Gunakan huruf, angka, dan simbol `_`.
- Tidak boleh diawali dengan angka.
- Gunakan gaya penulisan `camelCase`.

Contoh nama variabel yang valid:
```kotlin
val namaLengkap = "Kema M. Yunus"
val umurSekarang = 23
```

---
