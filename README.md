---
date created: 2023-04-04 09:38
date updated: 2023-04-04 10:55
---

# Javascript Cheatsheets

Cheatsheet(s)<sup>[1](#footnote1)</sup> simpel ini sebenarnya dibuat dan dicatat pada dokmuen word pada saat saya gabut gak tau mau ngapain (2018). Kemudian saya tulis kembali untuk saya jadikan referensi pribadi dan bukan untuk apa-apa. Ini juga ditulis ulang karena gabut (2023).

## Table of Contents

| No | JavaScript Dasar                                                  |
| -- | ----------------------------------------------------------------- |
| 1  | [Program Hello World](#program-hello-world)                       |
| 2  | [Komentar](#komentar)                                             |
| 3  | [Tipe Data Number](#tipe-data-number)                             |
| 4  | [Tipe Data Number](#tipe-data-number)                             |
| 5  | [Tipe Data Boolean](#tipe-data-boolean)                           |
| 6  | [Tipe Data String](#tipe-data-string)                             |
| 7  | [Variable](#variable)                                             |
| 8  | [Operator Matematika](#operator-matematika)                       |
| 9  | [Operator Perbandingan](#operator-perbandingan)                   |
| 10 | [Operator Logika](#operator-logika)                               |
| 11 | [Console](#console)                                               |
| 12 | [String Template](#string-template)                               |
| 13 | [Konversi String dan Number](#konversi-string-dan-number)         |
| 14 | [Tipe Data Array](#tipe-data-array)                               |
| 15 | [Tipe Data Object](#tipe-data-object)                             |
| 16 | [If Expressions](#if-expressions)                                 |
| 17 | [Popup](#popup)                                                   |
| 18 | [Undefined](#undefined)                                           |
| 19 | [Null](#null)                                                     |
| 20 | [Switch Expression](#switch-expression)                           |
| 21 | [Operator Typeof](#operator-typeof)                               |
| 22 | [Operator In](#operator-in)                                       |
| 23 | [Ternary Operator](#ternary-operator)                             |
| 24 | [Optional Chaining](#optional-chaining)                           |
| 25 | [Falsy and Truthy](#falsy-and-truthy)                             |
| 26 | [Operator Logika di Non Boolean](#operator-logika-di-non-boolean) |
| 27 | [For Loop](#for-loop)                                             |
| 28 | [While Loop](#while-loop)                                         |
| 29 | [Do While Loop](#do-while-loop)                                   |
| 30 | [Break and Continue](#break-and-continue)                         |
| 31 | [Label](#label)                                                   |
| 32 | [For In](#for-in)                                                 |
| 33 | [For Of](#for-of)                                                 |
| 34 | [With Statement](#with-statement)                                 |
| 35 | [Function](#function)                                             |
| 36 | [Function Parameter](#function-parameter)                         |
| 37 | [Function Return Value](#function-return-value)                   |
| 38 | [Optional Parameter](#optional-parameter)                         |
| 39 | [Default Parameter](#default-parameter)                           |
| 40 | [Rest Parameter](#rest-parameter)                                 |
| 41 | [Function Sebagai Value](#function-sebagai-value)                 |
| 42 | [Anonymous Function](#anonymous-function)                         |
| 43 | [Function dalam Function](#function-dalam-function)               |
| 44 | [Scope](#scope)                                                   |
| 45 | [Recursive Function](#recursive-function)                         |
| 46 | [Function Generator](#function-generator)                         |
| 47 | [Arrow Function](#arrow-function)                                 |
| 48 | [Closure](#closure)                                               |
| 49 | [Object Method](#object-method)                                   |
| 50 | [Kata Kunci This](#kata-kunci-this)                               |
| 51 | [Arrow Function di Object](#arrow-function-di-object)             |
| 52 | [Getter dan Setter](#getter-dan-setter)                           |
| 53 | [Masalah Variable Var](#masalah-variable-var)                     |
| 54 | [Destructuring](#destructuring)                                   |
| 55 | [Strict Mode](#strict-mode)                                       |

Sequel:

- [JavaScript Object Oriented Programming](#) (Soon)
- [Javascript Standard Library](#) (Soon)

---

# Javascript Dasar

### Program Hello World

```javascript
console.log("hello world");
```

Program ini akan mencetak pesan `"Hello World"` di konsol.

[⬆️ Back to Top](#table-of-contents)

---

### Komentar

Anda dapat menambahkan komentar dengan menggunakan tanda `//` untuk komentar
satu baris atau `/* */` untuk komentar beberapa baris, contohnya seperti ini:

```javascript
// ini adalah komentar satu baris

/*
dan ini adalah komentar banyak baris
yang bisa dilakukan di dalam javascript
*/
```

Dengan menambahkan komentar pada kode Anda, Anda dapat membantu memudahkan
pemahaman tentang kode bagi Anda dan bagi orang lain yang akan membaca kode
tersebut di kemudian hari.

[⬆️ Back to Top](#table-of-contents)

---

### Tipe Data Number

Di dalam JavaScript, tipe data Number digunakan untuk merepresentasikan bilangan
bulat (integer) atau bilangan pecahan (float). Contohnya:

```javascript
let integerNumber = 10; // bilangan bulat
let floatNumber = 3.14; // bilangan pecahan
```

Selain itu, JavaScript juga memiliki beberapa nilai khusus yang termasuk dalam
tipe data Number, yaitu:

- `Infinity`: merepresentasikan nilai tak terhingga.
- `-Infinity`: merepresentasikan nilai tak terhingga negatif.
- `NaN` (Not a Number): merepresentasikan hasil operasi matematika yang tidak
  valid.

Contohnya:

```javascript
let positiveInfinity = Infinity;
let negativeInfinity = -Infinity;
let notANumber = NaN;
```

Nilai khusus ini seringkali muncul dalam operasi matematika tertentu, seperti
pembagian dengan angka nol atau hasil operasi matematika yang tidak valid.

[⬆️ Back to Top](#table-of-contents)

---

### Tipe Data Boolean

Di dalam JavaScript, tipe data boolean digunakan untuk merepresentasikan nilai
kebenaran (true atau false). Contohnya:

```javascript
let isTodayFriday = true;
let isJavaScriptFun = false;
```

Tipe data boolean sangat penting dalam pengambilan keputusan dalam program. Kita
dapat menggunakan operator perbandingan atau logika untuk membandingkan nilai
dan menghasilkan nilai boolean. Berikut adalah contoh penggunaan operator
perbandingan:

```javascript
let numberOne = 10;
let numberTwo = 5;

let isNumberOneGreater = numberOne > numberTwo; // true
let isNumberTwoGreater = numberTwo > numberOne; // false
```

Berikut adalah contoh penggunaan operator logika:

```javascript
let isRaining = true;
let isCold = false;

let shouldStayIndoors = isRaining || isCold; // true
let shouldGoOutdoors = isRaining && !isCold; // false
```

Dalam contoh di atas, operator `||` (OR) menghasilkan nilai true jika salah satu
atau kedua operand memiliki nilai true. Sedangkan operator `&&` (AND)
menghasilkan nilai true jika kedua operand memiliki nilai true. Operator `!`
(NOT) digunakan untuk membalikkan nilai boolean.

[⬆️ Back to Top](#table-of-contents)

---

### Tipe Data String

Di dalam JavaScript, tipe data string digunakan untuk merepresentasikan teks
atau karakter. Contohnya:

```javascript
let firstName = "John";
let lastName = "Doe";
let fullName = firstName + " " + lastName;
```

Variabel fullName akan berisi string `"John Doe"`, karena nilai dari variabel
firstName dan lastName digabungkan dengan menggunakan operator `+`.

Selain itu, JavaScript juga mendukung penggunaan tanda kutip tunggal (`'...'`)
atau tanda kutip ganda (`"..."`) untuk merepresentasikan string. Anda dapat
menggunakan salah satu tanda kutip ini, asalkan tanda kutip pembuka dan penutup
yang digunakan cocok. Contohnya:

```javascript
let singleQuoteString = "Ini adalah string dengan tanda kutip tunggal.";
let doubleQuoteString = "Ini adalah string dengan tanda kutip ganda.";
```

Jika Anda ingin menggunakan tanda kutip yang sama di dalam string, Anda dapat
melakukannya dengan menambahkan tanda `\` sebelum tanda kutip tersebut.
Contohnya:

```javascript
let stringWithQuotes =
	'Ini adalah string dengan tanda kutip "ganda" di dalamnya.';
```

Selain itu, JavaScript juga memiliki beberapa metode bawaan untuk memanipulasi
string, seperti length untuk menghitung panjang string, `toUpperCase` untuk
membuat semua karakter di dalam string menjadi huruf kapital, dan sebagainya.

[⬆️ Back to Top](#table-of-contents)

---

### Variable

```javascript
let myVariable = "Hello World";
```

Variabel di atas diberi nama `myVariable` dan diinisialisasi dengan nilai string
`"Hello World"`. Keyword `let` digunakan untuk mendeklarasikan variabel di dalam
JavaScript. Anda juga dapat menggunakan keyword `var` atau `const`, tergantung
pada kebutuhan Anda.

Variabel juga dapat diinisialisasi dengan nilai dari tipe data lain, seperti
number atau boolean. Contohnya:

```javascript
let myNumber = 42;
let isTrue = true;
```

Dengan variabel, Anda dapat menyimpan nilai yang akan digunakan di dalam program
dan memanipulasi nilai tersebut dengan menggunakan operasi atau fungsi tertentu.

[⬆️ Back to Top](#table-of-contents)

---

### Operator Matematika

Di dalam JavaScript, operator matematika digunakan untuk melakukan operasi
matematika pada nilai numerik. Berikut adalah beberapa contoh operator
matematika yang dapat digunakan di dalam JavaScript:

- Penjumlahan (`+`): Digunakan untuk menjumlahkan dua nilai numerik atau
  menggabungkan dua string. Contohnya:

```javascript
let x = 10;
let y = 5;
let result = x + y; // result akan bernilai 15

let firstName = "John";
let lastName = "Doe";
let fullName = firstName + " " + lastName; // fullName akan bernilai "John Doe"
```

- Pengurangan (`-`): Digunakan untuk mengurangkan satu nilai numerik dari nilai
  yang lain. Contohnya:

```javascript
let x = 10;
let y = 5;
let result = x - y; // result akan bernilai 5
```

- Perkalian (`*`): Digunakan untuk mengalikan dua nilai numerik. Contohnya:

```javascript
let x = 10;
let y = 5;
let result = x * y; // result akan bernilai 50
```

Pembagian (`/`): Digunakan untuk membagikan satu nilai numerik dengan nilai yang
lain. Contohnya:

```javascript
let x = 10;
let y = 5;
let result = x / y; // result akan bernilai 2
```

Sisa Bagi atau Modulus (`%`): Digunakan untuk mendapatkan sisa dari hasil
pembagian dua nilai numerik. Contohnya:

```javascript
let x = 10;
let y = 3;
let result = x % y; // result akan bernilai 1
```

Operator matematika ini dapat digunakan dalam ekspresi matematika yang lebih
kompleks, dan juga dapat digunakan dengan nilai variabel dan konstanta yang
dideklarasikan sebelumnya.

[⬆️ Back to Top](#table-of-contents)

---

### Operator Perbandingan

Di dalam JavaScript, operator perbandingan digunakan untuk membandingkan dua
nilai. Operator perbandingan akan mengembalikan nilai boolean (true atau false)
tergantung pada apakah perbandingan tersebut benar atau salah. Berikut adalah
beberapa contoh operator perbandingan yang dapat digunakan di dalam JavaScript:

- Sama dengan (`==`): Digunakan untuk membandingkan apakah dua nilai memiliki
  nilai yang sama. Contohnya:

```javascript
let x = 10;
let y = 5;
let result = x == y; // result akan bernilai false

let name1 = "John";
let name2 = "Doe";
let result2 = name1 == name2; // result2 akan bernilai false
```

- Tidak sama dengan (`!=`): Digunakan untuk membandingkan apakah dua nilai tidak
  memiliki nilai yang sama. Contohnya:

```javascript
let x = 10;
let y = 5;
let result = x != y; // result akan bernilai true

let name1 = "John";
let name2 = "Doe";
let result2 = name1 != name2; // result2 akan bernilai true
```

- Lebih besar dari (`>`), kurang dari (`<`), lebih besar sama dengan (`>=`), dan
  kurang sama dengan (`<=`): Digunakan untuk membandingkan apakah satu nilai
  lebih besar, kurang, atau sama dengan nilai yang lain. Contohnya:

```javascript
let x = 10;
let y = 5;
let result1 = x > y; // result1 akan bernilai true
let result2 = x < y; // result2 akan bernilai false
let result3 = x >= y; // result3 akan bernilai true
let result4 = x <= y; // result4 akan bernilai false
```

Identitas (`===` dan `!==`): Digunakan untuk membandingkan apakah dua nilai sama
baik dari segi nilai maupun tipe data-nya. Contohnya:

```javascript
let x = 10;
let y = "10";
let result1 = x === y; // result1 akan bernilai false
let result2 = x !== y; // result2 akan bernilai true
```

Operator perbandingan ini dapat digunakan dalam pengambilan keputusan (if, else,
dan sebagainya) dan loop untuk menjalankan kode berdasarkan kondisi yang
diberikan.

[⬆️ Back to Top](#table-of-contents)

---

### Operator Logika

Di dalam JavaScript, operator logika digunakan untuk mengkombinasikan dua atau
lebih nilai boolean untuk membentuk ekspresi logika yang lebih kompleks.
Operator logika akan mengembalikan nilai boolean (true atau false) tergantung
pada apakah ekspresi logika tersebut benar atau salah. Berikut adalah beberapa
contoh operator logika yang dapat digunakan di dalam JavaScript:

- And (`&&`): Digunakan untuk memeriksa apakah dua ekspresi logika benar. Jika
  kedua ekspresi logika bernilai true, maka operator ini akan mengembalikan
  true. Contohnya:

```javascript
let x = 10;
let y = 5;
let result = x > 5 && y < 10; // result akan bernilai true
```

- Or (`||`): Digunakan untuk memeriksa apakah setidaknya satu dari dua ekspresi
  logika benar. Jika salah satu atau kedua ekspresi logika bernilai true, maka
  operator ini akan mengembalikan true. Contohnya:

```javascript
let x = 10;
let y = 5;
let result = x > 5 || y > 10; // result akan bernilai true
```

- Not (`!`): Digunakan untuk membalikkan nilai ekspresi logika. Jika ekspresi
  logika bernilai true, maka operator ini akan mengembalikan false, dan
  sebaliknya. Contohnya:

```javascript
let x = 10;
let y = 5;
let result1 = !(x > 5); // result1 akan bernilai false
let result2 = !(y > 10); // result2 akan bernilai true
```

Operator logika ini sering digunakan dalam pengambilan keputusan (if, else, dan
sebagainya) untuk menjalankan kode berdasarkan kondisi yang diberikan. Selain
itu, operator logika juga dapat digunakan bersama dengan operator perbandingan
untuk membentuk ekspresi logika yang lebih kompleks.
[⬆️ Back to Top](#table-of-contents)

---

### Console

Console pada JavaScript adalah sebuah alat untuk memantau dan menguji kode
JavaScript. Console dapat digunakan untuk menampilkan pesan, objek, atau nilai
variabel ke dalam console yang terletak pada browser atau lingkungan
pengembangan. Biasanya, penggunaan console digunakan dalam proses debugging atau
pengujian kode.

Di dalam JavaScript, console dapat diakses melalui objek global `console`.
Beberapa metode yang sering digunakan pada console antara lain:

- `log()`: digunakan untuk menampilkan pesan atau nilai variabel ke dalam
  console. Contohnya:

```javascript
console.log("Hello World!"); // Menampilkan pesan 'Hello World!' ke dalam console
let x = 10;
console.log(x); // Menampilkan nilai variabel x (10) ke dalam console
```

- `error()`: digunakan untuk menampilkan pesan error ke dalam console.
  Contohnya:

```javascript
console.error("Terjadi kesalahan!"); // Menampilkan pesan error 'Terjadi kesalahan!' ke dalam console
```

- `warn()`: digunakan untuk menampilkan pesan peringatan ke dalam console.
  Contohnya:

```javascript
console.warn("Harap perhatikan!"); // Menampilkan pesan peringatan 'Harap perhatikan!' ke dalam console
```

Selain itu, terdapat juga beberapa metode lain pada console yang dapat digunakan
seperti info(), clear(), table(), dan lain-lain. Console dapat sangat berguna
dalam proses pengembangan JavaScript karena dapat membantu pengembang menemukan
dan memperbaiki bug serta menguji kode yang telah dibuat.

[⬆️ Back to Top](#table-of-contents)

---

### String Template

String template atau dikenal juga sebagai template literal adalah fitur pada
JavaScript yang memungkinkan untuk menggabungkan string dengan ekspresi
JavaScript secara efisien dan mudah dibaca. String template ditandai dengan
penggunaan backtick (` `` `) sebagai pembatas string dan di dalamnya dapat
dimasukkan variabel atau ekspresi JavaScript yang diapit oleh tanda kurung
kurawal (`{ }`).

Contoh penggunaan string template:

```javascript
let name = "John";
let age = 30;
let message = `Hi, my name is ${name} and I am ${age} years old.`;

console.log(message); // Output: Hi, my name is John and I am 30 years old.
```

Pada contoh di atas, variabel `name` dan `age` dimasukkan ke dalam string
template menggunakan notasi `${}`. Dengan menggunakan string template,
penggunaan operator `+` untuk menggabungkan string dan variabel tidak perlu
dilakukan lagi, sehingga membuat kode lebih efisien dan mudah dibaca. Selain
itu, string template juga memungkinkan penggunaan fitur-fitur seperti line
break, escape sequence, dan lain-lain secara lebih mudah dan intuitif.

Penggunaan string template sering digunakan pada framework atau library
JavaScript modern seperti React, Vue, atau Angular untuk membangun tampilan
aplikasi yang dinamis dan kompleks.

[⬆️ Back to Top](#table-of-contents)

---

### Konversi String dan Number

Konversi atau mengubah tipe data dari string ke number, atau sebaliknya, dapat
dilakukan pada JavaScript dengan menggunakan beberapa metode yang disediakan
oleh bahasa tersebut.

1. Konversi dari string ke number

Untuk mengubah tipe data string ke number, kita dapat menggunakan metode
`parseInt()` atau `parseFloat()`. Perbedaannya adalah `parseInt()` digunakan
untuk mengubah string menjadi bilangan bulat (integer), sedangkan `parseFloat()`
digunakan untuk mengubah string menjadi bilangan desimal (float).

Contoh penggunaan `parseInt()`:

```javascript
let strNumber = "10";
let intNumber = parseInt(strNumber);

console.log(intNumber); // Output: 10
console.log(typeof intNumber); // Output: number
```

Contoh penggunaan `parseFloat()`:

```javascript
let strFloat = "3.14";
let floatNumber = parseFloat(strFloat);

console.log(floatNumber); // Output: 3.14
console.log(typeof floatNumber); // Output: number
```

2. Konversi dari number ke string

Untuk mengubah tipe data number ke string, kita dapat menggunakan metode
`toString()`. Metode ini akan mengubah bilangan menjadi string.

Contoh penggunaan `toString()`:

```javascript
let number = 42;
let strNumber = number.toString();

console.log(strNumber); // Output: '42'
console.log(typeof strNumber); // Output: string
```

Perlu diperhatikan bahwa ketika mengubah tipe data dari string ke number atau
sebaliknya, akan terjadi pengubahan format tampilan dan dapat menyebabkan
perubahan pada nilai atau hasil operasi matematika yang dilakukan. Oleh karena
itu, perlu dilakukan dengan hati-hati dan memastikan format data yang benar.

[⬆️ Back to Top](#table-of-contents)

---

### Tipe Data Array

Array adalah salah satu tipe data pada JavaScript yang dapat digunakan untuk
menyimpan kumpulan data dalam satu variabel. Setiap data dalam array
diidentifikasi oleh indeks yang dimulai dari nol (0). Dalam JavaScript, array
dapat berisi berbagai tipe data seperti angka, string, boolean, bahkan objek dan
array lainnya.

Untuk membuat array pada JavaScript, kita dapat menggunakan tanda kurung siku
(`[]`) dan memasukkan setiap data ke dalamnya, dipisahkan dengan tanda koma.
Sebagai contoh:

```javascript
let myArray = [10, "hello", true, [1, 2, 3]];
```

Pada contoh di atas, variabel `myArray` berisi kumpulan data seperti angka
(`10`), string (`'hello'`), boolean (`true`), dan array (`[1, 2, 3]`). Setiap
data tersebut memiliki indeks yang dapat diakses dengan cara memanggil nama
variabel dan indeksnya dalam tanda kurung siku. Sebagai contoh:

```javascript
console.log(myArray[0]); // Output: 10
console.log(myArray[1]); // Output: 'hello'
console.log(myArray[2]); // Output: true
console.log(myArray[3]); // Output: [1, 2, 3]
console.log(myArray[3][1]); // Output: 2
```

Pada contoh di atas, kita dapat mengakses setiap data pada array dengan
memanggil nama variabel dan indeksnya, seperti `myArray[0]` untuk mengakses data
dengan indeks 0 (angka 10), `myArray[1]` untuk mengakses data dengan indeks 1
('hello'), dan seterusnya. Kita juga dapat mengakses data pada array yang berupa
array lain dengan memanggil nama variabel dan indeksnya secara berulang, seperti
`myArray[3][1]` untuk mengakses data pada indeks 1 pada array yang ada di dalam
array.

Dalam penggunaannya, array sering digunakan untuk menyimpan data yang banyak,
seperti data pengguna pada sebuah aplikasi, data transaksi pada sebuah toko
online, dan sebagainya. Array juga dapat dimanipulasi dengan berbagai metode
yang disediakan oleh JavaScript seperti `push()`, `pop()`, `shift()`,
`unshift()`, `splice()`, dan lain-lain.

[⬆️ Back to Top](#table-of-contents)

---

### Tipe Data Object

Objek adalah salah satu tipe data kompleks pada JavaScript yang memungkinkan
kita untuk menyimpan kumpulan data dengan properti dan nilai yang terkait.
Setiap properti pada objek memiliki nama dan nilai, dan dapat diakses dengan
menggunakan sintaks titik (.) atau tanda kurung siku (`[]`).

Untuk membuat objek pada JavaScript, kita dapat menggunakan tanda kurung kurawal
(`{}`) dan menambahkan properti-properti beserta nilai-nilainya ke dalam objek
tersebut. Contohnya seperti berikut:

```javascript
let myObject = {
	name: "John",
	age: 25,
	isMarried: false,
	hobbies: ["reading", "playing games"],
};
```

Pada contoh di atas, kita membuat variabel `myObject` yang berisi objek dengan
properti-properti seperti `name`, `age`, `isMarried`, dan `hobbies`. Setiap
properti pada objek tersebut memiliki nilai yang terkait seperti `'John'`, `25`,
`false`, dan `['reading', 'playing games']`.

Untuk mengakses properti pada objek, kita dapat menggunakan sintaks titik (`.`)
atau tanda kurung siku (`[]`). Contohnya seperti berikut:

```javascript
console.log(myObject.name); // Output: 'John'
console.log(myObject["age"]); // Output: 25
console.log(myObject.hobbies[0]); // Output: 'reading'
```

Pada contoh di atas, kita mengakses properti `name` pada objek `myObject` dengan
sintaks titik (`.`), dan properti `age` serta `hobbies` dengan sintaks tanda
kurung siku (`[]`). Kita juga dapat mengakses data yang berada di dalam array
yang ada di dalam objek dengan menggunakan sintaks tanda kurung siku dan indeks.

Objek pada JavaScript sering digunakan untuk menyimpan data yang kompleks dan
terstruktur, seperti data pengguna, data produk pada sebuah toko online, dan
lain-lain. Objek juga dapat dimanipulasi dengan berbagai metode yang disediakan
oleh JavaScript seperti `Object.keys()`, `Object.values()`, `Object.entries()`,
dan lain-lain.

[⬆️ Back to Top](#table-of-contents)

---

### If Expressions

`if` expression adalah struktur kontrol pada JavaScript yang digunakan untuk
mengeksekusi satu blok kode jika kondisi yang diberikan bernilai `true`.
Struktur `if` expression terdiri dari kata kunci `if`, kondisi yang dievaluasi,
dan satu blok kode yang dieksekusi jika kondisi tersebut bernilai `true`.

Contohnya seperti berikut:

```javascript
let number = 10;

if (number > 5) {
	console.log("Number is greater than 5");
}
```

Pada contoh di atas, kita memeriksa apakah variabel `number` lebih besar dari 5
atau tidak. Jika kondisinya benar (nilai variabel `number` lebih besar dari 5),
maka blok kode yang berada di dalam struktur `if` expression (console.log) akan
dieksekusi.

Kita juga dapat menambahkan blok kode yang akan dieksekusi jika kondisi pada
struktur `if` expression bernilai `false` dengan menggunakan struktur `else`
seperti berikut:

```javascript
let number = 2;

if (number > 5) {
	console.log("Number is greater than 5");
} else {
	console.log("Number is not greater than 5");
}
```

Pada contoh di atas, karena nilai variabel `number` kurang dari 5, maka blok
kode yang berada di dalam struktur `else` (console.log) yang akan dieksekusi.

Kita juga dapat menambahkan beberapa kondisi yang akan dievaluasi dengan
menggunakan struktur `else if`. Contohnya seperti berikut:

```javascript
let number = 7;

if (number > 10) {
	console.log("Number is greater than 10");
} else if (number > 5) {
	console.log("Number is greater than 5");
} else {
	console.log("Number is less than or equal to 5");
}
```

Pada contoh di atas, kita menambahkan dua kondisi dengan menggunakan struktur
`else if`. Jika kondisi pertama (nilai variabel `number` lebih besar dari 10)
bernilai `false`, maka JavaScript akan mengevaluasi kondisi kedua (nilai
variabel `number` lebih besar dari 5). Jika kondisi kedua bernilai `false`, maka
blok kode yang berada di dalam struktur `else` (console.log) akan dieksekusi.

[⬆️ Back to Top](#table-of-contents)

---

### Popup

Popup atau pop-up adalah sebuah jendela kecil yang muncul secara otomatis di
atas halaman web yang sedang ditampilkan. Popup sering digunakan untuk
menampilkan informasi tambahan atau pesan kepada pengguna.

Di JavaScript, kita dapat membuat popup menggunakan method `alert()`,
`confirm()`, atau `prompt()`.

- `alert()` digunakan untuk menampilkan pesan pada popup tanpa meminta tanggapan
  dari pengguna. Popup akan menampilkan satu tombol OK, yang jika ditekan, popup
  akan ditutup.

Contohnya seperti berikut:

```javascript
alert("Ini adalah pesan pada popup");
```

- `confirm()` digunakan untuk meminta pengguna untuk menanggapi sebuah
  pertanyaan pada popup. Popup akan menampilkan dua tombol, OK dan Cancel. Jika
  pengguna menekan tombol OK, maka nilai yang dikembalikan adalah `true`,
  sedangkan jika pengguna menekan tombol Cancel, nilai yang dikembalikan adalah
  `false`.

Contohnya seperti berikut:

```javascript
let result = confirm("Apakah kamu yakin ingin melanjutkan?");

if (result === true) {
	console.log("Pengguna menekan tombol OK");
} else {
	console.log("Pengguna menekan tombol Cancel");
}
```

- `prompt()` digunakan untuk meminta pengguna untuk memasukkan sebuah nilai pada
  popup. Popup akan menampilkan sebuah kotak input untuk memasukkan nilai. Jika
  pengguna menekan tombol OK setelah memasukkan nilai, maka nilai tersebut akan
  dikembalikan sebagai string, sedangkan jika pengguna menekan tombol Cancel,
  nilai yang dikembalikan adalah `null`.

Contohnya seperti berikut:

```javascript
let name = prompt("Masukkan nama kamu:");

if (name != null) {
	console.log("Halo, " + name);
} else {
	console.log("Pengguna menekan tombol Cancel");
}
```

Namun, karena popup dapat mengganggu pengalaman pengguna pada situs web, maka
penggunaan popup sebaiknya dibatasi dan hanya digunakan pada kasus yang memang
memerlukan penggunaan popup.

[⬆️ Back to Top](#table-of-contents)

---

### Undefined

`undefined` adalah sebuah nilai yang menunjukkan bahwa sebuah variabel belum
diberi nilai atau tidak terdefinisi. Dalam JavaScript, ketika sebuah variabel
dideklarasikan tetapi tidak diinisialisasi dengan nilai apapun, maka nilai dari
variabel tersebut akan menjadi `undefined`.

Contoh penggunaan variabel yang belum didefinisikan:

```javascript
let x;
console.log(x); // output: undefined
```

Selain itu, nilai `undefined` juga akan dikembalikan ketika kita mencoba
mengakses properti atau indeks pada sebuah objek atau array yang tidak ada.

Contoh penggunaan pada objek:

```javascript
let person = {
	name: "John",
	age: 30,
};
console.log(person.address); // output: undefined
```

Contoh penggunaan pada array:

```javascript
let fruits = ["apple", "banana", "orange"];
console.log(fruits[3]); // output: undefined
```

Dalam kasus tertentu, penggunaan nilai `undefined` bisa dianggap sebagai sebuah
kesalahan atau bug pada program kita. Oleh karena itu, sebaiknya kita memeriksa
apakah sebuah variabel telah diberi nilai sebelum menggunakannya dalam program
kita.

[⬆️ Back to Top](#table-of-contents)

---

### Null

`null` adalah sebuah nilai khusus dalam JavaScript yang menunjukkan ketiadaan
nilai atau nilai kosong. Secara eksplisit, kita dapat memberikan nilai `null`
pada sebuah variabel untuk menunjukkan bahwa variabel tersebut tidak memiliki
nilai atau tidak menunjuk pada objek apapun.

Perbedaan antara `undefined` dan `null` adalah bahwa undefined menunjukkan bahwa
sebuah variabel belum diberi nilai atau tidak terdefinisi, sedangkan `null`
menunjukkan bahwa sebuah variabel memiliki nilai yang sengaja diberikan sebagai
"kosong" atau "tidak ada".

Contoh penggunaan `null` pada variabel:

```javascript
let x = null;
console.log(x); // output: null
```

Kita juga bisa menggunakan operator `===` untuk membandingkan nilai `null`.
Perlu diingat bahwa `null` adalah sebuah nilai, sehingga harus dibandingkan
dengan operator perbandingan, bukan dengan operator identitas.

Contoh penggunaan operator `===`:

```javascript
let x = null;
console.log(x === null); // output: true
console.log(x === undefined); // output: false
```

Dalam beberapa kasus, penggunaan `null` dapat digunakan untuk memperjelas niat
dari sebuah variabel atau untuk menunjukkan bahwa sebuah objek tidak memiliki
nilai tertentu. Namun, sebaiknya kita memastikan bahwa penggunaan `null` tidak
menimbulkan ambiguitas dalam program kita.

[⬆️ Back to Top](#table-of-contents)

---

### Switch Expression

`switch` adalah sebuah statement dalam JavaScript yang digunakan untuk
mengevaluasi sebuah ekspresi dan membandingkannya dengan beberapa nilai yang
telah ditentukan. Jika nilai dari ekspresi tersebut cocok dengan salah satu
nilai yang telah ditentukan, maka blok kode terkait dengan nilai tersebut akan
dijalankan.

Contoh penggunaan `switch`:

```javascript
let day = 3;
switch (day) {
	case 1:
		console.log("Monday");
		break;
	case 2:
		console.log("Tuesday");
		break;
	case 3:
		console.log("Wednesday");
		break;
	case 4:
		console.log("Thursday");
		break;
	case 5:
		console.log("Friday");
		break;
	default:
		console.log("Weekend");
		break;
}
```

Pada contoh di atas, kita menggunakan `switch` untuk mengevaluasi nilai dari
variabel `day`. Jika nilai `day` sama dengan 1, maka blok kode terkait dengan
`case 1` akan dijalankan. Jika nilai `day` sama dengan 2, maka blok kode terkait
dengan `case 2` akan dijalankan, dan seterusnya. Jika tidak ada nilai yang cocok
dengan nilai dari day, maka blok kode terkait dengan `default` akan dijalankan.

Perlu diingat bahwa setiap blok kode dalam `switch` harus diakhiri dengan
`break`, agar program tidak melanjutkan eksekusi pada blok kode berikutnya. Jika
`break` tidak digunakan, maka semua blok kode di bawah blok kode yang cocok akan
dijalankan, sehingga dapat menyebabkan kesalahan dalam program kita.

[⬆️ Back to Top](#table-of-contents)

---

### Operator Typeof

`typeof` adalah sebuah operator dalam JavaScript yang digunakan untuk
mengembalikan jenis tipe data dari sebuah nilai. Operator `typeof` mengembalikan
sebuah string yang berisi jenis tipe data dari nilai yang diberikan.

Contoh penggunaan `typeof`:

```javascript
console.log(typeof "Hello World"); // output: string
console.log(typeof 42); // output: number
console.log(typeof true); // output: boolean
console.log(typeof undefined); // output: undefined
console.log(typeof null); // output: object
console.log(typeof [1, 2, 3]); // output: object
console.log(typeof { name: "John", age: 30 }); // output: object
console.log(typeof function () {}); // output: function
```

Pada contoh di atas, kita menggunakan `typeof` untuk mengetahui jenis tipe data
dari beberapa nilai yang berbeda, seperti string, number, boolean, undefined,
null, array, object, dan function. Ketika `typeof` digunakan untuk mengevaluasi
nilai yang memiliki tipe data `null`, maka nilai yang dikembalikan adalah
`object`. Ini adalah sebuah keanehan dalam JavaScript yang telah menjadi bagian
dari perilaku yang tidak dapat diubah pada bahasa ini.

Operator `typeof` sangat berguna dalam debugging dan pengecekan tipe data pada
variabel. Kita dapat menggunakan `typeof` untuk memastikan bahwa sebuah nilai
memiliki tipe data yang diharapkan sebelum memprosesnya dalam program kita.

[⬆️ Back to Top](#table-of-contents)

---

### Operator In

`in` adalah sebuah operator dalam JavaScript yang digunakan untuk memeriksa
apakah sebuah properti tertentu ada dalam sebuah objek. Operator `in`
mengembalikan nilai `true` jika properti yang dicari ada dalam objek, dan
`false` jika tidak.

Contoh penggunaan `in`:

```javascript
let person = { name: "John", age: 30 };

console.log("name" in person); // output: true
console.log("age" in person); // output: true
console.log("email" in person); // output: false
```

Pada contoh di atas, kita menggunakan `in` untuk memeriksa apakah properti
"name", "age", dan "email" ada dalam objek `person`. Hasilnya, properti "name"
dan "age" ditemukan dalam objek, sehingga mengembalikan nilai `true`, sedangkan
properti "email" tidak ditemukan, sehingga mengembalikan nilai `false`.

Operator `in` sangat berguna dalam memeriksa keberadaan properti dalam objek
sebelum melakukan operasi pada properti tersebut. Kita dapat menggunakan `in`
untuk memeriksa keberadaan properti sebelum mengaksesnya, sehingga dapat
mencegah kesalahan dalam program kita.

[⬆️ Back to Top](#table-of-contents)

---

### Ternary Operator

Ternary operator, juga dikenal sebagai operator kondisional, adalah operator
dalam JavaScript yang memungkinkan kita untuk menulis kode yang lebih singkat
dan ekspresif untuk menggantikan kondisi `if..else`. Ternary operator terdiri
dari tiga bagian: kondisi, nilai ketika kondisi benar, dan nilai ketika kondisi
salah.

Contoh penggunaan ternary operator:

```javascript
let age = 20;
let status = age >= 18 ? "dewasa" : "anak-anak";

console.log(status); // output: "dewasa"
```

Pada contoh di atas, kita menggunakan ternary operator untuk memeriksa apakah
`age` lebih besar dari atau sama dengan 18. Jika kondisi benar, maka variabel
`status` akan diset ke nilai "dewasa", dan jika tidak, maka variabel `status`
akan diset ke nilai "anak-anak".

Ternary operator sangat berguna ketika kita ingin mengevaluasi sebuah kondisi
dan mengembalikan nilai berdasarkan hasil evaluasi kondisi tersebut. Kita dapat
menggunakan ternary operator untuk menggantikan blok `if..else` yang sederhana
dan menulis kode yang lebih singkat dan mudah dibaca.

[⬆️ Back to Top](#table-of-contents)

---

### Nullisth Coalesting Operator

Nullish Coalescing Operator (`??`) adalah operator dalam JavaScript yang
memungkinkan kita untuk memeriksa nilai yang "falsy" (nilai yang dianggap
sebagai `false` dalam kondisi boolean, seperti `false`, `null`, `undefined`,
`0`, `NaN`, atau `"..."`) dan mengembalikan nilai alternatif ketika nilai yang
diperiksa adalah "falsy".

Contoh penggunaan Nullish Coalescing Operator:

```javascript
let username = "";
let defaultUsername = "guest";

let result = username ?? defaultUsername;
console.log(result); // output: "guest"
```

Pada contoh di atas, kita menggunakan Nullish Coalescing Operator (`??`) untuk
memeriksa nilai `username`. Karena `username` adalah string kosong (`"..."`)
yang dianggap "falsy", maka operator `??` akan mengembalikan nilai
`defaultUsername` ("guest") sebagai nilai alternatif.

Nullish Coalescing Operator sangat berguna ketika kita ingin mengambil nilai
dari sebuah variabel atau objek tetapi nilai tersebut tidak selalu tersedia atau
bernilai "falsy". Dengan menggunakan Nullish Coalescing Operator, kita dapat
memastikan bahwa nilai yang digunakan tidak akan bernilai "falsy" dan memastikan
bahwa nilai alternatif yang diberikan benar-benar memiliki nilai yang
diinginkan.

---

### Optional Chaining

Optional chaining (`?.`) adalah fitur baru dalam JavaScript yang memungkinkan
kita untuk mengakses properti dan metode dari sebuah objek tanpa harus memeriksa
apakah objek tersebut `null` atau `undefined` terlebih dahulu.

Contoh penggunaan Optional chaining:

```javascript
let user = {
	name: "John",
	address: {
		city: "New York",
		zipCode: "12345",
	},
};

let zipCode = user.address?.zipCode;

console.log(zipCode); // output: "12345"
```

Pada contoh di atas, kita menggunakan Optional chaining (`?.`) untuk mengakses
properti `zipCode` dari objek `user.address`. Jika `user.address` adalah `null`
atau `undefined`, maka operator `?.` akan mengembalikan nilai `undefined` dan
tidak akan terjadi kesalahan.

Optional chaining sangat berguna ketika kita ingin mengakses properti dan metode
dari objek yang mungkin memiliki nilai null atau `undefined`. Dengan menggunakan
Optional chaining, kita dapat menulis kode yang lebih singkat dan mudah dibaca
tanpa harus menambahkan banyak kondisi untuk memeriksa apakah objek tersebut
memiliki nilai atau tidak.

[⬆️ Back to Top](#table-of-contents)

---

### Falsy and Truthy

Falsy dan Truthy adalah konsep dalam JavaScript yang mengacu pada nilai-nilai
yang dianggap `false` atau `true` dalam konteks boolean.

Nilai-nilai yang dianggap sebagai Falsy (false) adalah:

- `false`
- `0`
- `"..."` (string kosong)
- `null`
- `undefined`
- `NaN`

Sedangkan nilai-nilai yang dianggap sebagai Truthy (true) adalah:

- `t`rue`
- Semua angka selain dari 0, seperti `1`, `2`, `3`, dsb.
- Semua string yang bukan string kosong, seperti `"hello"`, `"world"`, dsb.
- Objek (termasuk array dan fungsi)
- Nilai `Infinity` dan `-Infinity`

Ketika kita menggunakan nilai-nilai ini dalam kondisi boolean, seperti dalam
pernyataan `if` atau operator logika, nilai-nilai yang dianggap falsy akan
dinilai `false`, sedangkan nilai-nilai yang dianggap truthy akan dinilai `true`.

Contoh penggunaan Falsy dan Truthy:

```javascript
let x = 0;

if (x) {
	console.log("x is truthy");
} else {
	console.log("x is falsy");
}
// output: "x is falsy"
```

Pada contoh di atas, nilai `x` adalah `0`, yang dianggap falsy. Oleh karena itu,
ketika kita menggunakan nilai `x` dalam kondisi boolean, pernyataan `if` akan
mengevaluasi `false` dan kode di dalam blok `else` akan dijalankan.

Pengetahuan tentang nilai Falsy dan Truthy sangat penting dalam pemrograman
JavaScript karena kita dapat menggunakannya untuk mengevaluasi kondisi dan
melakukan kontrol aliran program yang berbeda-beda tergantung pada nilai yang
diterima.

[⬆️ Back to Top](#table-of-contents)

---

### Operator Logika di Non Boolean

Operator logika di non-boolean mengacu pada konsep di mana operator logika `&&`,
`||`, dan `!` dapat diterapkan pada nilai-nilai non-boolean seperti string,
angka, atau objek.

Dalam konteks operator logika di non-boolean, nilai non-boolean akan dianggap
sebagai truthy atau falsy. Nilai yang dianggap sebagai falsy akan dinilai
sebagai `false`, sedangkan nilai yang dianggap sebagai truthy akan dinilai
sebagai `true`.

Operator logika `&&` dan `||` pada nilai non-boolean mengembalikan nilai asli
dari salah satu operand yang memenuhi kondisi. Jika operand pertama dalam
operator `&&` dianggap falsy, nilai asli operand pertama dikembalikan. Namun,
jika operand pertama dianggap truthy, nilai asli operand kedua dikembalikan.
Sebaliknya, jika operand pertama dalam operator `||` dianggap truthy, nilai asli
operand pertama dikembalikan. Namun, jika operand pertama dianggap falsy, nilai
asli operand kedua dikembalikan.

Contoh penggunaan operator logika di non-boolean:

```javascript
let x = "hello";
let y = "";

let result1 = x && y;
console.log(result1); // output: ""

let result2 = x || y;
console.log(result2); // output: "hello"
```

Pada contoh di atas, kita menggunakan operator `&&` dan `||` pada nilai
non-boolean `x` dan `y`, yang adalah string kosong dan string "hello". Karena
`x` dianggap truthy dan `y` dianggap falsy, nilai asli dari `y` dikembalikan
dalam operator `&&` dan nilai asli dari `x` dikembalikan dalam operator `||`.

Operator logika `!` pada nilai non-boolean mengembalikan nilai boolean yang
mengevaluasi ke `true` jika nilai asli dari operand dianggap falsy dan `false`
jika nilai asli dari operand dianggap truthy.

Contoh penggunaan operator `!` pada nilai non-boolean:

```javascript
let x = "hello";

if (!x) {
	console.log("x is falsy");
} else {
	console.log("x is truthy");
}
// output: "x is truthy"
```

Pada contoh di atas, operator `!` digunakan untuk mengevaluasi nilai non-boolean
`x`. Karena `x` dianggap truthy, operator `!` mengembalikan nilai boolean
`false`, sehingga blok `else` dijalankan.

[⬆️ Back to Top](#table-of-contents)

---

### For Loop

For loop adalah struktur kontrol pada bahasa pemrograman yang digunakan untuk
melakukan pengulangan atau iterasi sejumlah tertentu dalam sebuah blok kode. For
loop terdiri dari tiga bagian: inisialisasi, kondisi, dan ekspresi peningkatan.

Format dasar for loop adalah sebagai berikut:

```javascript
for (inisialisasi; kondisi; ekspresi peningkatan) {
  // blok kode yang akan diulang
}
```

Ketiga bagian for loop adalah:

1. Inisialisasi: di mana variabel penghitung atau variabel iterasi
   dideklarasikan dan diinisialisasi dengan nilai awal. Bagian ini hanya
   dieksekusi satu kali, pada awal loop.
2. Kondisi: di mana kondisi yang diuji untuk setiap iterasi ditempatkan. Selama
   kondisi ini terpenuhi atau benar, blok kode dalam for loop akan dijalankan.
   Jika kondisi ini salah atau tidak terpenuhi, loop akan dihentikan.
3. Ekspresi peningkatan: di mana nilai variabel penghitung ditingkatkan atau
   dikurangi pada setiap iterasi. Ekspresi peningkatan dieksekusi setiap kali
   blok kode dalam loop selesai dieksekusi.

Contoh penggunaan for loop:

```javascript
for (let i = 1; i <= 5; i++) {
	console.log("Angka " + i);
}
```

Pada contoh di atas, for loop digunakan untuk mencetak angka 1 hingga 5 pada
konsol. Variabel penghitung `i` dideklarasikan dan diinisialisasi dengan nilai 1
pada inisialisasi, kondisi diuji untuk setiap iterasi untuk memastikan nilai `i`
kurang dari atau sama dengan 5, dan ekspresi peningkatan menambahkan nilai `i`
sebesar 1 pada setiap iterasi.

Output dari contoh di atas adalah:

```bash
Angka 1
Angka 2
Angka 3
Angka 4
Angka 5
```

[⬆️ Back to Top](#table-of-contents)

---

### While Loop

While loop adalah struktur kontrol pada bahasa pemrograman yang digunakan untuk
melakukan iterasi atau pengulangan selama kondisi yang diberikan terpenuhi.
Kondisi yang diberikan pada while loop harus mengembalikan nilai boolean, true
atau false.

Format dasar while loop adalah sebagai berikut:

```javascript
while (kondisi) {
	// blok kode yang akan diulang
}
```

Blok kode dalam while loop akan terus diulang selama kondisi yang diberikan
terpenuhi atau menghasilkan nilai true. Kondisi akan dievaluasi pada awal setiap
iterasi sebelum blok kode dieksekusi. Jika kondisi menghasilkan false, maka loop
akan berhenti dan eksekusi kode dilanjutkan dari pernyataan setelah while loop.

Contoh penggunaan while loop:

```javascript
let i = 1;

while (i <= 5) {
	console.log("Angka " + i);
	i++;
}
```

Pada contoh di atas, while loop digunakan untuk mencetak angka 1 hingga 5 pada
konsol. Variabel `i` dideklarasikan dan diinisialisasi dengan nilai 1 di luar
while loop, dan kondisi diberikan pada while loop untuk memastikan nilai `i`
kurang dari atau sama dengan 5. Blok kode dalam while loop mencetak nilai `i`
pada konsol dan nilai `i` ditingkatkan sebesar 1 pada setiap iterasi menggunakan
`i++`.

Output dari contoh di atas adalah:

```
Angka 1
Angka 2
Angka 3
Angka 4
Angka 5
```

[⬆️ Back to Top](#table-of-contents)

---

### Do While Loop

Do-while loop adalah struktur kontrol pada bahasa pemrograman yang digunakan
untuk melakukan pengulangan atau iterasi pada sebuah blok kode, setidaknya satu
kali terlepas dari kondisi yang diberikan. Setelah itu, pengulangan akan
dilanjutkan selama kondisi yang diberikan terpenuhi atau mengembalikan nilai
`true`.

```javascript
do {
	// blok kode yang akan diulang
} while (kondisi);
```

Blok kode dalam do-while loop akan dieksekusi setidaknya satu kali sebelum
kondisi dievaluasi. Jika kondisi menghasilkan `true`, maka blok kode akan terus
dieksekusi dan pengulangan akan dilanjutkan. Jika kondisi menghasilkan `false`,
maka pengulangan berhenti dan eksekusi kode dilanjutkan dari pernyataan setelah
do-while loop.

Contoh penggunaan do-while loop:

Format dasar do-while loop adalah sebagai berikut:

```javascript
let i = 1;

do {
	console.log("Angka " + i);
	i++;
} while (i <= 5);
```

Pada contoh di atas, do-while loop digunakan untuk mencetak angka 1 hingga 5
pada konsol. Variabel `i` dideklarasikan dan diinisialisasi dengan nilai 1 di
luar do-while loop, dan blok kode dalam do-while loop mencetak nilai `i` pada
konsol dan nilai `i` ditingkatkan sebesar 1 pada setiap iterasi menggunakan
`i++`. Kondisi diberikan pada akhir do-while loop untuk memastikan bahwa
pengulangan dilakukan selama nilai `i` kurang dari atau sama dengan 5.

Output dari contoh di atas adalah:

```bash
Angka 1
Angka 2
Angka 3
Angka 4
Angka 5
```

[⬆️ Back to Top](#table-of-contents)

---

### Break and Continue

`break` dan `continue` adalah pernyataan yang digunakan pada loop di JavaScript
untuk mengontrol aliran program.

`break` digunakan untuk menghentikan eksekusi loop ketika kondisi tertentu
terpenuhi. Pernyataan `break` dapat digunakan di dalam loop for, while, atau
do-while. Ketika pernyataan `break` dijalankan, loop akan dihentikan dan
eksekusi program dilanjutkan pada baris kode setelah loop. Contoh penggunaan
`break` pada loop:

```javascript
for (let i = 1; i <= 10; i++) {
	if (i === 6) {
		break;
	}
	console.log(i);
}
```

Pada contoh di atas, loop for akan berjalan dari `i` sama dengan 1 hingga 10.
Pada setiap iterasi, program akan mengevaluasi apakah nilai `i` sama dengan 6.
Jika nilai `i` sama dengan 6, program akan keluar dari loop menggunakan
pernyataan `break`, dan eksekusi program akan dilanjutkan pada baris kode
setelah loop. Jika nilai `i` tidak sama dengan 6, program akan mencetak nilai
`i` pada konsol menggunakan pernyataan `console.log`.

`continue` digunakan untuk melompati satu iterasi pada loop ketika kondisi
tertentu terpenuhi. Pernyataan `continue` juga dapat digunakan di dalam loop
for, while, atau do-while. Ketika pernyataan `continue` dijalankan, loop akan
melanjutkan ke iterasi berikutnya tanpa mengeksekusi baris kode yang berada di
bawah pernyataan `continue`. Contoh penggunaan `continue` pada loop:

```javascript
for (let i = 1; i <= 10; i++) {
	if (i % 2 === 0) {
		continue;
	}
	console.log(i);
}
```

Pada contoh di atas, loop for akan berjalan dari `i` sama dengan 1 hingga 10.
Pada setiap iterasi, program akan mengevaluasi apakah nilai `i` adalah bilangan
genap dengan menggunakan operasi modulo (`%`). Jika nilai `i` adalah bilangan
genap, program akan melanjutkan ke iterasi berikutnya menggunakan pernyataan
`continue`, dan baris kode di bawah pernyataan `continue` tidak akan dieksekusi.
Jika nilai `i` adalah bilangan ganjil, program akan mencetak nilai `i` pada
konsol menggunakan pernyataan `console.log`.

[⬆️ Back to Top](#table-of-contents)

---

### Label

Label adalah sebuah identifier (penanda) yang digunakan untuk memberikan label
pada sebuah statement di dalam program JavaScript. Label biasanya digunakan
bersama dengan statement `break` atau `continue` untuk memberikan kontrol pada
loop atau statement yang lebih kompleks.

Berikut adalah contoh penggunaan label pada statement `break` dan loop `for`:

```javascript
outerloop: for (let i = 0; i < 5; i++) {
	innerloop: for (let j = 0; j < 5; j++) {
		if (j === 2) {
			break outerloop; // keluar dari loop for pada outerloop
		}
		console.log(`i = ${i}, j = ${j}`);
	}
}
```

Pada contoh di atas, label `outerloop` dan `innerloop` diberikan pada
masing-masing loop for. Kemudian, pada statement `break outerloop`, label
`outerloop` digunakan untuk memberikan kontrol pada loop for pada outerloop dan
keluar dari loop tersebut. Sehingga, ketika nilai `j` sama dengan 2, loop for
pada innerloop akan dihentikan dan langsung keluar dari loop for pada outerloop.

[⬆️ Back to Top](#table-of-contents)

---

### For in

`for...in` adalah sebuah perulangan yang digunakan untuk melakukan iterasi pada
properti-properti sebuah objek JavaScript. Perulangan ini akan mengulangi
seluruh properti yang ada pada sebuah objek, termasuk properti yang diwarisi
dari prototype chain-nya.

Berikut adalah contoh penggunaan perulangan `for...in` untuk melakukan iterasi
pada properti-properti sebuah objek:

```javascript
const myObject = { a: 1, b: 2, c: 3 };

for (const property in myObject) {
	console.log(`${property}: ${myObject[property]}`);
}
```

Pada contoh di atas, `for...in` digunakan untuk melakukan iterasi pada seluruh
properti yang ada pada objek `myObject`. Setiap properti akan diakses
menggunakan variabel `property` pada setiap iterasinya, kemudian nilai dari
properti tersebut akan dicetak ke konsol menggunakan notasi bracket `[]`.

Perlu diperhatikan, perulangan `for...in` tidak disarankan untuk digunakan pada
array, karena ia tidak menjamin urutan pengulangan sesuai dengan indeks array
dan juga akan mengiterasi seluruh properti pada objek, termasuk properti yang
didefinisikan di dalam prototype-nya. Untuk melakukan iterasi pada array,
sebaiknya menggunakan perulangan `for...of` atau `Array.forEach()`.

[⬆️ Back to Top](#table-of-contents)

---

### For Of

`for...of` adalah sebuah perulangan yang digunakan untuk melakukan iterasi pada
iterable objects seperti Array, String, Map, dan Set. Perulangan ini memudahkan
kita untuk mengakses setiap elemen atau value dari iterable object secara
berurutan.

Berikut adalah contoh penggunaan perulangan `for...of` untuk melakukan iterasi
pada setiap elemen dalam sebuah array:

```javascript
const myArray = ["apple", "banana", "orange"];

for (const value of myArray) {
	console.log(value);
}
```

Pada contoh di atas, `for...of` digunakan untuk mengakses setiap elemen pada
array `myArray`. Setiap elemen akan diakses menggunakan variabel `value` pada
setiap iterasinya, kemudian nilai dari elemen tersebut akan dicetak ke konsol.

Perlu diperhatikan, perulangan `for...of` hanya berfungsi pada iterable objects,
sehingga tidak dapat digunakan untuk melakukan iterasi pada objek JavaScript
yang bukan iterable.

[⬆️ Back to Top](#table-of-contents)

---

### With Statement

`with` adalah sebuah statement pada JavaScript yang digunakan untuk membuat
konteks lingkup baru (new lexical scope) dari sebuah objek. Konteks lingkup baru
tersebut memungkinkan kita untuk mengakses properti dan method dari objek
tersebut secara lebih singkat tanpa harus menuliskan nama objeknya
berulang-ulang.

Namun, penggunaan `with` dianggap sebagai best practice yang buruk dalam
pengembangan aplikasi karena dapat menimbulkan beberapa masalah seperti:

1. Meningkatkan kompleksitas kode.
2. Meningkatkan kemungkinan terjadinya kesalahan penulisan.
3. Memperlambat kinerja program.

Berikut adalah contoh penggunaan `with` statement:

```javascript
const myObj = {
	name: "John",
	age: 30,
	occupation: "Developer",
};

with (myObj) {
	console.log(name, age, occupation);
}
```

Pada contoh di atas, `with` statement digunakan untuk membuat konteks lingkup
baru dari objek `myObj`. Dalam konteks lingkup tersebut, kita dapat mengakses
properti dari objek tersebut secara lebih singkat hanya dengan menuliskan nama
propertinya saja.

Namun, seperti yang telah disebutkan sebelumnya, penggunaan `with` dianggap
sebagai best practice yang buruk dalam pengembangan aplikasi. Sebaiknya kita
menghindari penggunaan `with` statement dan lebih memilih untuk menuliskan nama
objeknya secara eksplisit untuk memperjelas kode.

[⬆️ Back to Top](#table-of-contents)

---

### Function

Function adalah sebuah blok kode yang terpisah dan dapat dipanggil atau
dieksekusi secara berulang dalam sebuah program. Fungsi dapat menerima input
atau parameter sebagai argumen, melakukan tindakan tertentu, dan mengembalikan
output.

Fungsi sangat penting dalam pemrograman karena memungkinkan kita untuk
mengorganisir dan mengelompokkan kode ke dalam bagian-bagian yang lebih kecil
dan terpisah, sehingga membuat kode lebih mudah dibaca, diubah, dan dikelola.

Berikut adalah contoh deklarasi fungsi:

```javascript
function tambah(a, b) {
	return a + b;
}
```

Pada contoh di atas, kita mendeklarasikan sebuah fungsi dengan nama `tambah`
yang menerima dua parameter `a` dan `b`. Fungsi tersebut melakukan operasi
penjumlahan antara kedua parameter tersebut dan mengembalikan hasilnya
menggunakan kata kunci `return`.

Setelah kita mendefinisikan fungsi di atas, kita dapat memanggilnya dari tempat
lain dalam program, seperti ini:

```javascript
const hasilTambah = tambah(2, 3);
console.log(hasilTambah); // Output: 5
```

Pada contoh di atas, kita memanggil fungsi `tambah` dengan memberikan dua
argumen yaitu 2 dan 3. Fungsi tersebut akan mengembalikan hasil penjumlahan dari
kedua argumen tersebut, yaitu 5. Hasil tersebut kemudian disimpan dalam variabel
`hasilTambah` dan dicetak ke konsol menggunakan `console.log()`.

[⬆️ Back to Top](#table-of-contents)

---

### Function Parameter

Function parameter adalah variabel yang digunakan dalam deklarasi sebuah fungsi
untuk menerima input atau argumen dari luar dan digunakan dalam tubuh fungsi.
Parameter ini kemudian dapat diakses dan digunakan dalam tubuh fungsi untuk
melakukan tindakan tertentu atau mengembalikan output.

Berikut adalah contoh deklarasi fungsi dengan dua parameter:

```javascript
function tambah(a, b) {
	return a + b;
}
```

Pada contoh di atas, kita mendeklarasikan fungsi tambah yang menerima dua
parameter `a` dan `b`. Dalam tubuh fungsi, kita menggunakan kedua parameter
tersebut untuk melakukan operasi penjumlahan dan mengembalikan hasilnya
menggunakan kata kunci `return`.

Kita dapat memanggil fungsi `tambah` dengan memberikan dua argumen sebagai
input, seperti ini:

```javascript
const hasilTambah = tambah(2, 3);
console.log(hasilTambah); // Output: 5
```

Pada contoh di atas, kita memanggil fungsi `tambah` dengan memberikan dua
argumen yaitu 2 dan 3. Kedua argumen tersebut akan dijadikan nilai untuk
parameter `a` dan `b` dalam fungsi `tambah`. Fungsi tersebut akan mengembalikan
hasil penjumlahan dari kedua argumen tersebut, yaitu 5. Hasil tersebut kemudian
disimpan dalam variabel `hasilTambah` dan dicetak ke konsol menggunakan
`console.log()`.

[⬆️ Back to Top](#table-of-contents)

---

### Function Return Value

Function return value atau nilai kembalian dari fungsi adalah nilai yang
dikembalikan oleh sebuah fungsi setelah menjalankan operasinya. Nilai ini dapat
digunakan atau disimpan ke dalam variabel atau digunakan sebagai input bagi
operasi selanjutnya di dalam program.

Berikut adalah contoh deklarasi fungsi yang mengembalikan nilai:

```javascript
function tambah(a, b) {
	return a + b;
}
```

Pada contoh di atas, kita mendeklarasikan fungsi `tambah` yang menerima dua
parameter `a` dan `b`. Di dalam tubuh fungsi, kita menggunakan kedua parameter
tersebut untuk melakukan operasi penjumlahan menggunakan operator `+`. Setelah
itu, kita menggunakan kata kunci `return` untuk mengembalikan nilai hasil
penjumlahan tersebut.

Kita dapat memanggil fungsi `tambah` dan menyimpan nilai kembaliannya ke dalam
variabel, seperti ini:

```javascript
const hasilTambah = tambah(2, 3);
console.log(hasilTambah); // Output: 5
```

Pada contoh di atas, kita memanggil fungsi `tambah` dengan memberikan dua
argumen yaitu 2 dan 3. Fungsi tersebut akan mengembalikan hasil penjumlahan dari
kedua argumen tersebut, yaitu 5. Hasil tersebut kemudian disimpan dalam variabel
`hasilTambah` dan dicetak ke konsol menggunakan `console.log()`.

[⬆️ Back to Top](#table-of-contents)

---

### Optional Parameter

Optional parameter adalah parameter pada fungsi yang dapat diisi atau tidak
diisi saat memanggil fungsi. Parameter tersebut memiliki nilai default yang akan
digunakan jika parameter tidak diisi saat memanggil fungsi.

Berikut adalah contoh penggunaan optional parameter pada sebuah fungsi:

```javascript
function halo(nama = "Dunia") {
	console.log(`Halo, ${nama}!`);
}
```

Pada contoh di atas, kita mendefinisikan sebuah fungsi `halo` yang memiliki satu
parameter `nama`. Parameter ini memiliki nilai default yaitu `'Dunia'`, artinya
jika saat memanggil fungsi `halo` kita tidak memberikan argumen, maka nilai
`'Dunia'` akan digunakan.

Kita dapat memanggil fungsi `halo` dengan atau tanpa argumen, seperti ini:

```javascript
halo(); // Output: Halo, Dunia!
halo("Andi"); // Output: Halo, Andi!
```

Pada contoh di atas, saat memanggil fungsi `halo` tanpa argumen, maka nilai
default `'Dunia'` akan digunakan dan hasilnya adalah `'Halo, Dunia!'`. Sedangkan
saat memanggil fungsi `halo` dengan argumen `'Andi'`, maka nilai argumen
tersebut akan digunakan dan hasilnya adalah `'Halo, Andi!'`.

[⬆️ Back to Top](#table-of-contents)

---

### Default Parameter

Default parameter adalah nilai default yang diberikan pada parameter fungsi jika
nilai untuk parameter tersebut tidak diberikan atau diberikan nilai `undefined`
saat pemanggilan fungsi. Dengan adanya default parameter, kita tidak perlu
melakukan pengecekan apakah parameter sudah memiliki nilai atau tidak, karena
nilai default akan digunakan jika parameter tidak diberikan nilai.

Berikut adalah contoh penggunaan default parameter pada sebuah fungsi:

```javascript
function tambah(a, b = 0) {
	return a + b;
}
```

Pada contoh di atas, kita mendefinisikan sebuah fungsi tambah dengan dua
parameter yaitu `a` dan `b`. Parameter `b` memiliki nilai default yaitu `0`,
artinya jika saat memanggil fungsi `tambah` kita tidak memberikan argumen untuk
`b`, maka nilai `0` akan digunakan.

Kita dapat memanggil fungsi `tambah` dengan atau tanpa memberikan argumen untuk
`b`, seperti ini:

```javascript
tambah(2); // Output: 2
tambah(2, 3); // Output: 5
```

Pada contoh di atas, saat memanggil fungsi `tambah` dengan satu argumen yaitu
`2`, maka parameter `a` akan memiliki nilai `2` dan parameter `b` akan memiliki
nilai default yaitu `0`, sehingga hasilnya adalah `2`. Sedangkan saat memanggil
fungsi `tambah` dengan dua argumen yaitu `2` dan `3`, maka parameter `a` akan
memiliki nilai `2` dan parameter `b` akan memiliki nilai `3`, sehingga hasilnya
adalah `5`.

[⬆️ Back to Top](#table-of-contents)

---

### Rest Parameter

Rest Parameter adalah sebuah fitur di JavaScript yang memungkinkan kita untuk
mengambil beberapa argumen sebagai array, dengan menempatkan tiga titik `...`
sebelum nama parameter dalam definisi fungsi.

Contoh penggunaan Rest Parameter adalah sebagai berikut:

```javascript
function myFunction(a, b, ...rest) {
	console.log("a = " + a);
	console.log("b = " + b);
	console.log("rest = " + rest);
}

myFunction(1, 2, 3, 4, 5);
```

Output dari kode di atas akan menjadi:

```bash
a = 1
b = 2
rest = 3,4,5
```

Dalam contoh di atas, `a` dan `b` adalah dua parameter pertama yang diberikan ke
fungsi `myFunction()`, sedangkan `...rest` mengambil sisa parameter sebagai
array dengan nama `rest`. Dalam contoh ini, nilai `rest` akan menjadi `3, 4, 5`.
Kita dapat menggunakan `rest` array di dalam fungsi untuk melakukan tindakan
tertentu, seperti mengambil jumlah elemen dalam array atau melakukan operasi
lainnya.

[⬆️ Back to Top](#table-of-contents)

---

### Function Sebagai Value

Dalam JavaScript, sebuah function dapat dianggap sebagai value yang dapat
disimpan ke dalam variabel atau dapat diteruskan sebagai argumen ke dalam fungsi
lain. Konsep ini dikenal sebagai first-class functions, yang artinya function
diperlakukan seperti tipe data lainnya.

Sebagai contoh, kita dapat menyimpan sebuah fungsi ke dalam sebuah variabel dan
memanggil fungsi tersebut nanti seperti berikut:

```javascript
const myFunction = function () {
	console.log("Hello World!");
};

myFunction(); // Output: "Hello World!"
```

Dalam contoh di atas, kita menyimpan fungsi anonim (tanpa nama) ke dalam
variabel `myFunction`, dan kemudian memanggil fungsi tersebut dengan menggunakan
`myFunction()`.

Kita juga dapat meneruskan sebuah fungsi sebagai argumen ke dalam fungsi lain,
seperti dalam contoh berikut:

```javascript
function myFunction(callback) {
	callback();
}

myFunction(function () {
	console.log("Hello World!");
});
```

Dalam contoh di atas, kita meneruskan sebuah fungsi anonim sebagai argumen ke
dalam fungsi `myFunction`. Fungsi `myFunction` kemudian memanggil fungsi yang
diteruskan sebagai argumen dan mengeluarkan output "Hello World!". Dalam hal
ini, kita menggunakan fungsi sebagai callback untuk melakukan tindakan tertentu
dalam fungsi lainnya.

[⬆️ Back to Top](#table-of-contents)

---

### Anonymous Function

Anonymous function adalah sebuah fungsi tanpa nama yang didefinisikan secara
langsung di dalam ekspresi atau statement yang lebih besar, biasanya sebagai
argumen ke fungsi lain atau dalam penggunaan teknik seperti IIFE (Immediately
Invoked Function Expression).

Contoh penggunaan anonymous function dalam argumen fungsi:

```javascript
setTimeout(function () {
	console.log("Hello world!");
}, 1000);
```

Contoh penggunaan anonymous function dalam IIFE:

```javascript
(function () {
	// kode di sini
})();
```

Dalam contoh-contoh tersebut, fungsi tidak memiliki nama dan tidak didefinisikan
terpisah, melainkan langsung digunakan sebagai argumen fungsi atau dieksekusi
secara langsung sebagai bagian dari ekspresi.

[⬆️ Back to Top](#table-of-contents)

---

### Function dalam Function

Function dalam function, juga dikenal sebagai nested function atau inner
function, adalah fungsi yang didefinisikan di dalam fungsi lain. Dalam
JavaScript, fungsi dapat didefinisikan di mana saja di dalam scope (lingkup)
fungsi induk, termasuk di dalam blok fungsi lain.

Contoh penggunaan function dalam function:

```javascript
function hitung(x, y) {
	function kali(a, b) {
		return a * b;
	}

	function tambah(a, b) {
		return a + b;
	}

	var hasilKali = kali(x, y);
	var hasilTambah = tambah(x, y);

	return hasilKali + hasilTambah;
}

var hasil = hitung(2, 3);
console.log(hasil); // Output: 11
```

Dalam contoh ini, fungsi `kali` dan `tambah` didefinisikan di dalam fungsi
`hitung`. Kedua fungsi tersebut hanya dapat diakses dari dalam fungsi `hitung`,
sehingga mereka tidak dapat dipanggil atau diakses dari luar fungsi `hitung`.
Fungsi `kali` dan `tambah` digunakan untuk menghitung nilai hasil `kali` dan
hasil `tambah` dari dua parameter `x` dan `y`, dan kemudian hasil keduanya
dijumlahkan dan dikembalikan sebagai hasil dari fungsi `hitung`.

[⬆️ Back to Top](#table-of-contents)

---

### Scope

Scope dalam pemrograman mengacu pada daerah kode tempat variabel dan fungsi
dapat diakses. Pada JavaScript, terdapat dua jenis scope, yaitu global scope dan
local scope.

Global scope mencakup semua variabel dan fungsi yang didefinisikan di luar dari
semua blok dan fungsi, dan dapat diakses dari mana saja dalam program.

Local scope terdiri dari variabel dan fungsi yang didefinisikan di dalam blok
atau fungsi tertentu. Variabel dan fungsi yang didefinisikan dalam local scope
hanya dapat diakses di dalam blok atau fungsi tempat mereka didefinisikan.

Pada JavaScript, variabel yang dideklarasikan tanpa var, let, atau const akan
secara otomatis menjadi variabel global, dan dapat diakses dari mana saja dalam
program. Oleh karena itu, disarankan untuk selalu mendeklarasikan variabel
menggunakan var, let, atau const agar variabel dapat berada dalam local scope
dan tidak menyebabkan konflik atau masalah dengan variabel global.

```javascript
let a = 10; // global variable

function multiply(b) {
	let a = 5; // local variable
	return a * b; // returns 5 times b
}

console.log(multiply(2)); // Output: 10
console.log(a); // Output: 10
```

Dalam contoh ini, variabel `a` memiliki scope global, sehingga dapat diakses di
dalam maupun di luar fungsi `multiply`. Sedangkan variabel `b` dan `a` yang
didefinisikan di dalam fungsi `multiply` memiliki scope lokal, yang hanya dapat
diakses di dalam fungsi tersebut. Oleh karena itu, pada saat fungsi `multiply`
dipanggil dengan argumen `2`, maka hasil yang dikembalikan adalah `5 * 2 = 10`,
dan nilai variabel `a` di luar fungsi tetap `10`.

[⬆️ Back to Top](#table-of-contents)

---

### Recursive Function

Recursive function adalah sebuah fungsi yang memanggil dirinya sendiri secara
terus-menerus hingga mencapai kondisi keluar. Recursive function biasanya
digunakan ketika penyelesaian sebuah masalah memerlukan pemanggilan fungsi
secara berulang-ulang hingga suatu kondisi terpenuhi.

Berikut adalah contoh sederhana dari recursive function yang menghitung
faktorial dari sebuah bilangan:

```javascript
function factorial(n) {
	if (n <= 1) {
		return 1;
	} else {
		return n * factorial(n - 1);
	}
}

console.log(factorial(5)); // Output: 120
```

Pada contoh di atas, fungsi `factorial` menerima satu parameter `n` yang
merupakan bilangan yang akan dihitung faktorialnya. Fungsi ini menggunakan
kondisi `if` untuk mengecek apakah `n` lebih kecil atau sama dengan 1. Jika iya,
maka fungsi akan mengembalikan nilai 1 karena faktorial dari bilangan 0 atau 1
adalah 1.

Jika kondisi `if` tidak terpenuhi, maka fungsi akan memanggil dirinya sendiri
dengan parameter `n - 1` untuk menghitung faktorial dari bilangan yang lebih
kecil dari `n`. Proses ini akan terus berulang hingga `n` sama dengan 1 atau 0,
dan akhirnya fungsi akan mengembalikan hasil perkalian dari semua bilangan yang
diproses sebelumnya.

[⬆️ Back to Top](#table-of-contents)

---

### Function Generator

Function Generator adalah sebuah fitur dalam JavaScript yang memungkinkan kita
untuk membuat fungsi yang dapat menghasilkan multiple nilai pada waktu yang
berbeda. Fitur ini diperkenalkan pada ECMAScript 2015 (ES6) dan menghasilkan
nilai berulang yang dapat dikonsumsi dengan menggunakan loop.

Sebuah Function Generator menggunakan kata kunci `function` untuk menandakan
bahwa ia adalah generator function. Selain itu, untuk menghasilkan nilai
generator function menggunakan kata kunci `yield`.

Berikut adalah contoh sederhana penggunaan function generator:

```javascript
function* count() {
	let i = 0;
	while (true) {
		yield i++;
	}
}

const counter = count();
console.log(counter.next().value); // 0
console.log(counter.next().value); // 1
console.log(counter.next().value); // 2
```

Pada contoh di atas, `count()` adalah generator function yang menghasilkan
sebuah `counter` object. Ketika kita memanggil `counter.next()`, ia akan
mengembalikan object yang berisi dua properti yaitu `value` dan `done`. `value`
adalah nilai yang dihasilkan oleh generator function, sedangkan `done` adalah
sebuah boolean yang menandakan apakah generator sudah selesai menghasilkan nilai
atau belum.

[⬆️ Back to Top](#table-of-contents)

---

### Arrow Function

Arrow function adalah cara baru untuk menulis function dalam JavaScript dengan
sintaks yang lebih ringkas dan mudah dibaca. Arrow function memiliki beberapa
kelebihan, yaitu lebih pendek, lebih mudah dibaca, dan tidak perlu menuliskan
kata kunci `function`.

Sintaks dari arrow function adalah sebagai berikut:

```javascript
(parameter1, parameter2, ...) => {
  // kode function
};

```

Contoh penggunaan arrow function:

```javascript
// function biasa
function multiply(x, y) {
	return x * y;
}

// arrow function
const multiply = (x, y) => x * y;
```

Perlu diingat bahwa arrow function tidak memiliki `this` yang ditentukan secara
dinamis seperti pada function biasa. Oleh karena itu, pada arrow function,
`this` memiliki nilai yang sama seperti pada konteks yang mengelilinginya.

[⬆️ Back to Top](#table-of-contents)

---

### Closure

Closure adalah kemampuan dalam JavaScript untuk mengakses variabel yang berada di dalam scope yang sama dengan function, meskipun function tersebut telah dijalankan atau keluar dari scope-nya. Closure dapat memungkinkan function untuk "mengingat" nilai variabel pada waktu pembuatan function, dan mengakses nilai tersebut pada waktu eksekusi function, bahkan jika function itu dipanggil di lingkup yang berbeda.

Closure biasanya terjadi ketika sebuah function di-deklarasikan di dalam function lain, sehingga function tersebut memiliki akses ke variabel lokal di dalam function yang lebih besar. Hal ini membuat code lebih fleksibel dan mudah dipelihara, karena variabel yang digunakan di dalam function hanya dapat diakses oleh function itu sendiri dan tidak dapat diakses dari luar.

Contoh penggunaan closure:

```javascript
function outer() {
  let count = 0;

  function inner() {
    count++;
    console.log(count);
  }

  return inner;
}

let closureFunc = outer(); // closureFunc adalah function inner yang memiliki akses ke variabel count di dalam function outer

closureFunc(); // output: 1
closureFunc(); // output: 2
closureFunc(); // output: 3
```

Pada contoh di atas, function `inner` adalah closure function karena memiliki akses ke variabel `count` yang berada di dalam function `outer`. Ketika function `outer` dipanggil, ia mengembalikan function `inner`. Variabel `closureFunc` kemudian menampung function `inner` yang dikembalikan oleh function `outer`. Ketika `closureFunc` dipanggil, variabel `count` akan bertambah dan menghasilkan output yang sesuai. Karena `closureFunc` memiliki akses ke variabel `count`, ia dapat melacak nilai `count` pada setiap pemanggilan function.

[⬆️ Back to Top](#table-of-contents)

---

### Object Method

Object Method adalah sebuah fungsi yang terkait dengan sebuah objek dalam bahasa pemrograman JavaScript. Dalam konteks objek, sebuah method biasanya digunakan untuk melakukan operasi pada data yang terkait dengan objek tersebut.

Untuk mendefinisikan sebuah method pada objek, kita dapat menambahkan sebuah properti yang memiliki nilai berupa sebuah fungsi. Properti tersebut kemudian dapat dipanggil seperti sebuah fungsi dan akan melakukan operasi tertentu pada objek.

Contoh sederhana:

```javascript
const person = {
  name: "John",
  age: 30,
  greet: function() {
    console.log(`Hello, my name is ${this.name} and I'm ${this.age} years old.`);
  }
};

person.greet(); // Output: "Hello, my name is John and I'm 30 years old."
```

Pada contoh di atas, kita mendefinisikan sebuah objek `person` dengan tiga properti: `name`, `age`, dan `greet`. Properti `greet` adalah sebuah method yang digunakan untuk mengeluarkan pesan sapaan dengan menggunakan properti `name` dan `age` dari objek `person`.

Kemudian, kita memanggil method `greet` pada objek `person` dengan menggunakan sintaks `person.greet()`. Output dari program tersebut adalah pesan sapaan yang dihasilkan oleh method `greet`.

[⬆️ Back to Top](#table-of-contents)

---

### Kata Kunci This

`this` merupakan kata kunci yang digunakan untuk mengacu pada objek yang sedang menjadi konteks saat ini dalam kode JavaScript. Dalam setiap fungsi yang dijalankan, nilai `this` akan mengacu pada objek yang menjadi "owner" dari fungsi tersebut.

Nilai `this` akan berbeda-beda tergantung dari bagaimana dan di mana sebuah fungsi dipanggil. Dalam lingkup global, `this` akan mengacu pada objek `window`, sedangkan dalam fungsi di dalam objek, `this` akan mengacu pada objek itu sendiri.

Dalam beberapa kasus, nilai `this` bisa diubah dengan menggunakan metode seperti `call()`, `apply()`, atau `bind()`. Metode-metode tersebut digunakan untuk menetapkan nilai `this` yang baru untuk fungsi yang sedang dijalankan.

Pemahaman yang baik tentang kata kunci `this` sangat penting dalam pemrograman JavaScript karena banyak kerangka kerja dan library yang bergantung pada pemahaman tentang bagaimana nilai `this` bekerja.

Berikut ini adalah contoh kode yang mengilustrasikan penggunaan kata kunci `this` di dalam sebuah method pada objek:

```javascript
const person = {
  name: "John",
  age: 30,
  greeting: function() {
    console.log("Hello, my name is " + this.name + " and I am " + this.age + " years old.");
  }
};

person.greeting(); // Output: Hello, my name is John and I am 30 years old.
```

Dalam contoh kode di atas, kita membuat sebuah objek `person` yang memiliki dua properti yaitu `name` dan `age`, serta satu method yaitu `greeting`. Method `greeting` berfungsi untuk mencetak pesan sapaan dengan menggunakan nilai dari properti `name` dan `age` pada objek `person`. Di dalam method `greeting`, kita menggunakan kata kunci `this` untuk merujuk pada objek `person` sehingga nilai dari properti `name` dan `age` dapat diakses.

[⬆️ Back to Top](#table-of-contents)

---

### Arrow Function di Object

Arrow function di objek dapat digunakan sebagai method, yang memungkinkan penggunaan kata kunci `this` untuk mengacu pada objek yang bersangkutan. Dalam arrow function, `this` merujuk pada nilai `this` dari lingkup di mana arrow function itu sendiri dibuat, dan bukan objek yang memanggilnya. Ini memudahkan penulisan kode yang lebih ringkas dan mudah dibaca.

Contoh kode:

```javascript
const obj = {
  name: "John",
  age: 30,
  sayHello: () => {
    console.log(`Hello, my name is ${this.name}.`);
  },
  sayAge: function() {
    console.log(`I am ${this.age} years old.`);
  }
};

obj.sayHello(); // Output: "Hello, my name is undefined."
obj.sayAge(); // Output: "I am 30 years old."
```

Pada contoh kode di atas, `sayHello()` adalah arrow function yang mencoba mencetak `this.name`, tetapi karena `this` merujuk pada lingkup global, `name` tidak terdefinisi. Di sisi lain, `sayAge()` adalah method reguler yang menggunakan `this` untuk mengakses properti `age` dari objek `obj`.

[⬆️ Back to Top](#table-of-contents)

---

### Getter dan Setter

Getter dan setter adalah metode untuk mengakses atau mengubah nilai dari properti objek. Getter digunakan untuk mendapatkan nilai dari properti objek, sedangkan setter digunakan untuk mengubah nilai dari properti objek.

Getter ditentukan dengan menggunakan kata kunci `get`, diikuti dengan nama metode, dan diakhiri dengan sepasang tanda kurung kurawal `{}` yang berisi kode untuk mengembalikan nilai properti yang diinginkan.

Contoh penggunaan getter pada objek `person` untuk mengambil nilai dari properti `name`:

```javascript
const person = {
  firstName: "John",
  lastName: "Doe",
  get name() {
    return this.firstName + " " + this.lastName;
  }
};

console.log(person.name); // Output: "John Doe"
```

Setter ditentukan dengan menggunakan kata kunci `set`, diikuti dengan nama metode, dan diakhiri dengan sepasang tanda kurung kurawal `{}` yang berisi kode untuk mengubah nilai properti yang diinginkan.

Contoh penggunaan setter pada objek `person` untuk mengubah nilai dari properti `firstName` dan `lastName`:

```javascript
const person = {
  firstName: "John",
  lastName: "Doe",
  set name(name) {
    const parts = name.split(" ");
    this.firstName = parts[0];
    this.lastName = parts[1];
  }
};

person.name = "Jane Smith";
console.log(person.firstName); // Output: "Jane"
console.log(person.lastName); // Output: "Smith"
```

[⬆️ Back to Top](#table-of-contents)

---

### Masalah Variable Var

Sebelum ES6 (ECMAScript 2015) diperkenalkan, satu-satunya kata kunci untuk mendeklarasikan variabel di JavaScript adalah `var`. Namun, `var` memiliki masalah yang dapat menyebabkan perilaku yang tidak terduga dalam kode.

Salah satu masalah utama dengan `var` adalah hoisting. Ini berarti bahwa ketika variabel dideklarasikan dengan `var`, mereka akan diangkat (dipindahkan) ke atas lingkup fungsi atau file JavaScript, bahkan sebelum variabel dideklarasikan. Akibatnya, jika sebuah variabel dipanggil sebelum dideklarasikan, itu tidak akan menghasilkan kesalahan, tetapi nilai variabel akan menjadi `undefined`.

Contoh:

```javascript
console.log(x); // Output: undefined
var x = 10;
```

Hal ini terjadi karena deklarasi `var x = 10` diangkat ke atas, sehingga ketika `console.log(x)` dieksekusi, `x` dikenali sebagai variabel yang telah dideklarasikan, meskipun nilai sebenarnya belum ditetapkan.

Selain itu, `var` juga memiliki cakupan yang salah dan memungkinkan perubahan nilai yang tidak disengaja. Variabel yang dideklarasikan dengan `var` dapat diakses dari dalam dan luar fungsi atau blok kode. Jika variabel dideklarasikan dengan `var` di dalam blok kode (seperti if statement atau loop), variabel tetap tersedia di luar blok itu dan dapat dengan mudah diubah tanpa disadari.

Untuk mengatasi masalah ini, ES6 memperkenalkan dua kata kunci deklarasi variabel lainnya: `let` dan `const`. Keduanya memiliki cakupan yang lebih baik dan tidak memiliki masalah hoisting seperti `var`.

[⬆️ Back to Top](#table-of-contents)

---

### Destructuring

Destructuring adalah sebuah fitur pada JavaScript yang memungkinkan kita untuk memecah struktur data seperti array atau objek menjadi variabel-variabel yang terpisah dan mandiri. Dengan destructuring, kita dapat mengambil nilai dari objek atau array dan menggunakannya dalam variabel terpisah dengan lebih mudah dan cepat.

Untuk array, destructuring memungkinkan kita untuk mengambil nilai-nilai dalam array dan menyimpannya ke dalam variabel-variabel terpisah. Contohnya:

```javascript
const numbers = [1, 2, 3];
const [a, b, c] = numbers;

console.log(a); // Output: 1
console.log(b); // Output: 2
console.log(c); // Output: 3
```

Sedangkan untuk objek, destructuring memungkinkan kita untuk mengambil nilai-nilai dalam objek dan menyimpannya ke dalam variabel-variabel terpisah dengan nama yang sama dengan properti objek tersebut. Contohnya:

```javascript
const person = { name: 'John Doe', age: 30 };
const { name, age } = person;

console.log(name); // Output: John Doe
console.log(age); // Output: 30
```

Kita juga dapat menggunakan alias untuk memberi nama variabel yang berbeda dengan nama properti objek. Contohnya:

```javascript
const person = { name: 'John Doe', age: 30 };
const { name: personName, age: personAge } = person;

console.log(personName); // Output: John Doe
console.log(personAge); // Output: 30
```

[⬆️ Back to Top](#table-of-contents)

---

### Strict Mode

Strict mode adalah sebuah fitur pada JavaScript yang memungkinkan kode untuk dijalankan dalam mode yang lebih ketat. Mode ini akan memaksa developer untuk menulis kode JavaScript yang lebih aman dan memperbaiki beberapa masalah umum yang ada pada JavaScript. Beberapa hal yang terdapat pada strict mode antara lain:

1. Menghilangkan akses ke variabel global secara tidak sengaja.
2. Melarang penggunaan variabel tanpa deklarasi.
3. Menghilangkan penggunaan beberapa sintaksis yang sebenarnya valid, namun sebaiknya dihindari.
4. Melarang penggunaan kata kunci yang sebenarnya valid, namun akan menjadi reserved keyword di masa depan.
5. Membuat beberapa kesalahan yang sebelumnya dibiarkan lewat menjadi error, seperti penggunaan `delete` pada variabel atau fungsi.

Strict mode dapat diaktifkan pada seluruh file JavaScript dengan menambahkan string `"use strict";` pada bagian atas file. Mode ini juga dapat diaktifkan pada fungsi tertentu dengan menambahkan string `"use strict";` pada awal fungsi tersebut.

Contoh penggunaan Strict Mode pada JavaScript:

```javascript
'use strict';

function myFunction() {
  x = 3.14; // menyebabkan ReferenceError karena variabel x tidak dideklarasikan
}
myFunction();
```

Pada contoh di atas, strict mode digunakan dengan menambahkan `'use strict';` pada baris pertama fungsi `myFunction()`. Hal ini akan mengakibatkan variabel `x` yang tidak dideklarasikan di dalam fungsi tersebut akan menyebabkan error saat dijalankan. Tanpa strict mode, variabel `x` akan secara otomatis ditambahkan ke dalam lingkup global.

[⬆️ Back to Top](#table-of-contents)

---

### Debugger

Debugger adalah sebuah alat atau fitur yang tersedia di banyak lingkungan pengembangan perangkat lunak (IDE atau browser), yang memungkinkan pengembang untuk memeriksa, memecah dan memperbaiki kode dengan lebih mudah. Debugger memungkinkan pengembang untuk melihat perubahan nilai variabel, memeriksa fungsi dan jalur eksekusi, serta menangkap dan menampilkan kesalahan pada saat runtime. Debugger adalah alat yang sangat berguna dalam pengembangan perangkat lunak karena dapat membantu pengembang memecahkan masalah dan memperbaiki bug dengan lebih cepat dan efisien.

[⬆️ Back to Top](#table-of-contents)

---

# Footer

<a name="footnote1">1</a>: Cheatsheet adalah sebuah lembaran yang berisi kumpulan informasi penting dan ringkas terkait dengan suatu topik atau bahasa pemrograman tertentu. Cheatsheet biasanya digunakan oleh programmer untuk memudahkan dalam mengingat atau mencari syntax dan aturan tertentu saat mengembangkan sebuah program. Cheatsheet juga dapat digunakan sebagai bahan referensi yang dapat diakses dengan mudah dan cepat ketika diperlukan.
