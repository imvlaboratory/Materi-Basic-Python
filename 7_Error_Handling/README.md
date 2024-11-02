# Error Handling

Merupakan salah satu teknik dalam pemrograman yang digunakan untuk mengatasi potensi kesalahan yang mungkin terjadi selama eksekusi program. Dalam Python, penanganan kesalahan dilakukan menggunakan blo `try`, `except`, `else`, dan `finally`.

## Try dan Except

- **Try Block**

Digunakan untuk menempatkan kode yang mungkin menyebabkan eror.

- **Except Block**

Digunakan untuk menangkap dan menangani eror yang muncul di dalam blok `try`.

```
try:
    # Kode yang mungkin menyebabkan error
    result = 10 / 0
except ZeroDivisionError:
    # Menangani error jika terjadi ZeroDivisionError
    print("Tidak bisa membagi dengan nol.")
```

## Else

- **Finally**

Dapat digunakan untuk menempatkan kode yang harus dijalankan, baik eror atau tidak. Blok ini akan berjalan selalu, bahkan jika ada atau tidak ada eror.

```
try:
  result = 10 / 2
except ZeroDivisionError:
  print("Tidak bisa membagi dengan nol.")
else:
  print("Hasil:", result)
finally:
  print("Eksekusi blok finally.")
```

## Menangkap Beberapa Jenis Error

- Kita dapat menangani beberapa jenis eror dengan menambahkan beberapa blok `except`.

```
try:
    result = 10 / 'a'
except ZeroDivisionError:
    print("Tidak bisa membagi dengan nol.")
except TypeError:
    print("Tipe data tidak sesuai.")
```

## Penggunaan `as` untuk Informasi Error.

- Kita dapat menggunakan `as` untuk memberikan nama pada variabel yang menyimpan informasi eror.

```
try:
    result = 10 / 'a'
except (ZeroDivisionError, TypeError) as err:
    print(f"Terjadi kesalahan: {err}")
```

## Raise

- Dapat digunakan untuk memicu eror secara manual. Kita dapat memasukkan tipe eror atau membuat eror khusus.

```
try:
    raise ValueError("Ini adalah error custom.")
except ValueError as err:
    print(f"Terjadi kesalahan: {err}")
```

Dengan konsep-konsep Error Handling di atas, kita dapat membuat program Python lebih tahan kesalahan dan memberikan pesan yang jelas saat terjadi kesalahan. Ini membantu dalam pemeliharaan dan debugging kode
