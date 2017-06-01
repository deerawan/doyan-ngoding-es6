# Destructuring

Destructuring merupakan salah satu pattern yg keren di ES6 karena bisa membuat kode jadi lebih mudah dibaca. Kita bisa menggunakan destructuring untuk Array dan juga Object. Tujuan dari destructuring adalah untuk memudahkan kita dalam mendapatkan elemen yang ada dalam Array atau Object. 

## Array Destructuring

Destructuring dapat kita gunakan pada Array. Namun sebelum sampai kesana, kita lihat contoh bagaimana kita mendapatkan elemen dalam Array. 

```javascript
const cars = ['toyota kijang', 'honda jazz', 'suzuki ertiga'];

const toyota = cars[0];
const honda = cars[1];
const suzuki = cars[2];
```

Untuk mendapatkan ketiga elemen dalam Array diatas, kita menggunakan index 0 hingga 2 pada Array `cars`. Nothing wrong with this way, but we can do better in ES6 dengan destructuring seperti pada contoh dibawah. 

```javascript
const cars = ['toyota kijang', 'honda jazz', 'suzuki ertiga'];

const [toyota, honda, suzuki] = cars;
```

Terlihat bahwa kita menggunakan pattern seperti saat kita membuat array dengan menggunakan square bracket `[...]` pada saat ingin mendapatkan element pada `cars`.  Kalau kita bandingkan, dengan menggunakan destructuring lebih clean dan readable. 

