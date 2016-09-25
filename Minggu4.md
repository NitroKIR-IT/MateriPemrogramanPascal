# Materi Minggu 4
## Assignment
### Bagaimana cara melakukan assignment?
Cara melakukan assignment cukup gampang. Contoh kode assignment adalah sebagai berikut
```
var
a: integer;

begin
    a := 5;
    writeln(a);
end.
```

Cara melakukan assignment adalah, pertama menuliskan nama variabel, kemudian tanda := (titik dua + sama dengan), kemudian nilai yang akan dimasukkan ke dalam variabel (dapat berupa 
variabel juga).

### Mengapa assignment tidak menggunakan '=' ?
Tanda sama dengan saja (=) dalam Pascal adalah operasi perbandigan Tanda titik dua dan sama dengan (:=) adalah assignment variabel.

## Perulangan: for
### Bagaimana cara melakukan perulangan dengan for
Cara melakukan perulangan dengan for adalah sebagai berikut:
```
for i := awal to akhir do
begin

end;
```
'i' merupakan sebuah variabel, awal berisi nilai awal i dan dan akhir berisi nilai akhir dari i.
Cara kerjanya, pertama i diset ke nilai awal, kemudian kode yang dalam begin ... end; dijalankan, kemudian i ditambah dengan satu, kemudian kode dijalankan lagi, seterusnya sampai i 
mencapai nilai akhir. Dengan kata lain, i merupakan variabel yang berfungsi sebagai counter.

### Menggunakan variabel counter dalam kode.
Anda juga bisa menggunakan variabel counter di dalam kode yang diulang-ulang tersebut. Contoh kodenya:
```
var i: integer;

begin
    for i := 1 to 10 do
    begin
        writeln('cot',i);
    end;
end.
```

## Perulangan: while
### Apa perbedaan for dan while?
Walau for dan while sama-sama digunakan untuk perulangan, namun penggunaannya berbeda.
Perulangan for digunakan untuk mengulang kode dari nilai counter awal sampai akhir
Perulangan while, artinya kode dijalankan terus selama suatu kondisi terpenuhi.


### Bagaimana cara menggunakan perulangan while?
Cara dasar untuk perulangan while adalah sebagai berikut
```
while kondisi do
begin

end;
```
Kondisi bisa berupa variabel boolean, atau operasi yang menghasilkan boolean (operasi biner dan operasi perbandingan)

Contoh:

```
var
i: integer;

begin
    while i < 6 do
    begin
        writeln('cot',i);
        i := i + 1;
    end;
end.
```
