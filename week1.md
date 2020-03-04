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

Dalam membuat nama sebuah variabel,  pilihlah yang memiliki makna. Hindari menggunakan singkatan karena bila bekerja dengan tim, anggota lain akan kebingungan membaca kode. Konsisten dalam penamaan apakah menggunakan gaya [Camel](https://en.wikipedia.org/wiki/Camel_case) atau [Snake](https://en.wikipedia.org/wiki/Snake_case). Pada kasus-kasus yang khusus gunakan *underscore* diawal nama variabel.

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

## 2 String
Fungsi `print()` mencetak seluruh argumennya sebagai string, dipisahkan dengan spasi dan diikuti dengan sebuah line break (`\n`) seperti contoh kode 1.2.
#### Contoh Kode 1.2
```python
name = "Budi"

print("Hello World")
print("Hello", 'World')
print("Hello", name)
```

> Catatan: Fungsi untuk mencetak di Python 2.7 dan Python 3 berbeda. Di Python 2.7, tidak perlu menggunakan tanda kurung di sekitar argumennya (contoh: `print \"Hello World\"`).

Fungsi print() memiliki argumen opsional untuk mengontrol di mana dan bagaimana statemen yang diberikan akan dicetak. Di antaranya adalah:
- `sep`, yaitu pemisah antar kata (nilai *default*-nya adalah spasi)\n
- `end`, yaitu karakter yang akan ditambahkan di akhir statemen (nilai *default*-nya adalah `\\n` (karakter *newline*))

Contoh kode 1.3 menunjukan penggunaan parameter sep dan end.
#### Contoh Kode 1.3
```python
print("Hello", "World", sep="...", end="!!")
```

### 2.1 String


## 2. List (Himpunan)
Seorang *data scientist*, akan berhubungan dengan banyak poin data; sebagai contoh:data tinggi badan anggota dalam sebuah keluarga. Untuk menampung data tinggi anggota keluarga, Python menyediakan List atau himpunan seperti contoh kode 1.2.
#### Contoh Kode 1.2
```python
family = [1.73,1.68,1.71,1.89]	
print(family)
```
Nilai atau elemen dalam satu List bisa memiliki beberapa macam tipe data, seperti float, integer, boolean,  string; atau yang lebih lanjutnya bisa menyimpan List lain, seperti contoh Kode 1.3.
#### Contoh Kode 1.3
```python
family = ["Rizki",1.73, "Heni", 1.68, "Hafidz", 1.71, "Azzam", 1.89]
print(family)
```
Python juga mendukung Sub List yang merupakan sebuah elemen List di dalam List lain, ditulis dengan square brackets di ikuti dengan koma, bentuknya  seperti contoh kode 1.4 yang memiliki 4 Sub List.
#### Contoh Kode 1.4
```python
family = [
            ["Rizki",1.73], 
            ["Heni", 1.68], 
            ["Hafidz", 1.71], 
            ["Azzam", 1.89]
        ]
print(family)
```

Python menyediakan berbagai operasi untuk memanipulasi List seperti berikut ini :
### 2.1 Menambah Elemen Baru
Elemen baru dapat ditambahkan pada List dengan perintah bawaan Python yaitu `append()` atau `extends()`.  Contoh kode 1.5 terdapat tuple. Tuple mirip dengan List perbedaannya elemennya tidak bisa diubah.

#### Contoh Kode 1.5
```python
_list = []
print ("Initial blank list : ")
print (_list)
# Menambah elemen ke _list
_list.append(10.40)
_list.append(78.9)
_list.append(15)
_list.append("Toward to Data Science")
print ("_list setelah ditambah 4 elemen baru")
print (_list)
# Menambah elemen pada _list dengan pengulangan
for i in range(10,14):
    _list.append(i)
print ("_list setelah ditambah 4 elemen baru dengan pengulangan for")
print (_list)
# Menambah tuple pada _list
_list.append((99,100))
print ("_list setelah ditambah 1 elemen tuple baru")
print (_list)
```

Fungsi `extends()` menambah beberapa elemen sekaligus ke dalam List seperti contoh kode 1.6
#### Contoh Kode 1.6
```python
# Creating a List 
List = [1,2,3,4] 
print("Initial List: ") 
print(List) 
  
List.extend([8, 'Geeks', 'Always']) 
print("\nList after performing Extend Operation: ") 
print(List) 
```

### 2.2 Menyisipkan Elemen Baru
Fungsi `append()` menambahkan elemen di akhir List; sedangkan untuk menyisipkan di antaran elemen dalam List, menggunakan fungsi `insert()` seperti contoh kode 1.7.

#### Contoh Kode 1.7
```python
List = [1,2,3,4] 
print("Initial List: ") 
print(List) 
  
List.insert(3, 12) 
List.insert(0, 'Geeks') 
print("\nList after performing Insert Operation: ") 
print(List) 
```

### 2.3 Menghapus Elemen dari List
Elemen dapat dihapus dari List menggunakan fungsi `remove()`. Pesan error akan muncul, bila elemen tidak ada dalam himpunan. Fungsi `remove()` akan menghapus elemen satu per satu meskipun ada elemen yang sama dalam himpunan; bila ingin menghapus beberapa elemen sekaligus gunakan pengulangan seperti contoh kode 1.8

#### Contoh Kode 1.8
```python
  
# membuat himpunan 
List = [1, 2, 3, 4, 5, 6,  
        7, 8, 9, 10, 11, 12] 
print("Intial List: ") 
print(List) 
  
# Removing elements from List 
# using Remove() method 
List.remove(5) 
List.remove(6) 
print("\nList after Removal of two elements: ") 
print(List) 
  
# Removing elements from List 
# using iterator method 
for i in range(1, 5): 
    List.remove(i) 
print("\nList after Removing a range of elements: ") 
print(List) 
```
