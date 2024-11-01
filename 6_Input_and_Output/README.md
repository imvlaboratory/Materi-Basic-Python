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
# parse input ke tipe data
tinggi = float(input("Masukan tinggi badan anda: "))
print(f'tinggi badan anda adalah {tinggi} cm')
```

## Membaca dan Menulis File

### Membaca File

- jika
