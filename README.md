# Praktikum-2 | Struktur Kondisi 

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

```Python
else:
    print("Tidak perlu ikut asuransi")
    if punya_rumah:
        print("Wajib bayar pajak rumah")
```
Jika kurang dari 3.000.000, akan mencetak "Tidak perlu ikut asuransi"

`if punya_rumah` kalau true akan mencetak "Wajib bayar pajak rumah"

## Pengunaan `if`, `else`, dan `elif` untuk nilai
```Python
if akhir > 80:
    huruf = "A"
elif akhir > 70:
    huruf = "B"
elif akhir > 50:
    huruf = "C"
elif akhir > 40:
    huruf = "D"
else:
    huruf = "E"
```

## Penggunaan kondisi `OR`
```Python
if a + b == c or b + c == a or c + a == b:
```

## Penggunaan `if`, `else` dan `elif` untuk tiket bioskop
```Python
if tipe_tiket == "reguler":
    harga_tiket = harga_reguler
elif tipe_tiket == "vip":
    harga_tiket = harga_vip
else:
    print("Tipe tiket tidak valid!")
    exit()
```

```Python
if status_member == "Y":
   diskon = 0.20 * harga_tiket
   harga_akhir = harga_tiket - diskon
   print(f"Anda mendapatkan diskon 20%! Potongan harga: Rp{diskon:.2f}")
else:
   harga_akhir = harga_tiket
```

## Penggunaan `if`, `elif`, dan `else`
```Python
if operator == '+':
    hasil = angka1 + angka2
    print(f"Hasil: {angka1} + {angka2} = {hasil}")
```

```Python
elif operator == '-':
    hasil = angka1 - angka2
    print(f"Hasil: {angka1} - {angka2} = {hasil}")
elif operator == '*':
    hasil = angka1 * angka2
    print(f"Hasil: {angka1} * {angka2} = {hasil}")
```

```Python
elif operator == '/':
    if angka2 != 0:
        hasil = angka1 / angka2
        print(f"Hasil: {angka1} / {angka2} = {hasil}")
    else:
        print("Error: Pembagian dengan nol tidak diperbolehkan!")
```

```Python
else:
    print("Operator tidak valid! Silakan masukkan +, -, *, atau /.")
```
