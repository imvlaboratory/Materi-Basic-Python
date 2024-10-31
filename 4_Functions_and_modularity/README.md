# Functional and Modularity

Dalam Python, fungsi adalah blok kode yang dapat dipanggil untuk menjalankan tugas tertentu, membantu mengorganisir logika program menjadi unit yang dapat digunakan kembali. Fungsi menerima input, melakukan operasi, dan mengembalikan output. Sementara itu, modularitas merujuk pada praktik membagi program menjadi modul-modul terpisah. Modul adalah file Python yang berisi definisi variabel , fungsi, dan kelas. Dengan fungsi, kita dapat mengelompokkan kode dengan logika serupa, sementara modularitas memungkinkan pemisahan program kedalam bagian yang lebih kecil, meningkatkan kejelasan, pemeliharaan, dan penggunaan kembali kode. Kombinasi fungsi dan modularitas memperkuat struktur dan pemahaman program, memfasilitasi pengembangan dan pemeliharaan yang lebih efisien.

## Higher Order Functions

Dalam Python, fungsi adalah blok kode yang dapat dipanggil secara berulang untuk melakukan tugas tertentu. Fungsi hanya dapat berjalan ketika dipanggil, dan fungsi juga biasanya menerima input (parameter), melakukan operasi tertentu, dan mengembalikan output.

Contoh fungsi sederhana :

```
def my_function():
    print("Hello from a function")

# Memanggil Fungsi
my_function()
```

### Parameter dan Return Value

Fungsi dapat menerima parameter sebagai input untuk melakukan operasi tertentu. Return Statement digunakan untuk mengembalikan nilai dari fungsi. Sebuah fungsi dapat memiliki atau tidak parameter, dan dapat atau tidak mengembalikan suatu nilai.

Contoh fungsi dengan parameter dan return values :

```
def tambah(x, y):
    """Fungsi Penjumlahan"""
    result = x + y
    return result

# Memanggil fungsi dan menyimpan hasilnya
sum_result = add(5,10)
print("Hasil sama dengan : ", sum_result)
```

Variabel yag terdapat pada fungsi hanya dapat digunakan dalam fungsi tersebut, bila ingin digunakan diluar fungsi tersebut maka variabel harus dideklarasikan kedalam variabel global.

## Lambda Functions

Fungsi lambda merupakan fungsi anonim pada python. Fungsi ini biasanya digunakan untuk tugas-tugas yang sangat sederhana dan pendek. Misalnya, fungsi yang hanya dibutuhkan sekali atau perhitungan sederhana.

Struktur umum fungsi Lambda :

```
lambda argumen: ekspresi
```

**Argumen** merupakan input yang kita berikan ke fungsi lambda, dan **ekspresi** adalah operator atau rumus atau kalkulasi yang ingin kita lakukan dengan argumen tersebut. Hasil dari **ekspresi** akan menjadi output fungsi.

Contoh :

```
tambah = lambda a, b: a + b
print(tambah(4,5)) #Output 9
```

**Penjelasan kode diatas**

- `tambah` Adalah variabel yang menyimpan fungsi lambda.
- Fungsi lambda menerima 2 argumen (`x` dan `y`) dan mengembalikan hasil penjumlahan mereka (`x + y`).
- Ketika kita memanggil `tambah (4, 5)`, fungsi ini akan mengembalikan 7.

## Modularity

Modularity atau modularitas adlaah konsep dalam pemrograman yang merujuk pada pemisahan program kedalam bagian-bagian yang lebih kecil yang disebut modul. Modul adalah file Python yang berisi definsi variabel, fungsi, dan kelas yang dapat digunakan oleh program lain. Prinsip modulasi memberikan keuntungan dalam pemeliharaan, pengembangan, dan kejelasan kode.
