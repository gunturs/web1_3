# STRUKTUR KENDALI (Decision)
Struktur Kendali merupakan sebuah program yang digunakan untuk memilih kondisi tertentu berdasarkan pilihan kondisi yang tersedia. Berikut syntax yang dapat digunakan dalam membuat Struktur Kendali yang kadang disebut Decision:
1. if....else
2. Switch... case

## If..
if terdiri atas beberapa bentuk pengunaan yaitu:
1. if tunggal

if yang memiliki kondisi tidak lebih dari dua pilihan sehingga hanya menggunakan hanya satu if, perhatikan contoh berikut yang menguji nilai mahasiswa.

```php
<?
$nilai=70;
if(nilai>=65)
{
  echo "Lulus";
}
else
{
  echo " Gagal";
}
?>
```
> Keterangan:
dalam program diatas terdapat 2 kondisi nilai lebih besar sama dengan 60 dan nilai lebih kecil 60 yang akan menghasilkan pilihan jawaban lulus atau gagal, $nilai merupakan variabel yang diuji

2. if majemuk

if yang memiliki kondisi lebih dari dua pilihan sehingga hanya menggunakan lebih dari satu if dengan ketentuan n-1, perhatikan contoh berikut yang menguji nilai mahasiswa.

perhatikan contoh pengujian nilai yusidium mahasiswa berikut

```php
<?php
$nilai=80;
if($nilai>=80)
{
  $yudisium="A";
}
elseif($nilai>=70)
{
   $yudisium="B";
}
elseif($nilai>=60)
{
   $yudisium="C";
}
elseif($nilai>=50)
{
   $yudisium="D";
}
else
{
   $yudisium="E";
}
echo "Nilai Yudisium= $yudisium";
?>
```
> **keterangan:** pada contoh program diatas terdapat 5 kondisi nilai sehingga if yang dipakai sebanyak 4

## Swicth

Perhatikan contoh berikut
```php
<?php
$nilai = 80;

switch ($nilai) {
  case $nilai>=80:
    $yudisium="A";
    break;
  case $nilai>=70:
    $yudisium="B";
    break;
  case $nilai>=60:
    $yudisium="C";
    break;
  case $nilai>=50:
    $yudisium="D";
    break;
default:
    $yudisium="E";
}
echo "Nilai Yusidium=". $yudisium;
?> 
```
> #Contoh lain

```php
<form action="?" method="post">
 <input type="text" name="tnilai">
 <input type="submit" value="Proses">
 </form>
 <?php
$nilai = $_POST['tnilai'];
else
{ $nilai=0;}
switch ($nilai) {
  case $nilai>=80:
    $yudisium="A";
    break;
  case $nilai>=70:
    $yudisium="B";
    break;
  case $nilai>=60:
    $yudisium="C";
    break;
  case $nilai>=50:
    $yudisium="D";
    break;
default:
    $yudisium="E";
}
echo "Nilai Yusidium=". $yudisium;
?> 
```


