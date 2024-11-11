# Control Structure

Control Structure dalam Python merupakan suatu aliran eksekusi program dengan menggunakan blok kode tertentu. Struktur Kontrol digunakan untuk mengatur urutan eksekusi pernyataan dalam sebuah program. Berikut struktur kontrol yang terdapat pada Python :

## Conditional Statement

Struktur pernyataan kode yang digunakan untuk mengontrol atau menjalankan aliran kode berdasarkan kondisi tertentu. Pernyataan kondisional pada Python terdiri dari dua bagian utama, yakni :

- **Kondisi** adalah pernyataan yang digunakan untuk menentukan apakah blok kode akan dieksekusi atau tidak.
- **Blok Kode** adalah kumpulan kode atau pernyataan yang akan dieksekusi jika kondisi benar.

3 Jenis pernyataan kondisional pada Python, yaitu :

- **If Statement** Pernyataan kondisi yang paling dasar. Blok akan mengeksekusi jika kondisi If bernilai benar.
- **Elif Statement** Pernyataan kondisional yang akan digunakan atau dijalankan setelah if statement.
- **Else Statement** pernyataan kondisional yang digunakan untuk mengeksekusi blok kode jika kondisi dari if statement dan elif statement bernilai salah.

### If Statement

Digunakan untuk menjalankan kode jika kondisi bernilai benar.

```
a = 10

if a > 8:
    print("a Lebih besar dari 8")
```

### Elif Statement

Digunakan untuk menjalankan kode jika kondisi dari if bernilai salah.

```
a = 6

if a > 11:
    print("a Lebih besar dari 11")
elif a > 5:
    print("a lebih besar dari 5")
```

### Else Statement

Digunakan untuk mengeksekusi kode jika kondisi bernilai salah

```
a = 4

if a > 11:
    print("a Lebih besar dari 11")
elif a > 5:
    print("a lebih besar dari 5")
else:
    print("a lebih kecil dari 5")
```

Pernyataan kodisional dapat digunakan untuk berbagai jenis keperluan, diantaranya :

- Untuk membuat kode lebih efisien
- Untuk membuat kode lebih fleksibel
- Untuk membuat kode lebih mudah dibaca

Manfaat dari pernyataan kodisional :

- Dapat membantu programmer untuk menghindari penulisan kode yang berulang.
- Dapat membantu Programmer untuk membuat kode yang dapat disesuaikan dengan berbagai kondisi.
- Dapat memudahkan programmer untuk membaca dan memahami kode yang ada.

Pernyataan kondisional adalah salah satu fitur penting yang perlu dipahami oleh programmer.

## Loop Statement

Pernyataan perulangan dalam Python digunakan untuk mengeksekusi blok kode berulang kali selama kondisi terpenuhi atau bernilai benar. Dalam Python sendiri terdapat dua jenis pernyataan perulangan pada Python, yaitu :

- **For Loop** pernyataan perulangan yang akan mengeksekusi blok kode untuk element dalam kumpulan data.
- **While Loop** pernyataan perulangan yang akan mengeksekusi blok kode selama kondisinya bernilai benar.

### For loop

```
for i in range(10):
    print(f"aku perulangan ke-{i}")

buah = ["apel", "mangga", "Jeruk"]
for x in buah:
    print(x)

fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break

for x in "banana":
  print(x)
```

### While loop

```
a = 10
while a > 0:
    print(a)
    a -= 1
```

Pernyataan perulangan dapat digunakan untuk berbagai keperluan, antara lain :

- Untuk mengeksekusi kode berulang kali
- Untuk memproses kumpulan data
- Untuk membuat kode yang lebih efisien

Berikut adalah beberapa manfaat pernyataan perulang :

- Dapat membantu programmer untuk menghindari penulisan kode yang berulang-ulang.
- Dapat membantu programmer untuk memproses kumpulan data dengan lebih efisien.
- Dapat membantu programmer untuk membuat kode yang lebih mudah dibaca dan dipahami.

Pernyataan perulangan adalah salah satu fitur penting yang perlu dipahami oleh programmer Python. Pernyataan perulangan dapat digunakan untuk membuat kode python lebih efisien, fleksibel, dan mudah dibaca.
