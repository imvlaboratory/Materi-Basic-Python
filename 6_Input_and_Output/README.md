# Input/Output

I/O pada Python merujuk pada proses masukan dan keluaran dalam programm. Hal ini melibatkan interksi antara program dan lingkungannya (terminal, akses file).

## Standar Input dan Output

### Standar Input

- `input()` digunakan untuk membaca suatu input dari pengguna (keyboard).
- Mengembalikan string yang di input oleh pengguna.

### Standar Output

- `print()` digunakan untuk menampilkan Output ke layar.
- Dapat mencetak nilai variabel atau teks.

**Contoh**

```
name = input("Masukkan nama Anda: ")
print("Hello, " + name + "!")
```

**Contoh untuk Tipe Data lain**

```
# parse input ke tipe data string
umur = int(input("Masukan umur anda"))
print(f'umur anda adalah {umur}')


tinggi = float(input("Masukan tinggi badan anda: "))
print(f'tinggi badan anda adalah {tinggi} cm')
```

## Membaca dan Menulis File

### Membaca File

- Fungsi `open()` digunakan untuk membuka file. Dapat menerima dua argumen : nama file dan mode (`r` untuk membaca, `w` untuk menulis, `a` untuk menambahkan, dan sebagainya).

* Metode `read()` digunakan untuk membaca isi file

**Contoh**

```
with open('file.txt', 'r') as file:
    content = file.read()
    print(content)
```

### Menulis File

- Jika file belum ada, fungsi `open()` dengan mode `w` akan membuat file baru. Jika sudah ada, akan menghapus kontennya dan menulis yang baru.
- Metode `write()` digunakan untuk menulis ke file.

**Contoh**

```
with open('file.txt', 'w') as file:
    file.write("Ini adalah contoh tulisan ke file.")
```

### Iterasi baris dalam File

- Kalian dapat menggunakan perulangan untuk membaca setiap baris dalam file.

```
with open('file.txt', 'r') as file:
    for line in file:
        print(line)
```

### Membaca, Menulis, dan Memanipulasi File Data Menggunakan Pandas

Pandas adalah salah satu pustaka Python yang sangat populer untuk analisis data, dan menyediakan fungsi untuk membaca dan menulis data dari dan ke berbagai format file, termasuk CSV (Comma-Separated Values). Berikut adalah cara membaca dan menulis file dari dan ke DataFrame Pandas ke file CSV :

**Membaca file ke DataFrame**

```
import pandas as pd

# Membaca file CSV ke DataFrame
df = pd.read_csv('nama_file.csv')

# Menampilkan beberapa baris pertama dari DataFrame
print(df.head())
```

Pada contoh diatas, `pd.read_csv('nama_file.csv')` digunakan untuk membaca data dari file CSV ke dalam sebuah DataFrame. Fungsi `head()` kemudian digunakan untuk menampilkan beberapa baris pertama dari DataFrame tersebut.

**Menulis DataFrame ke File**

```
import pandas as pd

# Membuat DataFrame contoh
data = {'Nama': ['John', 'Alice', 'Bob'],
        'Usia': [28, 24, 22],
        'Kota': ['Jakarta', 'New York', 'London']}

df = pd.DataFrame(data)

# Menulis DataFrame ke file CSV
df.to_csv('output_file.csv', index=False)
```

Pada contoh ini, `pd.DataFrame(data)` digunakan untuk membuat DataFrame dari data yang diberikan. Kemudian, `df.to_csv('output_file.csv', index=False)` digunakan untuk menulis DataFrame ke dalam file CSV baru dengan nama `output_file.csv`. Argumen `index = False`menunjukkan bahwa kita tidak ingin menyimpan indeks baris dalam file CSV.

Dengan menggunakan Pandas, kita dapat dengan mudah membaca dan menulis data dari dan ke file CSV, serta berbagai format file lainnya. Ini sangat berguna ketika kita bekerja dengan dataset dalam bentuk DataFrame dan ingin menyimpannya atau memuatnya dari file CSV untuk analisis lebih lanjut.
