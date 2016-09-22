# Materi Minggu 3
## Tipe Data
### Apa saja kah tipe data dalam Pascal
Pascal mempunyai beragam tipe data. Ini adalah daftar tipe data yang dapat dipakai dalam Pascal.
* integer: angka dari -2^15 sampai 2^15 -1
* longint: angka dari -2^32 sampai 2^32 -1
* int64: angka dari -2^64 sampai 2^64 -1
* char: berupa satu huruf
* string: berupa sebuah kata, panjang maks 255 byte
* float: angka berkoma, presisi single
* double: angka berkoma, presisi double
* real: angka berkoma
* boolean: berisi true atau false
## Percabangan: If
### If simple
If digunakan sebagai percabangan kode (jika begini maka begitu)
Kode If yang simple adalah sebagai berikut
```
if (boolean) then
begin
//kode program
end;
```
### If dan else
Kode dalam else akan dipanggil jika tidak ada kondisi yang memenuhi if sebelumnya.
Kode If yang menggunakan else adalah sebagai berikut:
```
if (boolean) then
begin
//kode program
end
else
begin
//kode jika tidak ada yang memenuhi
end;
```
### If bercabang banyak
setelah else juga bisa ditambahkan kata if, dengan cara seperti sebelumnya
Contoh kode if bercabang banyak:
```
if (boolean) then
begin
//kode program
end
else if (boolean) then
begin
//kode untuk kondisi kedua
end
else
begin
//kode jika tidak ada kondisi yang memenuhi
end;
```
kata boolean dapat diganti dengan variabel apapun yang bertipe boolean, atau operasi yang menghasilkan boolean, seperti operasi boolean dan operasi perbandingan
## Operasi boolean
Ada 4 operasi boolean yang sering dipakai, yaitu
### AND
| A | B | A AND B |
|---|---|---------|
| T | T | T       |
| T | F | F       |
| F | T | F       |
| F | F | F       |
### OR
| A | B | A OR B |
|---|---|--------|
| T | T | T      |
| T | F | T      |
| F | T | T      |
| F | F | F      |
### NOT
| A | NOT A |
|---|-------|
| T | F     |
| F | T     |
### XOR
| A | B | A XOR B |
|---|---|---------|
| T | T | F       |
| T | F | T       |
| F | T | T       |
| F | F | F       |
## Operasi perbandingan
Operasi perbandingan seperti pada matematika, yaitu < (kurang dari), >(lebih dari), = (sama dengan), != (tidak sama dengan), <= (kurang dari/sama dengan), >= (lebih dari/sama dengan)

