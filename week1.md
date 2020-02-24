# Week 1 (Dasar Pemrograman Python)
Minggu ke 1 belajar berkenaan dengan dasar pemrograman Python. Silahkan lanjutkan ke Week 2 bila merasa sudah menguasainya.

## 1. Variabel dan Tipe Data
Variabel adalah sebuah lokasi di memori dimana seorang Programmer dapat menyimpan sebuah nilai. Dalam Python deklarasi variabel tidak dilakukan secara eksplisit. Penggunaan variabel digambarkan seperti contoh kode 1.1 misalnya untuk menghitung BMI (*Body Mass Index*) yang rumusnya :
![BMI=\frac{weight}{height^{2}}](https://render.githubusercontent.com/render/math?math=BMI%3D%5Cfrac%7Bweight%7D%7Bheight%5E%7B2%7D%7D)
#### Contoh Kode 1.1
```python
height = 1.79
weight = 68.7

bmi = weight / height ** 2
print(bmi)
```
Seperti di bahasa pemrograman lain, Python juga memiliki aturan penamaan variabel seperti berikut :
  * Harus dimulai dengan huruf (a – z, A – Z) atau *underscore*. Karakter selanjutnya bisa berupa huruf atau angka atau *underscore*.
  * *Case sensitive*
  * Tidak boleh menggunakan kata-kata yang sudah dimiliki oleh Python, karena Python menggunakannya untuk hal yang lainnya.
  * Panjang variabel bisa berapa pun.
  
Dalam membuat nama sebuah variabel,  pilihlah yang memiliki makna. Hindari menggunakan singkatan karena bila bekerja dengan tim, anggota lain akan kebingungan membaca kode. Konsisten dalam penamaan apakah menggunakan gaya [Camel](https://en.wikipedia.org/wiki/Camel_case) atau [Snake](https://en.wikipedia.org/wiki/Snake_case). Pada kasus-kasus yang khusus gunakan *underscore* diawal nama variabel.\
Python memiliki beberapa tipe data yaitu :
<table>
<thead>
<tr>
<th>NO</th>
<th>NAMA TIPE</th>
<th>KETERANGAN</th>

</tr>
</thead>
<tbody>
<tr>
<td>1</td>
<td>float</td>
<td>Bilangan Real</td>
</tr>
<tr>
<td>2</td>
<td>int</td>
<td>Bilangan Bulat</td>
</tr>
<tr>
<td>3</td>
<td>str</td>
<td>string, text</td>
</tr>
<tr>
<td>4</td>
<td>bool</td>
<td>true atau false</td>
</tr>
</tbody>
</table>
