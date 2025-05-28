
# Percabangan dalam Kotlin

Percabangan digunakan untuk menjalankan kode tertentu berdasarkan kondisi yang diberikan. Dalam Kotlin, kita bisa menggunakan beberapa struktur kontrol:

## 1. `if`, `else if`, `else`

Struktur dasar:

```kotlin
val angka = 10

if (angka > 0) {
    println("Angka positif")
} else if (angka < 0) {
    println("Angka negatif")
} else {
    println("Angka nol")
}
```

### Kotlin mendukung `if` sebagai ekspresi:

```kotlin
val nilai = 85
val hasil = if (nilai >= 75) "Lulus" else "Tidak Lulus"
println(hasil)
```

---

## 2. `when`

Alternatif dari `switch` di bahasa lain. Lebih powerful dan fleksibel.

### Contoh dasar:

```kotlin
val hari = 3

when (hari) {
    1 -> println("Senin")
    2 -> println("Selasa")
    3 -> println("Rabu")
    4 -> println("Kamis")
    5 -> println("Jumat")
    6, 7 -> println("Akhir Pekan")
    else -> println("Hari tidak valid")
}
```

### `when` sebagai ekspresi:

```kotlin
val nilai = 90
val grade = when {
    nilai >= 90 -> "A"
    nilai >= 80 -> "B"
    nilai >= 70 -> "C"
    nilai >= 60 -> "D"
    else -> "E"
}
println("Grade: $grade")
```

---
