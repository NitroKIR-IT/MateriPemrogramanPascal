# Materi tambahan Array
## Apa itu array?
Array adalah variabel dengan satu nama, tetapi mempunyai banyak nilai.
Nilai dalam array dilakukan dengan sebuah indeks.
## Bagaimana cara mendeklarasikan array?
Cara mendeklarasikan array dalam Pascal adalah sebagai berikut:
```
var
a: array[1..15] of integer;
```
Dengan catatan:
* a: nama variabel
* array[1..15]: menandakan panjang dari array dan indeks yang berlaku, contoh di sini indeks yang berlaku dari 1 sampai 15
* integer: menunjukan tipe.
## Akses ke dalam array
Untuk mengakses salah satu nilai pada array, kita juga melakukannya seperti variabel biasa, hanya saya kita memerlukan sebuah indeks.

Contoh penjumlahan: `writeln(a[5]+a[7]);`

Contoh assignment: `a[5] := 7;`

## Membaca beberapa nilai berurutan
Kita bisa menggunakan perulangan untuk membaca banyak nilai dan memasukkannya ke array.
Contoh kode:
```
var
a: integer;
b: array[1..15] of integer;

begin
   for i := 1 to 15 do
   begin
       readln(b[i]);
   end;
   for i := 1 to 15 do
   begin
       writeln(b[i]);
   end;
end.
```

