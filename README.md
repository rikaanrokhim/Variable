# Variabel, Konstanta dan Ekspresi

## 1. Variabel

__Variabel__ merupakan tempat penyimpanan yang digunakan untuk menyimpan suatu data atau nilai, yang bersifat sementara. 
Isi dari Variabel dapat berubah-ubah selama proses program. Suatu variable dalam pemrograman PHP diawali dengan tanda `$` dan diikuti oleh nama variabel yang bersifat _case sensitive_ artinya huruf besar dan huruf kecil disini berlaku.

### Aturan Penamaan Variabel 

* Setiap nama variabel PHP didahului dengan tanda `$` .
* Nama variabel PHP hanya terdiri dari karakter (A-z), angka (0-9), dan underscore.
* Nama variabel PHP harus didahului dengan karakter (A-z) atau underscore dan tidak boleh didahului dengan angka (0-9).
* Nama variabel PHP bersifat 'case-senstive', yaitu ada berpedaan antara huruf besar A dengan huruf kecil a ($nama berbeda dengan $Nama, berbeda dengan $NAMA.
* Data yang ditunjukkan ke variabel PHP dapat berupa nilai (misalnya: `$x = 5`) atau berupa ekspresi (misalnya: `$x = $y + $z`).
* Jika nilai variabel berupa suatu teks (string), tambahkan tanda kutip untuk mengapit nilai tersebut. (misalnya `$x = "Ini nilai berupa teks"`.

### Jenis Variabel Berdasarkan Cakupannya

* Variabel Global: didefinisikan dan berlaku hanya di luar fungsi PHP buatan.
* Variabel Lokal: didefinisikan dan berlaku hanya di dalam fungsi PHP buatan.
* Variabel Super-global:dapat berlaku di dalam maupun diluar fungsi PHP.

```php
$_var = "dhezign";
$var = "dhezign";
$dhezign = 1;
```

### Link Belajar

* [Variabel PHP](http://m261an.com/belajar-php/PHPa_VariabelKonstanta.php)


## 2. Konstanta

__Konstanta (constant)__ adalah suatu lokasi penyimpanan (dalam memory) yang berisikan nilai yang sifatnya tetap dan tidak bisa diubah sepanjang program berjalan.
Cara penamaan konstanta sama seperti variable yaitu diawali dengan huruf atau underscore untuk karakter pertama, kemudian boleh diikuti dengan huruf, underscore atau angka untuk karakter kedua dan selanjutnya.
### Cara Pendefisian Konstanta
* Menggunakan Keyword `const`
Pendefinisian konstanta menggunakan keyword const hanya dapat digunakan pada top-level scope, yakni harus dalam lingkungan global PHP. 
Sehingga kita tidak bisa menggunakan const di dalam function, loop, atau kondisi if.

```php
const saya = "developer";
    echo saya;
```

* Menggunakan Fungsi `define()`
Mendefinisikan konstanta menggunakan fungsi `define()` maka membutuhkan dua nilai yaitu nama konstanta dan nilainya.

```php
define("saya", "developer");
    echo saya;
```

### Bersifat Case Sensitif

Bersifat Case Sensitif yaitu konstanta User, user dan USER akan dianggap sebagai tiga konstanta yang berbeda.

### Nilai Tidak Dapat Diubah

Konstanta sifatnya tetap dan tidak bisa diubah sepanjang program berjalan. Jika terdapat perubahan maka akan terjadi eror.

### Predefined Constants

PHP sendiri juga telah membawa konstanta bawaaan atau Predefined Constants atau Reserved Constants, artinya terdapat konstanta yang bawaan yang tidak boleh didefinisikan kembali oleh programmer. Contoh beberapa Predefined Constants:

`PHP_VERSION, PHP_MAJOR_VERSION, PHP_MINOR_VERSION, PHP_RELEASE_VERSION, PHP_VERSION_ID, PHP_EXTRA_VERSION, PHP_ZTS, PHP_DEBUG, PHP_MAXPATHLEN, PHP_OS, PHP_SAPI, PHP_EOL, PHP_INT_MAX, PHP_INT_SIZE, DEFAULT_INCLUDE_PATH, PEAR_INSTALL_DIR, PEAR_EXTENSION_DIR, PHP_EXTENSION_DIR, PHP_PREFIX, PHP_BINDIR, PHP_BINARY, PHP_MANDIR, PHP_LIBDIR, PHP_DATADIR, __LINE__ , __FILE__ , __DIR__ , __FUNCTION__ , __CLASS__ , __TRAIT__ , __METHOD__, __NAMESPACE__`

### Link Belajar

* [Konstanta PHP](http://php.net/manual/en/reserved.constants.php)
* [Konstanta di PHP](https://khoerodin.id/others/konstanta-dalam-php/)


## 3. Ekspresi
Segala yang memiliki nilai didalam pemrograman PHP dapat dikatakan sebagai Ekspresi. Dalam bentuk yang paling sederhana ekspresi dapat berupa konstanta maupun variable.

### Contoh:
`$a= 3`

Pada contoh diatas `$a` merupakan ekspresi yang bernilai `3` sedangkan `3` merupakan konstanta integer. 
Dalam bentuk yang kompleks ekspresi melibatkan operator dan operand.

`10 + 2 * 5`
Contoh tersebut merupakan sebuah bentuk dari ekspresi yang menghasilkan nilai `20`, dimana `10`, `2` dan `5` merupakan operand (nilai asal dalam sebuah operasi) dan tanda `+` dan `*` merupakan operator.

### Link Belajar

* [Eskpresi pada PHP](http://puroza.blogspot.co.id/2013/04/ekspresi-dasar-pemrograman-php.html#.WemeevmCy00)
