# Latihan 3: API
Latihan ini adalah untuk menunjukkan pemahaman membangunkan API menggunakan **_ExpressJS Framework_**

# Langkah 1.0: _Install Visual Studio Code Extension_
Langkah ini adalah untuk _install Express Framework_ dan _REST Client extensions_ untuk memudahkan pembangunan API

* Di Visual Studio Code, dari senarai ikon di kiri, klik _**Extension**_

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/25165bc1d1cd649f14bd96da890e1a44/image.png">

* Buat carian, _**ExpressJs 4 Snippets**_

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/49c4c53a495b34b47a44ac5711b43a7c/image.png">

* Klik Install

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/2713f45d6fa38c7c0f584517cb8182db/image.png">

* Buat carian sekali lagi, _**REST Client**_

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/4cb7cc8ec03a94979224becd8fa550ef/image.png">

* Klik Install

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/c83e430e1249301217ec6e353c49cc9d/image.png">

Note: Untuk menggunakan **REST Client**, pastikan **Code Lens** diaktifkan di **Visual Studio Code -> click Manage icon -> Settings -> Text Editor -> Enable Code Lens**

# Langkah 2.0: Penyediaan Persekitaran Projek

*  Buka aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS.

Nota: Untuk Windows, buka aplikasi ***Command Prompt*** dengan menggunakan **Administration mode** seperti paparan berikut:

<img src="https://code.cloud-connect.asia/Hanafiah/pembangunan-aplikasi-moden/uploads/c87c68041ae977df59582ea634de13bd/cmd-prompt.png">

*  Di aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS
*  Wujudkan direktori baru - latihan-5 dengan taip kod seperti berikut

```
> mkdir latihan-5
> cd latihan-5
```
* Taip kod berikut untuk membuka aplikasi Visual Studio Code

```
> code .
```

# Langkah 3.0: _**Initialize**_ Persekitaran NodeJS
Langkah ini adalah untuk initialize NodeJS environment sebagai langkah pertama untuk pembangunan API
*  Buka terminal, dari Menu klik _**Terminal -> New Terminal**_ 
*  Di terminal taip kod seperti berikut

```
> npm init
```
* Masukkan maklumat yang di perlukan seperti paparan berikut

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/52ea822daaa484df35b92d95e2386d25/image.png">

* Dari senarai ikon di kiri Visual Studio Code, klik ikon _**Explorer**_ untuk pastikan fail _**package.json**_ wujud dan mempunyai maklumat yang sama seperti yang dimasukkan sebelum ini. Sila rujuk paparan berikut:

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/ac4849231324d633864a5a7897f5be3d/image.png">

# Langkah 4.0: _Install ExpressJS Framework_
Langkah ini adalah untuk _Install ExpressJS Framework_
<br>
Sila layari https://www.npmjs.com/package/express untuk maklumat lanjut

*  Di terminal taip kod seperti berikut

```
> npm install express
```

* Setelah selesai, di fail _**package.json**_, pastikan _**express**_ adalah salah satu _**dependencies**_. Sila rujuk paparan berikut:

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/2bcc6ae4766a61355f76725ef761a2cc/image.png">

# Langkah 5.0: Penggunaan _ExpressJS Framework_
Langkah ini adalah untuk membangunkan API menggunakan ExpressJS Framework
* Wujudkan fail **index.js**. Dari Menu, klik **_File -> New File_**
* Salin dan tampal kod berikut

```
const express = require('express');
const app = express();

app.get('/', (req, res) => {
    res.send('Salam Muafakat!');
});

app.listen(8080, () => {
    console.log('App listening on port 8080!');
});

//Run app, then load http://localhost:8080 in a browser to see the output.
```
* Simpan / (_**Save**_) fail. Sila rujuk paparan berikut:

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/d3ea4578e7d749d9f419feaa7feef73a/image.png">

# Langkah 6.0: Uji Penggunaan ExpressJS Framework

* Di terminal taip kod seperti berikut:

```
> node index.js
```
* Jika berjaya, berikut adalah paparan maklumat di terminal:
```
App listening on port 8080!
```
* Buka internet browser, dan layari **http://localhost:8080** dengan paparan berikut

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/6b34f04a0263af57eaad377c073696ce/image.png" width=400>

* Di terminal, untuk **_stop_** applikasi NodeJS, tekan kekunci **_Ctrl-C_**

# Langkah 7.0: Using HTTP GET / POST & JSON
Langkah ini adalah untuk membangunkan API menggunakan _**HTTP GET / POST & JSON data**_


## Langkah 7.1: Using HTTP GET & JSON
Langkah ini adalah untuk membangunkan API menggunakan _**HTTP GET & JSON data**_

* Wujudkan fail **getjson.js**. Dari Menu, klik **_File -> New File_**
* Salin dan tampal kod berikut

