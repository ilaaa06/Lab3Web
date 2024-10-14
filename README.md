Lab3Web  
Nur Laila (312310149)  
Ti 23 A1  

## 1. Pertanyaan dan Tugas (Dropdown  & List)
```sh
<form action="proses.php" method="post">
    <fieldset>
        <legend>Data Pelanggan</legend>
        <p>
            <label for="nama">Nama</label>
            <input type="text" id="nama" name="nama">
        </p>
        <p>
            <label for="alamat">Alamat</label>
            <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
        </p>
        <p>
            <label>Jenis Kelamin</label>
            <input id="jk_l" type="radio" name="kelamin" value="L" />
            <label for="jk_l">Laki-laki</label>
            <input id="jk_p" type="radio" name="kelamin" value="P" />
            <label for="jk_p">Perempuan</label>
        </p>
        <p>
            <!-- Dropdown Menu -->
            <label for="kategori">Pilih Kategori Pelanggan</label>
            <select id="kategori" name="kategori">
                <option value="umum">Umum</option>
                <option value="mahasiswa">Mahasiswa</option>
                <option value="pelajar">Pelajar</option>
                <option value="karyawan">Karyawan</option>
            </select>
        </p>
        <p>
            <!-- Listbox with Multiple Selection -->
            <label for="produk">Pilih Produk Favorit</label>
            <select id="produk" name="produk[]" multiple size="5">
                <option value="kopi">Kopi</option>
                <option value="teh">Teh</option>
                <option value="jus">Jus Buah</option>
                <option value="susu">Susu</option>
                <option value="air_mineral">Air Mineral</option>
            </select>
        </p>
        <p>
            <input type="submit" value="Submit">
        </p>
    </fieldset>
</form>
```
![image](https://github.com/user-attachments/assets/953e528f-9395-46b0-84d6-d4da42ec238c)  
Form ini mengumpulkan data pelanggan dengan komponen berikut:  
Nama: Input teks untuk mengisi nama pelanggan.  
Alamat: Textarea untuk memasukkan alamat.  
Jenis Kelamin: Pilihan radio untuk memilih antara "Laki-laki" dan "Perempuan".  
Dropdown Menu: Memilih satu kategori pelanggan (Umum, Mahasiswa, Pelajar, Karyawan).  
Listbox Multiple Selection: Memilih beberapa produk favorit (misalnya Kopi, Teh, Jus, dll.).   
Tombol Submit: Mengirim data ke file proses.php.   
# Praktikum dan Screenshots
## 1. membuat dokumen HTML dengan nama file lab3_list.html seperti berikut.
```sh
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
```  
![image](https://github.com/user-attachments/assets/6086e164-b182-4dc7-aa63-4e4f52d33af1)
## 2. Membuat Orderred List
```sh
<section id="order-List">
    <h2>Ordered List</h2>
    <ol>
        <li>Pemrograman Web</li>
        <li>Sistem Informasi</li>
        <li>BBasis Data 2</li>
    </ol>
</section>
```
![Screenshot 2024-10-14 175301](https://github.com/user-attachments/assets/0b261b2f-54db-482b-9517-815ce9e56eb3)   
`<ol>`: Tag untuk membuat ordered list (daftar yang terurut atau bernomor).
`<li>`: Setiap item dalam daftar didefinisikan dengan tag ini.
## 3. Membuat Unorderd List
Kemudian tambakan kode untuk membuat Unordered List, setelah deklarasi ordered list pada
section unordered-list, seperti berikut.
```sh
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type=""square">
        <li>Jaringan Komputer</li>
        <li>Struktur Data</li>
        <li>Algoritma &amp; Pemrograman</li>
    </ul>
</section>
```
![Screenshot 2024-10-14 175459](https://github.com/user-attachments/assets/358c05e3-2c23-44ff-874e-1e6f0892afaa)  
Menggunakan tag `<ul>` untuk membuat daftar tanpa urutan (bullet list).  
Tipe bullet bisa diubah dengan atribut type, misalnya "square" untuk bullet persegi.  
Setiap item dalam daftar menggunakan tag `<li>`.  
## 4. Membuat Description List
Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list.
```sh
<section id="unorder-list">
    <h2>Description List</h2>
    <dl>
        <dt>Fakultas Teknik</dt>
        <dd>Teknik Industri</dd>
        <dd>Teknik Informatika</dd>
        <dd>Teknik Lingkungan</dd>
        <dt>Fakultas Ekonomi dan Bisnis</dt>
        <dd>Akuntansi</dd>
        <dd>Manajemen</dd>
        <dd>Bisnis Digital</dd>
    </dl>
</section>
```
![Screenshot 2024-10-14 175642](https://github.com/user-attachments/assets/79b69f1e-646b-4063-aa12-b761a8375447)  
Menggunakan tag `<dl>` untuk membuat description list (daftar dengan deskripsi).   
Tag <dt> digunakan untuk mendefinisikan istilah utama (contoh: fakultas).  
Tag <dd> digunakan untuk memberikan deskripsi atau rincian dari istilah tersebut (contoh: jurusan dalam fakultas).  
## 5. Membuat Tabel
Buat file baru dengan nama lab3_tabel.html seperti berikut.
```sh
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Table</h1>
    </header>
</body>
</html>
```
![image](https://github.com/user-attachments/assets/9ca27aa9-458f-4ce8-855b-68dc1ce5d2ff)   
Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:  
```sh
<table border="1" cellpadding="4" cellspacing="0">
    <thead>
         <tr>
            <th>No.</th>
            <th>Fakultas</th>
            <th>Program Studi</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1.</td>
            <td>Teknik</td>
            <td>Teknik Informatika</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>Teknik</td>
            <td>Teknik Industri</td>
        </tr>
        <tr>
            <td>3.</td>
            <td>Teknik</td>
            <td>Teknik Lingkungan</td>
        </tr>
    </tbody>
</table>
```
![Screenshot 2024-10-14 175928](https://github.com/user-attachments/assets/119681a9-a321-4596-b675-8e22e311b77a)  
Di dalam elemen `<header>`, masukkan judul halaman dengan tag `<h1>` bertuliskan "Membuat Table" dan beri judul tab browser   
menggunakan `<title>` dengan teks "HTML Lanjutan". Selanjutnya, tambahkan tabel sederhana dengan tag `<table>` yang memiliki      
`atribut border="1"`, `cellpadding="4"`, dan `cellspacing="0"`. Buat bagian header tabel menggunakan `<thead>`, dengan baris header `<tr>`  
yang berisi kolom judul menggunakan tag `<th>` untuk "No.", "Fakultas", dan "Program Studi". Terakhir, isi tabel dengan data dalam tag `<tbody>`,    
menambahkan beberapa baris `<tr>` yang berisi nomor urut, nama fakultas, dan program studi seperti "Teknik Informatika", "Teknik Industri", dan "Teknik Lingkungan".  
## 6. Menggabungkan Sel Data
Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut rowspan untuk
menggabungkan baris (secara vertikal) dan colspan untuk menggabungkan kolom (secara
horizontal).
```sh
<table border="1" cellpadding="6" cellspacing="0">
    <thead>
         <tr>
            <th>No.</th>
            <th>Fakultas</th>
            <th>Program Studi</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1.</td>
            <td rowspan="3">Teknik</td>
            <td>Teknik Informatika</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>Teknik Industri</td>
        </tr>
        <tr>
            <td>3.</td>
            <td>Teknik Lingkungan</td>
        </tr>
    </tbody>
</table>
```
![Screenshot 2024-10-14 180333](https://github.com/user-attachments/assets/4e568209-bcf0-4b39-87ad-685eda588686)
Untuk menggabungkan sel data dalam tabel, gunakan atribut rowspan dan colspan. Atribut rowspan digunakan   
untuk menggabungkan sel secara vertikal (beberapa baris), sementara colspan digunakan untuk menggabungkan   
sel secara horizontal (beberapa kolom). Misalnya, dalam tabel berikut, kolom "Fakultas" dengan nilai "Teknik"   
digabungkan menjadi satu sel yang membentang tiga baris menggunakan `rowspan="3"`.    
# Membuat Form
Buat file baru dengan nama lab3_form.html seperti berikut.  
```sh
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>
</body>
</html>
```
![image](https://github.com/user-attachments/assets/8aae7c39-97a4-454a-8d19-8bbb39cbff2c)   
Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:  
```sh
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>
</body>
</html>
<form action="proses.php" method="post">
    <fieldset>
        <legend>Data Pelanggan</legend>
        <p>
             <label for="nama">Nama</label>
             <input type="text" id="nama" name="nama">
        </p>
        <p>
            <label for="alamat">Alamat</label>
            <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
        </p>
        <p>
            <label>Jenis Kelamin</label>
            <input id="jk_l" type="radio" name="kelamin" value="L" /><label
for="jk_l">Laki-laki</label>
            <input id="jk_p" type="radio" name="kelamin" value="P" /><label
for="jk_p">Perempuan</label>
        </p>
        <p><input type="submit" value="Login"></p>
    </fieldset>
</form>
```
![Screenshot 2024-10-14 181205](https://github.com/user-attachments/assets/77edb856-2b71-4a57-a85d-0ed175bfb457)  
Di dalam elemen `<header>`, masukkan judul halaman dengan tag `<h1>` yang berjudul `"Membuat Form"`.     
Selanjutnya, buat elemen `<form>` dengan atribut `action="proses.php"` untuk menentukan tujuan    
pengiriman data dan `method="post"` untuk mengatur metode pengiriman. Di dalam form, tambahkan elemen    
`<fieldset>` untuk mengelompokkan elemen formulir, dengan `<legend>` berisi judul `"Data Pelanggan"`.   
   
Di dalam `<fieldset>`, buat input untuk nama menggunakan tag `<label>` dan `<input type="text">`,    
diikuti dengan textarea untuk alamat menggunakan `<textarea>`. Tambahkan opsi jenis kelamin     
menggunakan input radio dengan dua pilihan: "Laki-laki" dan "Perempuan", masing-masing ditandai    
dengan tag `<input type="radio">` dan `<label>`. Akhiri dengan tombol submit menggunakan `<input type="submit">`,   
yang memungkinkan pengguna mengirimkan data ke file `proses.php` saat ditekan.   

## Menambahkan Style pada Form
Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.
```sh
<style>
    form p > label {
        display: inline-block;
        width: 100px;
    }
    form input[type="text"], form textarea {
        border: 1px solid #197a43;
    }
    form input[type="submit"] {
        border: 1px solid #197a43;
        background-color: #197a43;
        color: #ffffff;
        font-weight: bold;
        padding: 5px 15px;
    }
</style>
```
![Screenshot 2024-10-14 181355](https://github.com/user-attachments/assets/cd32db26-7869-4b6b-b310-100cd48eba3c)   
Tambahkan tag `<style>` di dalam elemen `<head>` untuk mengatur gaya form. Gaya pertama mengatur label agar ditampilkan    
dalam satu baris dengan lebar tetap. Kemudian, gaya untuk input teks dan textarea menggunakan border berwarna hijau.   
Gaya untuk tombol submit mengatur warna latar belakang, warna teks, dan penataan untuk menjadikannya lebih menonjol    
dengan padding dan border hijau.   






