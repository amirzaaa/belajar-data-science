# Belajar List, Tuple, dan Set

Pada bagian awal mata kuliah Data Science, mahasiswa wajib untuk mengetahui fundamental dari list, tuple, dan juga Set agar dapat memahami bagaimana cara menyimpan serta mengelola kumpulan data dalam bahasa Pemrograman Python. Berikut adalah penjelasannya:

## Apa itu List, Tuple, dan Set?

### List

<img width="476" height="295" alt="image" src="https://github.com/user-attachments/assets/df63000a-1e7e-4217-b033-921709d38112" />


Anggap saja kamu memiliki suatu tas ransel yang tentunya dapat kamu tambahkan barang-barang kedalamnya, menghapus atau mengeluarkan barang dari keranjang tersebut, bahkan kamu juga dapat menukar posisi barang yang ada di dalam tas tersebut. Seperti itulah kira-kira perumpaan yang tepat untuk menggambarkan suatu list. berikut ini adalah karakteristik yang dimiliki oleh list:

- Dapat Diubah (Mutable)
  
  Elemen-elemn yang ada di dalam list tersebut dapat ditambah, dihapus, bahkan setelah list itu telah dibuat.

- Terurut (Ordered)

  Memiliki urutan elemen yang tetap, kecuali urutan tersebut diubah.
  
- Dapat diduplikasi

  Dapat berisi elemen yang sama (lebih dari satu elemen yang sama).
  
### Tuple

<img width="440" height="300" alt="image" src="https://github.com/user-attachments/assets/9f31020f-aabb-4370-ba95-74b0d4507b05" />

Bayangkan kamu memiliki kotak yang sudah tersegel. Setelah kotak itu ditutup dengan rapat, kamu tidak bisa lagi menambah, menghapus, atau mengubah elemen yang ada di dalamnya. Seperti itulah sedikit perumpaan tentang Tuples. Berikut ini adalah karakteristik yang dimiliki oleh Tuples.

- Tidak dapat diubah (Immutable)

  Elemen-elemen yang ada di dalam tuples tersebut tidak dapat ditambah, dihapus, ataupun diubah isinya.
  
- Berurutan (Ordered)

  Memiliki urutan elemen yang tetap dan berurut
  
- Dapat diduplikasi

  Dapat berisi elemen yang sama (lebih dari satu elemen yang sama).

### Set

<img width="400" height="320" alt="image" src="https://github.com/user-attachments/assets/90382d0b-429b-449d-a90c-fe6e1dcd31a6" />

Bayangin saja kamu mempunyai suatu keranjang buah, yang di dalamnya kamu dapat menambahkan buah, mengganti buah yang ada di dalamnya, serta kamu juga dapat mengeluarkan buah yang ada di keranjang buah tersebut. Namun, kamu hanya dapat menambahkan buah yang unik pada keranjang buah tersebut (tidak boleh ada buah yang sama), dan di dalam keranjang tersebut tidak memperdulikan tentang urutan. Begitulah perumpamaan yang cocok untuk menggambarkan Sets yang ada di bahasa pemrograman Python. Berikut ini adalah karakteristik yang dimiliki oleh Sets:

- Dapat diubah (Mutable)

  Elemen-elemen yang ada di dalam sets tersebut tidak dapat ditambah, dihapus, ataupun diubah isinya.

- Tidak berurutan (Unordered)

  Tidak mementingkan urutan dari elemen yang ada di dalamnya

- Tidak dapat di duplikasi

  Elemen-elemen yang ada di dalam sets harus unique

Setelah mengetahui definisi dan karakteristik dari list, tuple dan set, step berikutnya yang perlu untuk dipelajari adalah bagaimana cara penanganan list, tuple, dan set dengan menggunakan bahasa pemrograman Python. berikut adalah pembahasan lebih lengkapnya.

## Bagaimana cara penanganan List, Tuple, dan Set?

### List

