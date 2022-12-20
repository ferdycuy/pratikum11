# Tugas Pertemuan 13

### Exception Handling
- Exception merupakan kesalahan (error) yang terjadi saat proses eksekusi program sedang berjalan,
  Kesalahan menyebabkan program berakhir dengan tidak normal.
### Handling
- bisa juga disebut Penanganan file, adalah bagian penting dari aplikasi apa pun.
### Assertion
- Assertion(pernyataan) adalah kewajaran program yang kalian bisa aktif/nonaktifkan saat selesai menjalankan program.
### The Assert Statement
- Saat menemukan pernyataan, Python mengevaluasi ekspresi yang menyertainya, yang mana semoga benar. Jika ekspresi salah, Python memunculkan pengecualian AssertionError.
   
   *Sintaks untuk pernyataan yaitu :*
   assert Expression[, Arguments]

   Jika pernyataan gagal, Python menggunakan ArgumentExpression ArgumentExpression sebagai argumen argumen untuk AssertionError AssertionError. Pengecualian       AssertionError Pengecualian AssertionError dapat ditangkap dan ditangani ditangani seperti pengecualian lainnya menggunakan try- kecuali pernyataan, tetapi jika dibiarkan, mereka akan menghentikan program dan menghasilkan backtrace.

##### Contoh

- Berikut adalah fungsi fungsi yang mengubah suhu dari derajat Kelvin menjadi derajat Fahrenheit.Karena nol derajat Kelvin dingin, fungsi fungsi menyimpannya jika melihat negatif negatif suhu.

![1](https://user-images.githubusercontent.com/115714443/208670023-f6a3c0ee-b02a-4d25-a264-4f135b1d346a.png)

### Menangani Pengecualian

- Jika kalian memiliki beberapa kode mencurigakan yang mungkin mengeluarkan pengecualian, kalian dapat mempertahankan program kalian, letakkan kode yang mencurigakan di *try: blok. Setelah coba: blok, sertakan pernyataan sertakan *except: statemen, diikuti oleh blok kode yang menangani masalah seanggun mungkin.

##### Contoh

- Contoh-contoh berikut ini membuka file, menulis konten file, dan keluar dengan aman karena ada tidak masalah

![2](https://user-images.githubusercontent.com/115714443/208671126-c244af12-ef97-4122-aaee-1c5f3567f475.png)

- Contoh ini mencoba membuka file yang kalian tidak memiliki izin menulis, sehingga membuat file pengecualian

![3](https://user-images.githubusercontent.com/115714443/208671963-2b1def64-de1e-47d2-b32f-a528733cf996.png)

### Fasal kecuali tanpa Pengecualian

kalian juga dapat menggunakan pernyataan exception tanpa exception yang didefinisikan sebagai berikut:

try: You do your operations here; ...................... except: If there is any exception, then execute this block. ...................... else: If there is no exception then execute this block.

### Klausa kecuali dengan Berbagai Pengecualian

Anda juga dapat menggunakan pernyataan exception yang sama untuk menangani beberapa exception sebagai berikut:

try: You do your operations here; ...................... except(Exception1[, Exception2[,...ExceptionN]]]): If there is any exception from the given exception list, then execute this block. ...................... else: If there is no exception then execute this block.

### Klausa coba-akhirnya

##### Contoh

- Jika Anda tidak memiliki izin untuk membuka file dalam mode tulis yang dapat ditulis, maka ini akan menghasilkan hasil berikut:

![4](https://user-images.githubusercontent.com/115714443/208673285-8a32a009-98c6-4d3d-af08-1bac931dd141.png)

- Contoh yang sama sebagai berikut:

![5](https://user-images.githubusercontent.com/115714443/208674311-96ab3487-35a0-465b-b106-5b7b71571600.png)

Ketika exception dilempar ke dalam blok try, eksekusi segera dilanjutkan ke akhir memblok. Setelah semua pernyataan di blok akhirnya dieksekusi, pengecualian dimunculkan lagi dan ditangani dalam pernyataan kecuali jika ada di lapisan berikutnya yang lebih tinggi dari percobaan-kecuali penyataan.

### Argumen Pengecualian

##### Contoh untuk satu pengecualian

![6](https://user-images.githubusercontent.com/115714443/208674540-737bd679-5a8f-442f-b24b-16afea54a8a1.png)

### Melempar Pengecualian
##### Contoh
Pengecualian dapat berupa string, kelas, atau objek. Sebagian besar pengecualian adalah pengecualian dari inti Python menimbulkan adalah kelas, dengan argumen=argumen yang merupakan turunan dari kelas. Mendefinisikan pengecualian barucukup mudah dan dapat dilakukan sebagai berikut:

![7](https://user-images.githubusercontent.com/115714443/208674733-30cf6a16-57fa-4cd1-8593-0dce85871c6f.png)

### Pengecualian yang Ditetapkan Pengguna

- Python juga memungkinkan kalian membuat pengecualian sendiri dengan menurunkan kelas-kelas dari yang standar pengecualian bawaan.
- Berikut adalah contoh yang terkait dengan RuntimeError.Kelas dibuat merupakan subkelas dari subkelas RuntimeError. Ini berguna saat kalian perlu menampilkan tampilan informasi yang lebih spesifik saat e pengecualian tertangkap.
- Di blok coba, pengecualian yang ditentukan pengguna dimunculkan dan ditangkap di blok kecuali. Itu variabel e digunakan untuk membuat instance dari kelas Networkerror.

![8](https://user-images.githubusercontent.com/115714443/208675196-a61d9151-e3b3-4b3b-ae98-d1654f45bbd9.png)
### TERIMAKASI ###
