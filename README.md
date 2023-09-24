# fomotoko

Task 1
Penjelasan:

- Kode pertama, header("Content-Type: application/json");, mengatur header HTTP untuk memberitahu klien bahwa konten yang dikirimkan dalam format JSON.

- Selanjutnya, saya mendefinisikan koneksi ke database dengan mengganti nilai variabel $host, $username, $password, dan $database sesuai dengan database.

- Kemudian, saya membuta endpoint create_order yang memproses permintaan POST. Ini memungkinkan pelanggan untuk membuat pesanan produk dengan memasukkan product_id dan quantity ke dalam permintaan.

- Dalam endpoint create_order, saya melakukan validasi stok produk untuk memastikan bahwa stok mencukupi sebelum membuat pesanan. Jika stok cukup, pesanan dibuat, dan stok produk dikurangi sesuai jumlah pesanan.

- Saya memberikan respons dalam format JSON dengan pesan "Pesanan berhasil dibuat." atau pesan kesalahan yang sesuai jika ada kesalahan dalam prosesnya.

- Terakhir, kita menutup koneksi database setelah selesai menggunakan database.



Task2

Penjelasan:

 1. HTML dan CSS:
    - Kode HTML digunakan untuk membuat struktur halaman web.
    - Saya menggunakan Bootstrap untuk mengatur tampilan tabel agar terlihat rapi.
    - CSS kustom digunakan untuk menentukan gaya visual elemen-elemen dalam tabel.
    
 2. Fungsi findPossibleItemLocations:
    - Fungsi ini digunakan untuk mencari koordinat yang mungkin untuk item yang harus ditemukan oleh pemain.
    - Ini memeriksa langkah-langkah yang diperlukan oleh pemain (atas, kanan, bawah) dan mengidentifikasi lokasi-lokasi yang mungkin sesuai dengan aturan permainan.
   
 3. Fungsi printGridWithPossibleItem:
    - Fungsi ini digunakan untuk mencetak grid permainan dalam bentuk tabel HTML.
    - Setiap sel dalam tabel diberi warna sesuai dengan jenisnya (rintangan, jalan yang jelas, posisi pemain, kemungkinan lokasi item).
    - Sel yang mungkin berisi item ditandai dengan simbol "$".

4. Variabel $grids:
    - Ini adalah array dari beberapa grid permainan yang berbeda yang akan ditampilkan.
    - Setiap grid direpresentasikan sebagai array string dengan karakter "#" untuk rintangan, "." untuk jalan yang jelas, dan "X" untuk posisi pemain.

5. Aturan Permainan:
    - Aturan permainan seperti jumlah langkah ke atas, ke kanan, dan ke bawah yang harus diikuti oleh pemain ditentukan sebagai variabel, yaitu $upSteps, $rightSteps, dan $downSteps.

6. Perulangan foreach untuk Setiap Grid:
    - Kode mencetak setiap grid permainan dari $grids.
    - Untuk setiap grid, posisi awal pemain dan lokasi item yang mungkin ditentukan.
    - Grid dicetak ke dalam tabel HTML menggunakan fungsi printGridWithPossibleItem.

7. Deskripsi Permainan:
    - Di bawah setiap tabel grid, terdapat deskripsi permainan yang menjelaskan simbol-simbol yang digunakan dalam grid dan aturan langkah-langkah yang harus diikuti oleh pemain.
