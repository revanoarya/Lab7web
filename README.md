## Nama    : Revano Arya Saputra
## Kelas   : TI.20.A.1
## Matkul  : Pemograman Web 
## Pertemuan 9 Lab7Web <b>
Dalam pertemuan 9 ini kita akan mempelajari PHP Dasar dengan beberapa program code PHP nya.
## PHP Dasar <b>
## 1. Install XAMPP <b>
![1](https://user-images.githubusercontent.com/101621068/168739100-1675e988-d5ef-42b7-bec0-4e6f2740990d.png)
Install XAMPP kemudian ekstrak file dan sesuaikan lokasi penyimpanannya.
## 2. Menjalankan XAMPP <b>
![2](https://user-images.githubusercontent.com/101621068/168739382-f93e186b-16f2-4f89-a5a8-e92efb2eed9e.png)
Menjalankan XAMPP dengan cara klik tombol Start pada server Apache seperti di gambar.
## 3. Memulai PHP <b>
![3](https://user-images.githubusercontent.com/101621068/168739543-924122cf-fe58-45b5-b14a-0e6bd50fa47f.png)
Buat folder lab7_php_dasar pada root directory web server (c:xampp/htdocs).
Kemudian akses directory pada web server dengan mengakses URL :
http://localhost/lab7web/lab7_php_dasar/
![4](https://user-images.githubusercontent.com/101621068/168740145-4b3e9690-4120-4b51-810b-c9b8808d2f1f.png)
## 4. PHP Dasar <b>
![5](https://user-images.githubusercontent.com/101621068/168740303-2082a5f7-adc5-48ff-8dd4-b9c34be953f9.png)
Berikut adalah hasil Run PHP Dasar
### Contoh Codingan <b>
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PHP Dasar</title>
</head>
<body>
    <h1>Belajar PHP Dasar</h1>
    <?php
        echo "Hello World";
    ?>
```
## 5. Variabel PHP
![6](https://user-images.githubusercontent.com/101621068/168741611-30ae671d-3baa-45e8-af94-acd553cd174a.png)
Berikut adalah hasil Run Variabel PHP
### Contoh Codingan <b>
```html
    <!-- Variabel PHP -->
    <h2>Menggunakan Variabel</h2>
    <?php
        $nim = "0411500400";
        $nama = 'Abdullah';
        echo "NIM : " . $nim . "<br>";
        echo "Nama : $nama";
    ?>
```
## 6. Predefine $_GET <b>
![7](https://user-images.githubusercontent.com/101621068/168745632-a4ffdb2d-e594-47d8-817f-d7e7f4a01b44.png)
Buat file baru dalam directory lab7_php_dasar dengan nama filenya adalah latihan2.php dan untuk mengaksesnya menggunakan URL :
http://localhost/lab7web/lab7_php_dasar/php_dasar.php?nama=%20Denas
### Contoh Codingan <b>
```html
    <!-- Variabel $_GET -->
    <h2>Predefine Variabel</h2>
<?php
    echo 'Selamat Datang'. $_GET['nama'];
?>
```
## 7. Membuat Form Input <b>
![8](https://user-images.githubusercontent.com/101621068/168748851-365dddd1-777a-4c74-aac7-891d1d20aca9.png)
Buat File baru dengan nama latihan3.php dalam directory folder lab7_php_dasar
Berikut adalah hasil atau tampilan dalam membuat form dalam php dengan variable $_POST
### Contoh Coding <b>
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>
<body>
<h2>Form Input</h2>
<form method="post">
    <label>Nama: </label>
    <input type="text" name="nama">
    <input type="submit" value="Kirim">
</form>
<?php
    echo 'Selamat Datang ' . $_POST['nama'];
?>
</body>
</html>
```
## 8. Operator <b>
![9](https://user-images.githubusercontent.com/101621068/168749767-bfa95649-918e-4c9a-89e3-1b22e91aff2c.png)
Membuat OPERATOR dalam php seperti contoh hasil tampilan di atas beserta code nya.
### Contoh Codingan <b>
```html
<h2>Operator</h2>
<?php
    $gaji = 1000000;
    $pajak = 0.1;
    $thp = $gaji - ($gaji*$pajak);
        echo "Gaji sebelum pajak = Rp. $gaji <br>";
        echo "Gaji yang dibawa pulang = Rp. $thp";
?>
```
## 9. Kondisi IF <b>
![10](https://user-images.githubusercontent.com/101621068/168750379-bf117664-d3e0-4756-ac56-3e80984171c9.png)
## 10. Kondisi Switch
![11](https://user-images.githubusercontent.com/101621068/168751037-b8d21956-aa03-4f4f-b0ac-a4d6a1a5296a.png)
Contoh penggunaan pengondisian SWICTH CASE dengan Break seperti contoh hasil diatas beserta code.
### Contoh Codingan <b>
```html
 <h2>Kondisi Switch</h2>
<?php
    $nama_hari = date("l");
    switch ($nama_hari) {
        case "Sunday":
            echo "Minggu";
            break;
        case "Monday":
            echo "Senin";
            break;
        case "Tuesday":
            echo "Selasa";
            break;
        default:
            echo "Sabtu";
    }
    echo"/$nama_hari";
?>
```
## 11. Perulangan For
![12](https://user-images.githubusercontent.com/101621068/168751854-91dff157-d48a-4aab-9c6e-56146d2b6a84.png)
Menggunakan PERULANGAN WHILE seperti hasil gambar dan code di atas.
### Contoh Codingan <b>
```html
    <h2>Perulangan For</h2>
<?php
        echo "Perulangan 1 sampai 10 <br />";
    for ($i=1; $i<=10; $i++) {
        echo "Perulangan ke: " . $i . '<br />';
    }
        echo "Perulangan Menurun dari 10 ke 1 <br />";
    for ($i=10; $i>=1; $i--) {
        echo "Perulangan ke: " . $i . '<br />';
    }
?>
```
## 12. Perulangan While <b>
![13](https://user-images.githubusercontent.com/101621068/168754423-cfa18eb8-0ec6-4fc4-97ea-1e65d49fb9ce.png)
### Contoh Codingan <b>
```html
<h2>Perulangan While</h2>
<?php
        echo "Perulangan 1 sampai 10 <br />";
        $i=1;
    while ($i<=10) {
        echo "Perulangan ke: " . $i . '<br />';
        $i++;
    }
?>
```
## 13. Perulangan Dowhile <b>
![14](https://user-images.githubusercontent.com/101621068/168754492-14c42d77-e71e-4cb7-83b7-7fa2bdb24467.png)
### Contoh Codingan <b>
```html
<h2>Perulangan Dowhile</h2>
<?php
        echo "Perulangan 1 sampai 10 <br />";
        $i=1;
    do {
        echo "Perulangan ke: " . $i . '<br />';
        $i++;
        } while ($i<=10);
?>
```
## Pertanyaan & Tugas <b>

Buatlah program PHP sederhana dengan menggunakan form input yang menampilkan nama , tanggal lahir dan pekerjaan . Kemudian tampilkan outputnya dengan menghitung umur berdasarkan inputan tanggal lahir . Dan pilihan pekerjaan dengan gaji yang berbeda-beda sesuai pilihan pekerjaan.

![15](https://user-images.githubusercontent.com/101621068/168755092-e71f04dc-bb81-4649-a7e0-e07591bcae9c.png)
![15](https://user-images.githubusercontent.com/101621068/168781601-d1b7bd47-578f-4d32-a07a-3f059f27e525.png)

### Contoh Codingan <b>
```html
   <h2>TUGAS</h2>
    <form class="form" method="post" >
            <label>Nama: </label>
            <br>
            <input type="text" name="nama">
            <br>
            <label>Tanggal Lahir: </label>
            <br>
            <input type="text" name="tgl_lahir">
            <br>
            <label>Pekerjaan: </label>
            <br>
            <select name='pekerjaan'>
                <option value="-">>---Pilih Pekerjaan---<</option>
                <option value='Operator'>Operator</option>
                <option value='Staff Admin'>Staff Admin</option>
                <option value='HRD'>HRD</option>
                <option value='Maintenance'>Maintenance</option>
                <option value="QC">QC</option>
            </select>
            <br>
            <br>
            <button type="submit">Kirim</button>
    </form>
    <h2>HASIL</h2>
    <?php
        # Memanggil Nama
        echo 'Nama: ' . $_POST['nama'];
        # Merubah Tanggal Lahir menjadi Umur (Tahun)
        $tgl_lahir = @$_POST['tgl_lahir'];
        $lahir = new DateTime($tgl_lahir);
        $hari_ini = new DateTime();
        $diff = $hari_ini->diff($lahir);
        # Memanggil fungsi umur yg sudah dibuat diatas
        echo "<br> Umur: ". $diff->y ." Tahun";
        # Memanggil pekerjaan
        echo "<br> Pekerjaan: ". $_POST['pekerjaan'];
        # Kondisi if pekerjaan untuk menentukan gaji
        $pekerjaan = @$_POST['pekerjaan'];
        if($pekerjaan == "Operator"){
            echo '<br> Gaji: Rp. 6.000.000,-';
        }elseif($pekerjaan == "Staff Admin"){
            echo '<br> Gaji: Rp. 7.500.000,-';
        }elseif($pekerjaan == "HRD"){
            echo '<br> Gaji: Rp. 10.000.000,-';
        }elseif($pekerjaan == "Maintenance"){
            echo '<br> Gaji: Rp. 9.000.000,-';
        }elseif ($pekerjaan == "QC"){
            echo '<br> Gaji: Rp. 7.000.000,-';
        }
    ?>
```
# TERIMAKASIH
