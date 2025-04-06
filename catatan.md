

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

## 5. Deklarasi dengan Tipe Data

Kotlin memiliki sistem tipe data yang kuat:
```kotlin
val umur: Int = 23
val tinggi: Double = 1.75
val aktif: Boolean = true
```

Tipe data umum:
- `Int`, `Double`, `Float`, `Boolean`, `Char`, `String`

Kotlin bisa menebak tipe data (type inference), jadi deklarasi seperti ini juga valid:
```kotlin
val nama = "Kema"
```

---

## 6. Bermain dengan String

```kotlin
val nama = "Kema"
val pesan = "Halo, saya $nama"
println(pesan)
```

Fitur:
- Interpolasi string dengan `$`
- Multiline string dengan `"""..."""`

```kotlin
val biodata = """
    Nama: Kema
    Umur: 23
""".trimIndent()
```

---

## 7. Bermain dengan Angka

Kotlin mendukung operasi matematika:
```kotlin
val a = 10
val b = 3

println(a + b) // 13
println(a - b) // 7
println(a * b) // 30
println(a / b) // 3
println(a % b) // 1
```

Untuk pembagian dengan hasil desimal, gunakan `toDouble()`:
```kotlin
println(a.toDouble() / b) // 3.333...
```

---

## 8. Mengconvert Tipe Data

Kotlin tidak mengkonversi tipe data otomatis. Harus dilakukan secara eksplisit:

```kotlin
val angkaStr = "123"
val angka = angkaStr.toInt()

val nilai = 99
val nilaiStr = nilai.toString()
```

Metode umum:
- `toInt()`, `toDouble()`, `toFloat()`, `toString()`, `toBoolean()`

---
