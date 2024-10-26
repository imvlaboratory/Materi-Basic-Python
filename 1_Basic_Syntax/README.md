# BASIC SYNTAX

Python merupakan bahasa pemrograman yang memiliki syntaks yang relatif sederhana dan mudah untuk dipelajari. Maka dari itu, berikut merupakan beberapa sytaks dasar Python :

## Comment

Comment merupakan sebuah catatan yang dapat dimasukkan kedalam kode untuk menjelaskan apa yang dilakukan oleh kode tersebut. Comment diawali dengan tanda Pound(#).

```
# Ini komen pada baris pertama
# ini komen pada baris kedua

""
Ini adalah multi-line comment atau bisa disebut juga docs string

dengan cara ini dapat membuat suatu dokumentasi.
untuk pembahasan lebih lanjut akan dijelaskan pada (type data string)
""
```

## Identasi

Merupakan suatu cara untuk menandai blok kode. Tidak seperti bahasa lain yang biasanya menggunkan kurung kurawal `{}` . Python menggunakan **identasi**(pergeseran baris kode kekanan) untuk menunjukkan hierarki atau struktur kode. Identasi standar di Python adalah 2 atau 4 spasi.

contoh :

```
a = "variable dalam outer scope"
print(a) # kode akan tereksekusi tanpa error, karna variable a dalam jangkauan

    b = "variable dalam inner scope"
    print(a) # kode akan tereksekusi tanpa error, karena variable a masih bisa dijangkau walaupun berada di scope luar
    print(b) # kode akan tereksekusi tanpa error, karena variable b dalam jangkauan

print(b) # kode error, variable a tidak terbaca karena ada pada block scope berbeda, dan outer scope tidak bisa membaca variable yang terdefinisi di inner scope

if True:
    print("Ini adalah bagian dari blok 'if'.")
print("Ini di luar blok 'if'.")
```

## Variabel
