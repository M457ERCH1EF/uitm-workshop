Kandungan:

[[_TOC_]]


# Latihan 2: NodeJS

Latihan ini adalah untuk menunjukkan pemahaman NodeJS

# Langkah 1.0: NodeJS ***Installation***

*  Muat turun aplikasi dan ***install*** nodeJS dari [https://nodejs.org/en/download/](https://nodejs.org/en/download/)
*  Buka aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS.

Nota: Untuk Windows, buka aplikasi ***Command Prompt*** dengan menggunakan **Administration mode** seperti paparan berikut:

<img src="https://code.cloud-connect.asia/Hanafiah/pembangunan-aplikasi-moden/uploads/c87c68041ae977df59582ea634de13bd/cmd-prompt.png">

*  Di aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS, taip kod berikut untuk melihat versi aplikasi node dan npm:
```
> node -v
> npm -v
```
<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/6dcc9b64b6407171537cc5dab4803d02/image.png" width="400">

# Langkah 2.0: Wujudkan projek NodeJS
*  Di aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS
*  Wujudkan direktori baru - latihan-2

```
> mkdir latihan-2
> cd latihan-2
```
* Taip kod berikut untuk membuka aplikasi **Visual Studio Code**

```
> code .
```
* Wujudkan fail **index.js**. Dari Menu, klik **_File -> New File_**

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/e2f4f6a855259f435b63bf1e1e4fb6ef/image.png" width=350>

* Salin dan tampal kod berikut dan simpan / (_**Save**_) fail

```
console.log("Selamat Datang ke Latihan NodeJS")
```
nota: gunakan CTRL-S untuk simpan fail

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/4134469ee88370b6949bec89e4e17bb7/image.png">

# Langkah 3.0: Uji aplikasi
*  Dari Menu Visual Studio Code buka terminal seperti paparan berikut

<img src="https://code.cloud-connect.asia/Hanafiah/pengenalan-aplikasi-moden/uploads/f02cbf2409449b5d461dc7737676a88b/image.png" width="300">

*  Di terminal taip kod seperti berikut untuk mulakan aplikasi Node.js

```
> node index.js
```
atau 

```
> node .
```

Pastikan paparan di terminal adalah **Selamat Datang ke Latihan NodeJS**


# Langkah 4.0: NodeJS dan javascript 
*  Padam semua kod di fail _**index.js**_, Salin dan tampal kod berikut

```
function tambah(a,b){
    console.log(a + b)
}
tambah(5,2)
```

*  Simpan / **Save** fail index.js

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/2bdc0a5f7ebdee4621aea34150b1b1db/image.png">

# Langkah 5.0: Uji aplikasi - NodeJS dan javascript

*  Di terminal taip kod seperti berikut untuk mulakan aplikasi Node.js

```
> node index.js
```
Pastikan paparan di terminal adalah **7**


# Langkah 6.0: Penggunaan javascript 
*  Padam semua kod di fail _**index.js**_, Salin dan tampal kod berikut

```
function tambah(a,b){
    let jawapan = a + b
    console.log("Jumlah = " + jawapan)
}
tambah(5,2)
```

*  Simpan / **Save** fail index.js

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/e9cc81c49c99f01344bc6cf2940a3bcd/image.png">

# Langkah 7.0: Uji aplikasi - Penggunaan javascript

*  Di terminal taip kod seperti berikut untuk mulakan aplikasi Node.js

```
> node index.js
```
Pastikan paparan di terminal adalah **Jumlah = 7**