```
const express = require('express');
const app = express();

app.get('/', (req, res) => {
    res.send('Salam Muafakat!');
});

app.get('/johor', (req, res) => {
    res.json({ data: "Salam Muafakat" });
});

app.listen(8080, () => {
    console.log('App listening on port 8080!');
});
```
* Simpan / (_**Save**_) fail. Sila rujuk paparan berikut:

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/f29dd7a41c2ab73394e67d9ee633873d/image.png">

## Langkah 7.2: Uji HTTP GET & JSON

* Di terminal taip kod seperti berikut:

```
> node getjson.js
```
* Jika berjaya, berikut adalah paparan maklumat di terminal:
```
App listening on port 8080!
```
* Buka internet browser, dan layari **http://localhost:8080/johor** dengan paparan berikut

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/1037338f2c7c100146a5103616b41782/image.png" width=400>

* Di terminal, untuk **_stop_** applikasi NodeJS, tekan kekunci **_Ctrl-C_**

## Langkah 7.3: _Install body-parser library_
Langkah ini adalah untuk menggunakan **_body-parser library to parse incoming HTTP POST request_**
<br>
Sila layari https://www.npmjs.com/package/body-parser untuk maklumat lanjut
*  Di terminal taip kod seperti berikut

```
> npm install body-parser
```

* Setelah selesai, di fail _**package.json**_, pastikan _**body-parser**_ adalah salah satu _**dependencies**_. Sila rujuk paparan berikut:

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/405b0fe55a2b08e16ee668d47d9e6c1f/image.png">

## Langkah 7.4: Using HTTP POST & JSON
Langkah ini adalah untuk membangunkan API menggunakan _**HTTP POST & JSON data**_

* Wujudkan fail **postjson.js**. Dari Menu, klik **_File -> New File_**
* Salin dan tampal kod berikut 

```
const express = require('express');
const bodyParser = require('body-parser');

const app = express();
app.use(bodyParser.json());
app.use(bodyParser.urlencoded({extended: false}));

app.post('/echo', (req, res) => {
    console.log(req.body);
    console.log("Nama saya " + req.body.nama);
    console.log("Saya berasal dari " + req.body.alamat);
    res.json({ data: "Maklumat diterima"})
});

app.get('/', (req, res) => {
    res.send('Salam Muafakat!');
});

app.get('/johor', (req, res) => {
    res.json({ data: "Salam Muafakat" });
});

app.listen(8080, () => {
    console.log('App listening on port 8080!');
});
```
* Simpan / (_**Save**_) fail. Sila rujuk paparan berikut:

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/2ad82e1e1c6ad3f58294cf69acffa018/image.png">

## Langkah 7.5: Uji HTTP POST & JSON

* Di terminal taip kod seperti berikut:

```
> node postjson.js
```
* Jika berjaya, berikut adalah paparan maklumat di terminal:
```
App listening on port 8080!
```
* Wujudkan fail **uji.http**. Dari Menu, klik **_File -> New File_**
* Salin dan tampal kod berikut 

```
POST http://localhost:8080/echo
content-type: application/json

{
    "nama": "hanafiah",
    "alamat": "Kota Tinggi"
}
```
* Simpan / (_**Save**_) fail. Sila rujuk paparan berikut:

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/a73779a212d1477bb89fcc6f3933a259/image.png">

* Di fail uji.http, klik **Send Request**. Sila rujuk paparan berikut:

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/5ba9e4f76d9db264df330f7ffd617283/image.png">

* Berikut adalah paparan di sebelah kanan jika berjaya

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/7ac2c800d9a23cd231af8336f7a82a4e/image.png">

* Berikut adalah paparan di terminal jika berjaya

<img src="https://gitlab.com/akademi-cloud-connect/johor-ict/latihan-pembangunan-aplikasi-moden/uploads/289ec9c3c15f696d48dfc13484bb4aee/image.png">

* Di terminal, untuk **_stop_** applikasi NodeJS, tekan kekunci **_Ctrl-C_**


# Langkah 8.0: Pengunaan NPM RUN
Langkah ini adalah untuk membuat konfigurasi NodeJS dengan menggunakan _command **NPM RUN**_
* Buka fail **package.json**.
* Tukar kod _**"script"**_ dengan salin dan tampal kod seperti berikut

```
"scripts": {
    "start": "node postjson.js"
  },
```
* Simpan / (_**Save**_) fail. 
* Di terminal taip kod seperti berikut:

```
> npm run start
```
* Jika berjaya, berikut adalah paparan maklumat di terminal (maklumat akan berbeza di terminal anda):
```
> latihan-5@1.0.0 start /Users/hanafiah/Documents/Development/node/latihan/latihan-5
> node postjson.js

App listening on port 8080!
```

* Di fail uji.http, klik **Send Request** untuk **POST http://localhost:8080/echo**. Jika berjaya maklumat yang sama akan di paparkan seperti ujian di Langkah 7.5
