### 1. **Pengenalan Kotlin**

* Kotlin adalah bahasa pemrograman modern yang dikembangkan oleh JetBrains.
* Bisa digunakan untuk Android, backend (JVM), desktop, bahkan web.
* Sintaks lebih ringkas dari Java, dan interoperable dengan Java.

### 2. **Dasar-Dasar Kotlin**

* **Hello World**:

  ```kotlin
  fun main() {
      println("Hello, Kotlin!")
  }
  ```

* **Variabel**:

  ```kotlin
  var nama = "Budi"      // bisa diubah
  val umur = 22          // tidak bisa diubah (immutable)
  ```

* **Tipe Data**: `Int`, `Double`, `Boolean`, `String`, `Char`

### 3. **Kontrol Alur**

* **If-Else**:

  ```kotlin
  if (umur > 18) {
      println("Dewasa")
  } else {
      println("Anak-anak")
  }
  ```

* **When (seperti switch)**:

  ```kotlin
  when (nilai) {
      10 -> println("Sempurna")
      in 7..9 -> println("Bagus")
      else -> println("Perlu belajar lagi")
  }
  ```

* **For loop**:

  ```kotlin
  for (i in 1..5) {
      println(i)
  }
  ```

* **While loop**:

  ```kotlin
  var x = 1
  while (x <= 5) {
      println(x)
      x++
  }
  ```

### 4. **Fungsi**

```kotlin
fun salam(nama: String): String {
    return "Halo, $nama!"
}
```

### 5. **Nullable dan Null Safety**

```kotlin
var nama: String? = null
println(nama?.length) // safe call
```

### 6. **Object-Oriented Programming (OOP)**

* **Class & Object**:

  ```kotlin
  class Mahasiswa(val nama: String, val nim: String)

  val mhs = Mahasiswa("Ani", "123")
  println(mhs.nama)
  ```

* **Inheritance**:

  ```kotlin
  open class Hewan
  class Kucing : Hewan()
  ```

* **Interface**:

  ```kotlin
  interface Terbang {
      fun terbang()
  }

  class Burung : Terbang {
      override fun terbang() {
          println("Burung terbang")
      }
  }
  ```

### 7. **Collection**

* **List, Set, Map**:

  ```kotlin
  val angka = listOf(1, 2, 3)
  val data = mapOf("nama" to "Budi", "umur" to 22)
  ```

* **Mutable**:

  ```kotlin
  val mutable = mutableListOf("A", "B")
  mutable.add("C")
  ```

### 8. **Extension Function**

```kotlin
fun String.terbalik(): String {
    return this.reversed()
}
println("Kotlin".terbalik()) // niltoK
```
