# Praktikum-2 | Struktur Kondisi 

Nama : Tiara Hayatul Khoir

Kelas : TI.24.A.5

NIM : 312410474

Mata Kuliah : Bahasa Pemrograman

## Penggunaan stuktur kondisi menggunakan statement `if`, `else` dan `elif` dalam Python
Dalam Python, `if` dan `else` digunakan untuk melakukan pengambilan keputusan berdasarkan kondisi tertentu. Program akan menjalankan blok kode dalam `if` jika kondisi tersebut bernilai True. Namun, jika kondisinya False, program akan menjalankan blok kode yang terdapat dalam `else`. Selanjutnya `elif` adalah singkatan dari "else if". Ini digunakan untuk memeriksa kondisi tambahan jika kondisi sebelumnya `if` atau `elif` bernilai False. Dengan elif, kita dapat mengevaluasi beberapa kondisi secara berurutan.

## Penggunaan `if`, `else`, dan `elif` Untuk Nilai
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
`if`: Mengecek apakah nilai akhir lebih dari 80.

Jika True, variabel huruf diisi dengan "A", dan program tidak memeriksa kondisi lainnya (blok selesai di sini).

`elif`: (else if) Memeriksa kondisi tambahan jika kondisi pertama (nilai akhir > 80) False.

Jika akhir > 70: Huruf diisi "B". Jika akhir > 50: Huruf diisi "C". Jika akhir > 40: Huruf diisi "D".

`else`: Menangani semua kondisi lainnya (yaitu jika nilai akhir ≤ 40). Dalam kasus ini, huruf diisi dengan "E".

![foto](https://github.com/tir890/foto/blob/755cb9a2f8fc7f875fefd558d47e191951a9f12a/Blank%20diagram%20(2).png)

## Hasil Kode program

![foto](https://github.com/tir890/foto/blob/5ebac34cd25748e5017f89f183641b77a495e9be/nilai.png)

## Penggunaan `elif` Untuk Gaji Karyawan
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

`if punya_rumah` jika true akan mencetak "Wajib bayar pajak rumah"

![foto](https://github.com/tir890/foto/blob/040510722a9232213763c1e3934d2732c1ad44f1/Blank%20diagram%20(1).png)

## Hasil Kode Program
![foto](https://github.com/tir890/foto/blob/2c337f093c7404f272af9a1533ba70f7b817c777/gaji%20karyawan.png)

## Penggunaan Kondisi `OR`
```Python
if a + b == c or b + c == a or c + a == b:
```
Pada baris ini, program memeriksa beberapa kondisi menggunakan operator logika `or`. Operator `or` digunakan untuk menggabungkan beberapa kondisi. Jika salah satu dari kondisi yang digabungkan dengan `or` adalah `True`, maka seluruh pernyataan akan dianggap `True`.

![foto](https://github.com/tir890/foto/blob/0d2b351c77b752f25056d4c8fd906d8cf0a9b4c4/Blank%20diagram%20(3).png)

## Hasil Kode Program
![foto](https://github.com/tir890/foto/blob/0d2b351c77b752f25056d4c8fd906d8cf0a9b4c4/Screenshot%202024-10-30%20231511.png)

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
Kondisi `if` Memeriksa apakah variabel `tipe_tiket` sama dengan "reguler". Jika kondisi ini benar (True), maka nilai `harga_tiket` diatur ke `harga_reguler`.

Kondisi `elif` Jika kondisi sebelumnya tidak terpenuhi (tipe_tiket bukan "reguler"), program akan memeriksa apakah `tipe_tiket` sama dengan "vip". Jika benar, maka `harga_tiket` diatur ke harga_vip.

Kondisi `else` Jika kedua kondisi di atas tidak terpenuhi (artinya `tipe_tiket tidak valid`), program mencetak pesan "Tipe tiket tidak valid!" dan kemudian menghentikan eksekusi program dengan `exit()`.

```Python
if status_member == "Y":
   diskon = 0.20 * harga_tiket
   harga_akhir = harga_tiket - diskon
   print(f"Anda mendapatkan diskon 20%! Potongan harga: Rp{diskon:.2f}")
else:
   harga_akhir = harga_tiket
```
Kondisi `if` Memeriksa apakah `status_member` sama dengan "Y" (yang mungkin berarti pengguna adalah anggota).

Jika benar, maka:

Diskon dihitung sebagai 20% dari `harga_tiket`. `harga_akhir` dihitung dengan mengurangi `diskon` dari `harga_tiket`. Program mencetak pesan yang menyatakan bahwa pengguna mendapatkan diskon, termasuk jumlah potongan harga dalam format yang diinginkan.

Kondisi else:

Jika pengguna bukan anggota (status_member bukan "Y"), maka `harga_akhir` diatur sama dengan `harga_tiket` tanpa diskon.

![foto](https://github.com/tir890/foto/blob/be4012cea396c69e55735abd5bc14c64875fdbf4/Blank%20diagram%20(4).png)

## Hasil Kode Program

![foto](https://github.com/tir890/foto/blob/be4012cea396c69e55735abd5bc14c64875fdbf4/Screenshot%202024-10-30%20235607.png)

## Penggunaan `if`, `elif`, dan `else`
```Python
if operator == '+':
    hasil = angka1 + angka2
    print(f"Hasil: {angka1} + {angka2} = {hasil}")
```
Memeriksa apakah operator yang dimasukkan adalah `+`. Jika benar, maka kode menghitung jumlah `angka1` dan `angka2`, lalu mencetak hasilnya.

```Python
elif operator == '-':
    hasil = angka1 - angka2
    print(f"Hasil: {angka1} - {angka2} = {hasil}")
elif operator == '*':
    hasil = angka1 * angka2
    print(f"Hasil: {angka1} * {angka2} = {hasil}")
```
`elif` digunakan untuk memeriksa kondisi berikutnya, yaitu jika operator adalah `-` atau `*`. Setiap blok `elif` melakukan operasi yang sesuai (pengurangan atau perkalian) dan mencetak hasilnya.


```Python
elif operator == '/':
    if angka2 != 0:
        hasil = angka1 / angka2
        print(f"Hasil: {angka1} / {angka2} = {hasil}")
    else:
        print("Error: Pembagian dengan nol tidak diperbolehkan!")
```
Memeriksa apakah operator adalah `/`. Sebelum melakukan pembagian, kode memeriksa apakah `angka2` tidak sama dengan 0. Jika `angka2` tidak sama dengan 0, maka pembagian dilakukan dan hasilnya dicetak. Jika `angka2` sama dengan 0, kode mencetak pesan kesalahan karena pembagian dengan nol tidak diperbolehkan.

```Python
else:
    print("Operator tidak valid! Silakan masukkan +, -, *, atau /.")
```
Jika semua kondisi sebelumnya tidak terpenuhi (misalnya, pengguna memasukkan operator yang tidak valid), maka blok `else` dieksekusi.

Program akan mencetak pesan bahwa operator tidak valid dan meminta pengguna untuk memasukkan operator yang benar.

![foto](https://github.com/tir890/foto/blob/1720ed118f2b1f579cab7b0a6b756c7b45733848/Blank%20diagram%20(5).png)

## Hasil Kode Program

![foto](https://github.com/tir890/foto/blob/1720ed118f2b1f579cab7b0a6b756c7b45733848/Screenshot%202024-10-31%20001903.png)
