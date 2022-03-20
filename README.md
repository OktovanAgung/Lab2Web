| Nama  | Oktovan Agung Shailendra|
|-------|-------------------------|
|NIM    |312010131                |
| Kelas | TI.20.A.1               |


---
# Langkah - Langkah Praktikum
## 1. Membuat Dokumen HTML
Membuat dokumen HTML seperti berikut kemudian simpan dan lihat hasilnya di web browser.
![img](img/img1.png)

## 2. Mendeklarasikan CSS Internal
Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen, kemudian simpan dan lihat hasilnya pada web browser.
![img](img/img2.png)

## 3. Menambahkan Inline CSS
Kemudian tambahkan deklarasi CSS pada tag `<p>` seperti berikut. Seimpan kembali dan refresh web browser untuk melihat hasilnya.
![img](img/img3.png)

## 4. Menambahkan CSS Eksternal
Buatlah file baru dengan nama <b>style_eksternal.css<b> kemudianbuatlah deklarasi CSS seperti berikut.
![img](img/img4.png)
Kemudain tambahkan tag `<link>` untuk merujuk file css yang sudah dibuat pada bagiann `<head>`, kemudian simpan dan refresh padah web browser untuk melihat hasilnya.
![img](img/img5.png)

## 5. Menambahkan CSS Selector
selanjutnya menambahkan <b>CSS Selector<b> menggunakan ID dan Class Selector. Pada file <b>style_eksternal.css<b>, tambahkan kode berikut. Kemudian simpan kembali dan refresh web browser untuk melihat hasilnya.
![img](img/img6.png)

---

## Pertanyaan dan Tugas
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ( `<p id="paragraf-1" class="text-paragraf">` )

## Jawaban

1. Disini saya akan menambahkan dan mengubah properti dan nilaipada kode CSS, dimulai darimembuat kerangka HTML nya.
![img](img/img7.png)

Kemudian membuat CSS nya dengan menambahkan nilai dan properti pada kode diatas
Disini Saya menambahkan 4 selector kedalam CSS, diantaranya body, h2, .avatar, .header-profile. Masing - masing memiliki fungsi untuk mengatur tampilan pada HTML

Pada selector body saya menambahkan properti, yaitu width, font-size, color, width, DST.
Pada selector h2 saya menambahkan properti, yaitu font-width, fonth-size
Pada selector .avatar saya menambahkan properti, yaitu width, border-radius 
Pada selector .header-profile saya menambahkan properti, yaitu justify-content, align-items
![img](img/img8.png)

Pada hasil tersebut dapat dilihat, pada mode mobile lebar body terlalu ke tengah, karena widht pada selektor body diatur dengan nilai 50% pada ukuran desktop, agar dapat terlihat proporsional pada ukuran mobile dapat ditambahkan selektor @media only screen and (max-width: 760px), dan hasil nya bisa dilihat.
![img](img/img9.png)

2. Perbedaan antara element h1 {...} dengan #intro h1 {...} adalah :
h1 {...} Antuk memberikan style pada semua h1 sedangkan,
#intro h1 {...} Awalan simbol hash (#) memungkinkan kita untuk memberikan style pada id. selector id bersifat kaku dan tidak bisa digunakan kembali pada element yang lainnya. Menurut saya lebih baik menggunakan selektor class untuk mendefinisikan element yang ingin diberi nilai.
![img](img/img10.png)

3. Setelah dilakukan pengujian, deklarasi CSS Inline lebih dahulu tampil di browser, itu dikarenakan permintaan HTTP yang sangat kecil memungkinkan untuk ditampilkan dahulu

	Berikut merupakan hasil pengujian deklarasi CSS

	CSS Inline `blue`
	
	CSS Internal `red`
	
	CSS Eksternal `yellow`
![img](img/img11.png)

4. Deklarasi `id="paragraf-1"` akan ditampilkan pada browser, karena selektor id lebih spesifik dari class atau bahkan element P itu sendiri, kecuali jika kita menambahkan property pada inline element P maka selektor id tersebut akan tertimpa, karena inline lebih spesifik daripada id, class, dan element
![img](img/img12.png)