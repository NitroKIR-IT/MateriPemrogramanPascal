# Materi Minggu 2
## Perkenalan Pascal
### Apa itu Pascal?
Pascal adalah sebuah bahasa pemrograman, sama seperti bahasa pemrograman lain seperti C, C++, Java, dan lain-lain.
### Mengapa Pascal?
Pascal dipilih untuk pembelajaran awal karena Pascal lebih mudah dibaca, dan lebih mendekati bahasa manusia, tidak seperti C/C++.
### Bagaimana cara mendownload bahasa Pascal?
Kita akan menggunakan Free Pascal, yang dapat didownload [di sini](http://www.freepascal.org/download.var)
## Struktur Program
### Bagaimanakah struktur dasar sebuah program Pascal?
Sebuah program Pascal sederhana dapat dilihat sebagai berikut
```
begin
    writeln('Hello World');
end.
```
Kata kunci `begin` adalah cara untuk memulai barisan program Pascal.
Setelah kata `begin` berisi kode program kita. Setelah itu, diakhir dengan kata kunci `end.` (dengan titik, mirip bahasa manusia)

## Variabel
### Bagaimana cara mendeklarasikan variabel di Pascal?
Dalam suatu program, ada yang bernama variabel, seperti variabel dalam matematika, variabel ini dapat diisi oleh data.
Untuk mendeklarasikan variabel, kita aka modifikasi kode kita tadi menjadi seperti ini:

```
var
a: integer;

begin
    writeln('Hello World');
end.
```
Di bagian paling atas program, sebelum `begin`, kita mulai dengan kata kunci `var`. Setelah itu kita definisikan namanya (misalnya `a`), kemudian `:` (titik dua), kemudian tipe data 
(akan dijelaskan lebih lanjut di materi selanjutnya), dan pada akhirnya `;` (titik koma).

## Operasi input/output
### Bagaimana menerima data dan mengeluarkan data?
Pascal sudah menyediakan caranya, yaitu dengan writeln, readln, write, dan read.
### writeln
Writeln berfungsi mengeluarkan output, setelah itu berpindah ke baris baru (seperti menekan ENTER)
Contoh kode program dengan writeln:
```
begin
    writeln('Hello World');
end.
```
Output program:
```
Hello World
```

### write
write berfungsi mengeluarkan output, tanpa berpindah ke baris baru
Contoh kode program dengan write:
```
begin
    writeln('Hello world');
    write('Hello');
    writeln('World');
end.
```
Output program:
```
Hello world
HelloWorld
```

### readln
readln berfungsi menerima input, setelah penekanan ENTER.
Contoh kode program dengan readln:
```
var
a: integer;

begin
    readln(a);
    writeln(a);
end.
```
Input: `16`
Output: `16`

### read
read berfungsi untuk menerima input.
Contoh kode program dengan read:
```
var a: integer;

begin
    read(a);
    writeln(a);
end.
```

Input: `156`
Output: `156`

## Operasi aritmatika berbasis angka integer
Operasi aritmatika Pascal sebagai berikut:
* +: tambah
* -: kurang
* \*: kali
* /: bagi
