# Praktikum 2 - Struktur Kondisi 

Nama : Tiara Hayatul Khoir

Kelas : TI.24.A.5

NIM : 312410474

Mata Kuliah : Bahasa Pemrograman

## Penggunaan stuktur kondisi menggunakan statsment `if`, `else` dan `elif` dalam Python
Dalam Python, `if` dan `else` digunakan untuk melakukan pengambilan keputusan berdasarkan kondisi tertentu. Program akan menjalankan blok kode dalam `if` jika kondisi tersebut bernilai True. Namun, jika kondisinya False, program akan menjalankan blok kode yang terdapat dalam `else`. Selanjutnya `elif` adalah singkatan dari "else if". Ini digunakan untuk memeriksa kondisi tambahan jika kondisi sebelumnya `if` atau `elif` bernilai False. Dengan elif, kita dapat mengevaluasi beberapa kondisi secara berurutan.

## Penggunaan `elif` untuk gaji karyawan
```Python
if gaji > 3000000:
    print("Gaji sudah di atas UMR")
    if berkeluarga:
        print("Wajib ikut asuransi dan menabung untuk pensiun")
```
Program akan memeriksa apakah gaji lebih dari 3.000.000.

Jika benar, akan mencetak "Gaji sudah di atas UMR".

Kemudian, program memeriksa apakah sudah berkeluarga.

Jika benar, akan mencetak "Wajib ikut asuransi dan menabung untuk pensiun".