Ketika ingin menggunakan list pada bahasa pemrograman Python, kita dapat menggunakan simbol `[]` untuk membungkus elemen-elemen yang ada di dalamnya, atau kita juga dapat memnbuat suatu list dengan membuat tuple terlebih dahulu kemudian kita ubah tuple tersebut menjadi sebuah list. berikut adalah contoh penggunaannya:

```
# Contoh penggunaan menggunakan simbol []
buah = ["apel", "jeruk", "alpukat"]

# Contoh penggunaan list dengan tuple
sayur = ('bayam','kubis','wortel')
mySayur = list(sayur)

# Mengakses elemen berdasarkan indeks
print(buah[2])
print(mySayur[0])

print(buah)
print(mySayur)
```

berikut adalah output dari kode tersebut:

<img width="1151" height="301" alt="image" src="https://github.com/user-attachments/assets/68d02e7c-1241-4d4d-8eaa-476d6cf259ee" />

Setelah mengetahui cara penggunaan dari list, berikut adalah contoh penanganan (method) yang dapat digunakan pada list.

| **Metode**      | **Deskripsi**                                                                                  | **Contoh**                      |
|-----------------|-----------------------------------------------------------------------------------------------|---------------------------------|
| `append()`      | Menambahkan item ke **akhir** list.                                                           | `buah.append("apel")`       |
| `insert()`      | Menambahkan item pada **indeks tertentu**.                                                    | `buah.insert(1, "anggur")`     |
| `extend()`      | Menambahkan semua elemen dari iterable lain (seperti list lain) ke akhir list saat ini.       | `buah.extend(["kiwi", "melon"])` |
| `remove()`      | Menghapus kemunculan **pertama** dari item berdasarkan **nilainya**.                          | `buah.remove("pisang")`       |
| `pop()`         | Menghapus dan mengembalikan item pada indeks tertentu. Jika indeks tidak diberikan, akan menghapus dan mengembalikan item terakhir. | `buah.pop(1)`                 |
| `del`   | Menghapus item pada indeks tertentu atau menghapus seluruh list.                              | `del buah[0]`                 |
| `clear()`       | Mengosongkan list dari semua item.                                                            | `buah.clear()`                |
| `sort()`        | Mengurutkan list dalam urutan **menaik** secara default.                                      | `buah.sort()`                 |
| `reverse()`     | Membalik urutan item dalam list.                                                              | `buah.reverse()`              |

### Tuple

Dalam menggunakan tuple pada bahasa pemrograman Python, kita dapat menggunakan simbol `()` untuk membungkus elemen-elemen yang ada di dalamnya, atau kita juga dapat memnbuatnya tanpa menggunakan simbol tersebut. berikut adalah contoh penggunaannya:

```
# Contoh penggunaan dengan simbol ()
warna = ("abu-abu", "biru", "hijau")

# Contoh penggunaan tanpa simbol ()
numbers = 1,2,3,4,5,2,3,2

# Cara mengakses elemen tuple
print(warna[0])
print(warna2[1])

print(warna)
print(warna2)
```

Berikut adalah output dari kode tersebut.

<img width="1145" height="307" alt="image" src="https://github.com/user-attachments/assets/b9d6fd51-0370-4038-b729-1c681ca26841" />


Karena tuples memiliki karakteristik immutable, penanganan atau built-in methods yang dimiliki oleh tuples hanya terdapat 2 methods. berikut adalah contoh penggunaannya.

| **Metode** | **Deskripsi**                                                                                  | **Contoh**                            |
|---------------------|-----------------------------------------------------------------------------------------------|---------------------------------------|
| `count()`           | Menghitung jumlah kemunculan suatu nilai di dalam tuple.                                      | `numbers.count(2)`                    |
| `index()`           | Mengembalikan indeks dari kemunculan pertama suatu nilai di dalam tuple.                      | `numbers.index(3)`                    |

Berikut adalah contoh output dari penggunaan metode tersebut.

