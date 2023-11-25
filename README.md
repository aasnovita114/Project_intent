# Project_intent

<table>
  <tr>
    <th colspan="2">DATA MAHASISWA</th>
  </tr>
  <tr>
    <td>Nama</td>
    <td>Aas Novitasari</td>
  </tr>
  <tr>
    <td>NIM</td>
    <td>312210167</td>
  </tr>
  <tr>
    <td>Kelas</td>
    <td>TI.22.A1</td>
  </tr>
</table>

# Tugas :
```
Buatkanlah :

1. Launcher Splash logo masing-masing Individu 

2. Buatkanlah untuk menampilkan semua project sebelum UTS dengan metode Ekplisit Intent dan

     Implisit Intent:

    a. Project Hallo

    b. Project Count

    c. Project Sianida

    d. Project TwoActivity

    e. Project Set Alarm

 
Untuk tampilan Layout Bebas, terima kasih.
```
Launcher Splash Logo Pertama, yaitu membuat Launcher Splash Logo atau menampilkan logo / icon saat kita pertama kali membuka aplikasi. Caranya adalah :

* Persiapkan gambar terlebih dahulu
* Selanjutnya kita klik app, lalu klik res dan setelahnya kita pilih dan klik mipmap
* Setelah itu klik kanan pada bagian mipmap , lalu pilih new
* Lalu pilih dan klik Image Asset
* Lalu ketika sudah terbuka, kita klik bagian Icon Type lalu pilih yang Launcher Icons (Adaptive and Legacy)
* Lalu pada bagian Path kita klik logo file lalu kita pilih dan klik file gambar yang telah disiapkan sebelumnya dan klik OK
* Lalu untuk ukuran logo / ikon bisa kita atur pada bagian Resize, Jika sudah kita klik Next
* Setelah itu kita klik Finish, Maka logo / ikon aplikasi kita akan berubah sesuai gambar yang kita inginkan

Untuk menambahkan file gambar seperti untuk SplashScreen, Background di setiap project kita bisa klik bagian Resource Manager lalu kita klik tanda +. Setelah itu kita pilih dan klik Import Drawables, setelah itu kita pilih dan klik file gambar yang sudah kita siapkan lalu klik OK. Maka gambar akan tersedia di res pada drawable.

* Lalu buka backgroundlauncher.xml dan masukkan code ini :
```
<?xml version="1.0" encoding="utf-8"?>
<layer-list xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:drawable="@color/birumuda"/>
    <item>
        <bitmap
            android:src="@drawable/logo"
            android:gravity="center" />
    </item>
</layer-list>
```
* Lalu, buka themes.xml yang letaknya ada di res/values/themes, dan tambahkan code ini didalam resourcesnya ;
  ```
  <resources xmlns:tools="http://schemas.android.com/tools">
    <!-- Base application theme. -->
    <style name="SplashScreen" parent="Theme.MaterialComponents.DayNight.NoActionBar">
        <item name="android:windowBackground">@drawable/logo</item>
        <item name="android:statusBarColor">?attr/colorOnPrimary</item>
    </style>
</resources>
```
