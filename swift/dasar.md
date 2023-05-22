# Dasar

## Variabel

Variabel adalah sebuah objek yang berfungsi untuk menyimpan sebuah nilai atau data. Bayangkan sebuah kotak kemudian Anda beri label sesuai dengan apa yang akan diisi di kotak tersebut kemudian Anda isi kotak tersebut dengan benda atau barang sesuai dengan label yang tertera.

Contoh, Anda memiliki sebuah toples dengan label camilan kemudian Anda isi dengan keripik kentang. Apabila kita menulis kode dari contoh tersebut, beginilah kodenya:

```swift
var camilan = "keripik kentang"
```

1. Gunakan kata kunci `var` untuk membuat sebuah variabel.
2. Tulis nama variabel sesuai dengan nilai yang akan disimpan, yaitu `camilan`.
3. Berikan nilai untuk variabel setelah tanda sama dengan. Dalam hal ini kita memberikan nilai dengan sebuah teks `"keripik kentang"`.

Jika kita ingin mengganti nilai dari variabel yang sudah kita buat, misalkan mengganti keripik kentang dengan kacang almond. Maka kodenya adalah sebagai berikut:

```swift
camilan = "kacang almond"
```

Ya, kita **tidak** perlu menulis kembali kata kunci `var` dan langsung menuliskan nama variabel kemudian memberi nilai baru yaitu `"kacang almond"`.

```swift
var camilan = "keripik kentang"

camilan = "keripik singkong"

print(camilan)

camilan = "kacang atom"

print(camilan)
```

Kode di atas akan menampilkan nilai dari `camilan` di konsol jika dijalankan yaitu `keripik singkong` dan `kacang atom` Hal ini disebabkan oleh fungsi `print()` yang berfungsi menampilkan nilai yang kita masukkan di antara tanda kurung ke konsol. Konsol tidak dapat dilihat oleh pengguna aplikasi dan hanya bisa dilihat lewat IDE atau Terminal. Coba tulis kode tersebut di SwiftFiddle dan tekan tombol **Run**.

Kita menulis kode yang akan dijalankan di panel sebelah kiri dan setelah menekan tombol **Run** hasilnya akan muncul di panel sebelah kanan. Tampilan konsol kurang lebih mirip dengan panel sebelah kanan.

<figure><img src="../.gitbook/assets/Jepretan Layar 2023-05-20 pukul 9.41.56 AM.png" alt=""><figcaption><p>Menampilkan hasil SwiftFiddle</p></figcaption></figure>

## Konstanta

Tidak semua hal yang akan kita proses harus bisa diganti nilainya. Contohnya jika kita akan menghitung luas lingkaran yang menggunakan rumus pi dikali jari-jari kuadrat. Nilai pi adalah tetap dan tidak boleh berubah. Untuk membuat konstanta, kita menggunakan kata kunci `let`.

```swift
let pi = 3.14
var jariJari = 1.0
var luasLingkaran = pi * jariJari * jariJari

print(luasLingkaran)
```

Jika kita berusaha untuk mengubah nilai dari sebuah konstanta, maka Swift tidak akan melanjutkan proses _build_ dan menampilkan pesan kesalahan di konsol. Cobalah menuliskan kode berikut di SwiftFiddle dan tekan tombol **Run**.

```swift
let pi = 3.14

// Kita coba ubah nilai pi
pi = 2.00

var jariJari = 1.0
var luasLingkaran = pi * jariJari * jariJari

print(luasLingkaran)
```

<figure><img src="../.gitbook/assets/Jepretan Layar 2023-05-20 pukul 9.40.14 AM.png" alt=""><figcaption><p>Pesan kesalahan saat mencoba mengubah nilai konstanta</p></figcaption></figure>

Dari gambar di atas, SwiftFiddle sudah memberikan peringatan bahwa terdapat kesalahan dari kode program kita yaitu dengan tanda garis gelombang warna merah di bawah `pi` dan blok merah di sebelah ujung kanan baris ke-empat.