<img width="1131" height="169" alt="image" src="https://github.com/user-attachments/assets/20c17170-c392-47d2-94cd-b72000cefd0f" />

### Set

Untuk menggunakan set pada bahasa pemrograman Python, kita dapat menginisiasinya dengan simbol `{}` untuk membungkus elemen-elemen yang ada di dalamnya. Berikut adalah contoh penggunaannya.

```
numbers = {1,2,3,4,5}
numbers2 = {5,6,7,8,9}

print(numbers)
print(numbers2)
```

berikut adalah output dari kode diatas.

<img width="1173" height="249" alt="image" src="https://github.com/user-attachments/assets/d3dde043-7d8f-493f-a005-cd0d78d350e8" />

Setelah mengetahui cara penggunaan dari sets, berikut adalah contoh penanganan (method) yang dapat digunakan pada sets.

| **Metode** | **Deskripsi**                                                                                  | **Contoh**                      |
|---------------------|-----------------------------------------------------------------------------------------------|---------------------------------|
| `add()`            | Menambahkan satu elemen ke dalam set.                                                          | `fruits.add("melon")`          |
| `update()`         | Menambahkan banyak elemen dari iterable lain (seperti list atau set lain) ke dalam set.        | `fruits.update(["kiwi", "nanas"])` |
| `remove()`         | Menghapus elemen tertentu dari set. Jika elemen tidak ada, akan menimbulkan error.             | `fruits.remove("apel")`        |
| `discard()`        | Menghapus elemen tertentu dari set. Jika elemen tidak ada, **tidak menimbulkan error**.        | `fruits.discard("apel")`       |
| `pop()`            | Menghapus dan mengembalikan elemen **acak** dari set.                                          | `fruits.pop()`                  |
| `clear()`          | Menghapus semua elemen dari set.                                                               | `fruits.clear()`                |
| `union()`   | Mengembalikan set baru yang merupakan gabungan dari dua set.                                   | `numbers.union(numbers2)` |
| `intersection()` (`&`) | Mengembalikan set baru berisi elemen yang ada di **keduanya**.                              | `numbers.intersection(numbers2)` |
| `difference()` (`-`) | Mengembalikan set baru berisi elemen yang ada di set pertama tetapi tidak di set kedua.      | `numbers.difference(numbers2)` |
| `symmetric_difference()` (`^`) | Mengembalikan set baru berisi elemen yang ada di salah satu set, tetapi tidak di keduanya. | `numbers.symmetric_difference(numbers2)` |
| `issubset()`       | Mengecek apakah semua elemen set saat ini ada di dalam set lain.                               | `numbers.issubset(numbers2)`           |
| `issuperset()`     | Mengecek apakah set saat ini berisi semua elemen set lain.                                     | `numbers.issuperset(numbers2)`         |
| `isdisjoint()`     | Mengecek apakah dua set **tidak memiliki elemen yang sama**.                                   | `numbers.isdisjoint(numbers2)`         |
| `len()`            | Menghitung jumlah elemen dalam set.                                                            | `len(fruits)`                   |
| (`in`) | Mengecek apakah suatu nilai ada di dalam set.                                                  | `"apel" in fruits`             |

Setelah mengetahui seluruh penanganan dari list, tuple, dan set, sebagai mahasiswa yang sedang belajar Data science, kita perlu untuk mengetahui apa perbedaan dari ketiga jenis struktur data tersebut agar kita tidak bingung ketka ingin menggunakannya.

## Apa perbedaan dari List, Tuple, dan Set?

Perbedaan utama list, tuple, dan set terletak pada kemampuan untuk diubah (mutabilitas), urutan elemen, dan keunikan elemen. List bersifat mutable, terurut, dan mengizinkan duplikat. Tuple bersifat immutable (tidak bisa diubah), terurut, dan mengizinkan duplikat. Sedangkan set bersifat mutable, tidak terurut, dan hanya menyimpan elemen unik.
