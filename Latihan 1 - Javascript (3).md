[[_TOC_]]

# Latihan 1: Javascript

Latihan ini adalah untuk menunjukkan penggunaan Javascript di *web browser*

# Langkah 1.0: Pemahaman *Web browser*

*  Di Chrome *web browser*, buka laman web - http://www.cloud-connect.asia/
*  ***Right Click*** di web browser dan pilih ***Inspect***

<img src="https://code.cloud-connect.asia/Hanafiah/pengenalan-aplikasi-moden/uploads/ff9c3f8d3303e81bddbdc94b0c92e79b/image.png" width=200>

*  Pilih Tab ***Console***

<img src="https://code.cloud-connect.asia/Hanafiah/pengenalan-aplikasi-moden/uploads/0ede97b671887d83c8abf8fa1a751191/image.png" width=400>

# Langkah 2.0: Pemahaman *HTML DOM Structure*

<img src="https://code.cloud-connect.asia/Hanafiah/pengenalan-aplikasi-moden/uploads/948973a3552ef41dcb15531358a1b833/image.png" width=400>

## Langkah 2.1: Mendapatkan tajuk laman web

*  Di Chrome ***Inspect*** tab, taip kod seperti di bawah

```
> document.title
```
<img src="https://code.cloud-connect.asia/Hanafiah/pengenalan-aplikasi-moden/uploads/d40e4e43fe1676ea1b180b9021186e22/image.png" width="400">

## Langkah 2.2: Mendapatkan alamat di laman web

*  Di Chrome *web browser*, buka laman web - http://www.cloud-connect.asia/contact-us/
*  ***Right Click*** di web browser dan pilih ***Inspect***
*  Di Chrome ***Inspect*** tab, taip kod seperti di bawah
  
```
> document.getElementsByTagName('p')[0].innerHTML
```
<img src="https://code.cloud-connect.asia/Hanafiah/pengenalan-aplikasi-moden/uploads/3db3439178fa7b54be05a649562e44f4/image.png" width="500">


# Langkah 3: Penggunaan Javascript di *web browser*


*  Di Chrome ***Inspect*** tab, taip kod seperti di bawah

```
> function tambah(a,b) { return a+b }
```
<img src="https://code.cloud-connect.asia/Hanafiah/pengenalan-aplikasi-moden/uploads/2b316788be4b194157b2c1788f22823d/image.png" width="500">

*  taip kod seperti di bawah

```
> tambah(2,3)
```

<img src="https://code.cloud-connect.asia/Hanafiah/pengenalan-aplikasi-moden/uploads/9c65de22ab0f6696b42c819b65a2355b/image.png" width="200">
