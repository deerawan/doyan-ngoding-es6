# Destructuring

Destructuring merupakan salah satu pattern yg keren di ES6 karena bisa membuat kode jadi lebih mudah dibaca. Kita bisa menggunakan destructuring untuk Array dan juga Object. Tujuan dari destructuring adalah untuk memudahkan kita dalam mendapatkan elemen yang ada dalam Array atau Object.

## Array Destructuring

Destructuring dapat kita gunakan pada Array. Namun sebelum sampai kesana, kita lihat contoh bagaimana kita mendapatkan elemen dalam Array.

```javascript
const cars = ['toyota kijang', 'honda jazz', 'suzuki ertiga'];

const toyota = cars[0];
const honda = cars[1];
const suzuki = cars[2];

// toyota = 'toyota kijang'
// honda = 'honda jazz'
// suzuki = 'suzuki ertiga'
```

Untuk mendapatkan ketiga elemen dalam Array diatas, kita menggunakan index 0 hingga 2 pada Array `cars`. Nothing wrong with this way, but we can do better in ES6 dengan destructuring seperti pada contoh dibawah.

```javascript
const cars = ['toyota kijang', 'honda jazz', 'suzuki ertiga'];

const [toyota, honda, suzuki] = cars;

// toyota = 'toyota kijang'
// honda = 'honda jazz'
// suzuki = 'suzuki ertiga'
```

Terlihat bahwa kita menggunakan pattern square bracket `[...]` untuk mendapatkan tiap elemen dari array `cars`. Tiap elemen tersebut akan di-assign ke masing-masing variabel `toyota`, `honda`, dan `suzuki` sesuai urutannya pada array `cars`. Kalau kita bandingkan dengan sebelumnya menggunakan index, destructuring lebih clean dan readable.

Bagaimana jika kita menambahkan satu variabel lagi yaitu `mercedes`di destructuring seperti kode dibawah ini, apa nilai dari `mercedes`?

```javascript
const [toyota, honda, suzuki, mercedes] = cars;

// mercedes = undefined
```

`mercedes` akan bernilai `undefined` karena memang elemen ke-empat dari array `cars` tidak ada.

### Default Value

Kita bisa memberikan default value saat melakukan destructuring. Seperti contoh sebelumnya, kita bisa memberikan default value pada variable `mercedes` jika nilainya tidak ada. Instead kita mendapatkan nilai `undefined`, kita mendapatkan default value yang kita definisikan. 

```javascript
const [toyota, honda, suzuki, mercedes = 'mercedes xls'] = cars;

// mercedes = 'mercedes xls'
```







