# Materi Minggu 5
## Subprogram: Procedure dan Functiom
### Apa itu subprogram?
Subprogram itu adalah 'program dalam program', yaitu kode yang bisa kita jalankan dalam program kita
### Mengapa kita membutuhkan subprogram?
Saat program kita semakin panjang, akan semakin susah untuk dipahami. Karena itu, ada beberapa bagian program yang dipisahkan menjadi subprogram, terutama bagi yang sering dipakai 
berulang-ulang

### Subprogram procedure
Cara mendeklarasikan sebuah procedure adalah sebagai berikut
```
var a: integer;

procedure cot();
begin
     writeln('bagus');
end;

begin
    cot();
end.
```
Sebuah procedure harus dideklarasikan sebelum kode utama program.
Dalam hal ini, procedure `cot` akan mengeluarkan kata 'bagus'.

### Parameter
Subprogram kita juga dapat menerima nilai, yang disebut dengan parameter.
Contoh procedure dengan parameter
```
procedure cot(x: integer);
begin
    writeln('cot',x);
end;
```
Cara pemanggilan procedure ini adalah sebagai berikut:
```
begin
    cot(5);
end.
```
Program ini akan menghasilkan output `cot5`, yaitu kata `cot` ditambah dengan isi variabel x, yaitu 5 (dari pemanggilan function).

### Variabel subprogram
Didalam subprogram juga dapat mendeklarasikan variabel. Contoh:
```
procedure cotwithvar();
var
    bau: integer;
begin
    bau := 16;
    writeln(bau);
end;
```
Pemanggilan procedure:
```
begin
cotwithvar();
end.
```
Program ini akan mengeluarkan angka 16.

### Ruang lingkup parameter.
Jika ada nama variabel yang sama dari parameter dan variabel utama program, maka variabel yang diakses dalam subprogram adalah variabel parameter. Begitu juga dengan variabel 
subprogram dan variabel program utama, maka yang diakses adalah variabel subprogram.

Contoh:
```
var x,y: integer;

procedure tukar(x,y: integer);
begin
    x := x+y
    y := x-y
    x := x-y
end;

begin
    x := 7;
    y := 15;
    tukar(x,y);
    writeln(x,' ',y);
end;
```
Saat program ini dijalankan, procedure tukar yang dipanggil tidak menukar kedua variabel yang kita assign tadi. Ini karena saat procedure tukar dipanggil, yang diakses sebenarnya
variabel parameter pada subprogram.

### Perbedaan function dengan procedure
Ada lagi satu cara untuk mendeklarasikan subprogram, yaitu function. Berbeda dengan procedure, function harus mengembalikan suatu nilai, tidak seperti procedure yang bisa hanya 
dipanggil saja.

### Pendeklarasian function
Contoh untuk mendeklarasikan function adalah sebagai berikut:
```
function jumlah(x,y: integer) : integer;
begin
    jumlah := x + y;
end;
```
Perbedaan utama adalah, pertama, adalagi tanda titik dua (:) dan nama tipe setelah penulisan function. Ini mendapatkan tipe data yang dikeluarkan oleh function. Kedua, pemanggilan 
terakhir function harusnya assignment ke nama function.

Pemanggilan function:
```
begin
    writeln(jumlah(5,6));
end.
```
Tidak seperti procedure, function yang mempunyai nilai bisa dimasukkan ke function lain, perintah writeln/write, masuk dalam rangkaian operasi biner, dan perbandingan.

## Manipulasi String
### Bagaimana cara memanipulasi string?
Pascal menyediakan berbagai fungsi yang membantu kita dalam memanipulasi string, yaitu:
#### length(S)
Mengembalikan panjang string S.
Contoh pemanggilan
```
writeln(length('cot'));
```
akan mengeluarkan `3` (panjang dari string 'cot')
#### pos(T,S)
Mengembalikan posisi substring T dalam string S.
Mengembalikan 0 jika tidak ditemukan substring T.
Contoh pemanggilan
```
writeln(pos('cot','bacot');
```
akan mengeluarkan angka `3` (posisi dari string 'cot' dalam 'bacot').
#### copy(S, pos, cnt)
Mengembalikan potongan string S yang dimulai dari posisi pos sepanjang cnt karakter.
Contoh pemanggilan
```
writeln(copy('fumiomurakami',5,3);
```
akan menngeluarkan string `omu`

#### delete(S,pos,cnt)
Adalah prosedur yang akan menghapus bagian dari string S dimulai dari posisi pos sepanjang cnt karakter.
Contoh kode:
```
var s: string;

begin
    s := 'ketikatitusmenagihuangkas';
    delete(s,7,6);
    writeln(s);
end.
```
Program akan mengeluarkan string `ketikaenagihuangkas`.

#### insert(T,S,pos);
Adalah prosedur yang akan memasukan string T di string S pada posisi pos.
Contoh kode:
```
var s: string;
begin
    s := 'ketikamenagihuangkas';
    insert('titus',s,7);
    writeln(s);
end.
```
Program akan mengeluarkan string `ketikatitusmenagihuangkas` saat dijalankan.

