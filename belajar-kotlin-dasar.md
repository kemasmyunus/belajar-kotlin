# Belajar Kotlin Dasar

## 1. Pendahuluan
Kotlin adalah bahasa pemrograman modern yang dikembangkan oleh JetBrains dan digunakan secara luas untuk pengembangan aplikasi Android serta aplikasi backend.

## 2. Struktur Dasar Program Kotlin
```kotlin
fun main() {
    println("Hello, Kotlin!")
}
```
- `fun main()` adalah fungsi utama dalam Kotlin.
- `println()` digunakan untuk mencetak output ke konsol.

## 3. Variabel dan Tipe Data
```kotlin
val nama: String = "John"
var umur: Int = 25
```
- `val` adalah variabel yang bersifat immutable (tidak bisa diubah).
- `var` adalah variabel yang bisa diubah nilainya.
- Kotlin memiliki tipe data seperti `Int`, `Double`, `Boolean`, `String`, dll.

## 4. Operasi Dasar
```kotlin
val a = 10
val b = 5
println(a + b) // Penjumlahan
println(a - b) // Pengurangan
println(a * b) // Perkalian
println(a / b) // Pembagian
println(a % b) // Modulus
```

## 5. Struktur Kontrol
### 5.1 Percabangan (if-else)
```kotlin
val nilai = 80
if (nilai >= 75) {
    println("Lulus")
} else {
    println("Tidak Lulus")
}
```

### 5.2 When (Mirip Switch di Java)
```kotlin
val angka = 2
when (angka) {
    1 -> println("Satu")
    2 -> println("Dua")
    3 -> println("Tiga")
    else -> println("Angka lain")
}
```

## 6. Perulangan
### 6.1 For Loop
```kotlin
for (i in 1..5) {
    println("Perulangan ke-$i")
}
```

### 6.2 While Loop
```kotlin
var i = 1
while (i <= 5) {
    println("Iterasi ke-$i")
    i++
}
```

## 7. Fungsi
```kotlin
fun tambah(a: Int, b: Int): Int {
    return a + b
}

fun main() {
    val hasil = tambah(3, 4)
    println("Hasil: $hasil")
}
```

## 8. Class dan Object
```kotlin
class Orang(val nama: String, var umur: Int) {
    fun perkenalan() {
        println("Halo, nama saya $nama dan saya berumur $umur tahun.")
    }
}

fun main() {
    val orang1 = Orang("Budi", 21)
    orang1.perkenalan()
}
```
