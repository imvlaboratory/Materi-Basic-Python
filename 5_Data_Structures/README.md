# Data Structure

Struktur data dalam Python adalah cara penyusunan dan penyimpanan data agar dapat diakses dan dikeloa dengan efisien. Python menyediakan berbagai jenis tipe data dan struktur data bawaan seperti lists, tuple, sets, dictionaries, strings, queues, stacks, linked lists, dan lainnya. Bebrapa diantaranya sudah dibahas pada section Data Types.

Data struktur memungkinkan pengorganisasian data dengan cara tertentu agar dapat diakses atau dimanipulasi sesuai dengan kebutuhan aplikasi atau algoritma. Struktur data yang baik dapat memudahkan pengembangan, pemeliharaan, dan pemahaman kode program.

Pada Section ini akan dijelaskan bagaimana cara pengoprasian dan manipulasi tipe data kompleks yang ada pada Python.

## Indexing dan Slicing

### Indexing

- **Definisi** indexing merujuk pada proses mengakses element di dalam struktur data seperti tuple, list, atau string dengan menggunakan indeks.

- **Indeksing Dimulai dari 0**

Sama seperti beberapa bahasa pemrograman lain, dalam Python juga indeksing dimulai dari 0, element kedua memiliki indeks 1, dan seterusnya.

**Contoh Indexing pada List**

```
my_list = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

print(my_list[0]) # Output: 1
print(my_list[5]) # Output: 6
print(my_list[-2]) # Output 9 (Indeks negatif mengakses elemen dari belakang)
```

**contoh Indeksing pada String**

```
my_string = "Hello, World!"

print(my_string[0])  # Output: 'H'
print(my_string[7])  # Output: 'W'
```

### Slicing

- **Slicing** adalah proses mengambil sebagian dari struktur data dengan menyertakan batas awal dan akhir.

**Contoh Slicing pada List**

```
my_list = [10, 20, 30, 40, 50]

print(my_list[1:4])  # Output: [20, 30, 40] (indeks 1 hingga 3, indeks 4 tidak termasuk)
print(my_list[:3])   # Output: [10, 20, 30] (indeks awal tidak ditentukan, dimulai dari awal)
print(my_list[2:])   # Output: [30, 40, 50] (indeks akhir tidak ditentukan, berakhir di akhir)
```

**Contoh Slicing pada String**

```
my_string = "Hello, World!"

print(my_string[7:12])  # Output: 'World' (indeks 7 hingga 11)
print(my_string[:5])    # Output: 'Hello' (indeks awal tidak ditentukan, dimulai dari awal)
print(my_string[7:])    # Output: 'World!' (indeks akhir tidak ditentukan, berakhir di akhir)
```

**Contoh Slicing dengan Langkah pada List**

Pada Slicing kita juga dapat menggunakan langkah (step) untuk mengambil elemen yang diinginkan engan interval tertentu.

```
my_list = [10, 20, 30, 40, 50, 60, 70, 80, 90]

print(my_list[1:8:2])  # Output: [20, 40, 60, 80] (indeks 1 hingga 7, langkah 2)
```

- Saat melakukan indexing atau slicing, pastikan indeks yang digunakan berada dalam batas valid untuk menghindari indexError.

- Slicing menghasilkan salinan dari struktur data baru, sehingga perubahan pada hasil slicing tidak mempengaruhi struktur data asli.

Indexing dan Slicing adalah teknik dasar yang sangat penting dalam pemrograman Python, memungkinkan anda untuk mengakses dan memanipulasi data secara efisien dalam berbagai jenis struktur.

## List Comprehensions

List comprehensions adalah konstruksi sintaksis yang kuat dalam Python yang memungkinkan kita membuat list dengan kode yang lebih singkat dan ekspresif. Mereka memberikan cara ringkas untuk membuat list dengan memanfaatkan loop dan ekspresi kondisional.

### Sintaks Umum

```
new_list = [expression for item in iterable if condition]
```

**Komponen Utama**

- **Expression** Ekspresi yang mendefinisikan nilai untuk setiap elemen dalam list.

- **Item** Variabel yang mewakili setiap elemen dalam iterabel (misal list, tuple, atau string)

- **Iterabel** Struktur data yag dapat di iterasi (list, tuple, string, dll)

- **Condition (Optional)** kondisi opsional yang memfilter elemen yang akan dimasukkan kedalam list.

**Contoh List Comprehesions**

1. **Membuat Angka Kuadrat**

```
squares = [x**2 for x in range(5)]
# Output: [0, 1, 4, 9, 16]
```

2. **Membuat List Hanya Bilangan Ganjil**

```
odd_numbers = [x for x in range(10) if x % 2 != 0]
# Output: [1, 3, 5, 7, 9]
```

3. **Membuat List yang Menggandakan Setiap Karakter dalam String**

```
word = "hello"
doubled_characters = [char*2 for char in word]
# Output: ['hh', 'ee', 'll', 'll', 'oo']
```

4. **Membuat List yang Menggabungkan Elemen 2 List**

```
list1 = [1, 2, 3]
list2 = ['a', 'b', 'c']
combined_list = [(x, y) for x in list1 for y in list2]
# Output: [(1, 'a'), (1, 'b'), (1, 'c'), (2, 'a'), (2, 'b'), (2, 'c'), (3, 'a'), (3, 'b'), (3, 'c')]
```

**Keuntungan List Comprehession**

- **Kode lebih singkat**
- **Kode lebih cepat** Dapat lebih efisien dari pada loop tradisional
- **Ekspresif** menyederhanakan logika pembuatan list.

**Penting**

- Gunakan list Comprehession dengan bijak agar kode tetap mudah dibaca
- Jangan terlalu komplek untuk menjaga kejelasan kode.
