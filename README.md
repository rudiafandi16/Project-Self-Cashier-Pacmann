# Project-Self-Cashier-Pacmann
Pengumpulan Project Python Sekolah Bisnis 2022

SELF_CASHIER (KASIR MANDIRI)
Merupakan program python sederhana yang digunakan untuk melakukan penambahan, penghapusan, pengecekan, dan perhitungan dari total belanjaan secara otomatis. Data berasal dari input user atau dalam hal ini customer.

LATAR BELAKANG
Project python sederhana ini dibuat untuk membantu Andi seorang pemilik Supermarket besar di salah satu kota di Indonesia. Andi memiliki rencana untuk melakukan perbaikan proses bisnis, yaitu dengan membuat sistem kasir yang sifatnya self-service di supermarket miliknya. Sehingga customer bisa langsung memasukkan item yang dibeli, jumlah item yang dibeli, dan harga item yang dibeli dan fitur yang lain. Sehingga customer yang tidak berada di kota tersebut bisa membeli dari supermarket tersebut. 

REQUIREMENT
Program kasir mandiri ini berbentuk modular code, yaitu ada file yang menyimpan data code(kasir_mandiri.py) kemudian ada satu file lagi yaitu main.py untuk melakukan eksekusi kode. Dibutuhkan juga modular pandas untuk membantu visualisasi tabel dari barang belanjaan. Kemudian data disimpan dalam bentuk disctionary, dan ada 9 method yang digunakan dalam program ini.
![Flow Chart Kasir Mandiri](https://user-images.githubusercontent.com/53332703/218122385-ac6ec8f5-e111-4d76-a7b5-f283b6f9a7d6.png)

FUNGSI (ATTRIBUTE)

1.  Class: Transaction
    Dibuat suatu class yang diberi nama Transaction yang digunakan sebagai prototipe untuk wadah menghimpun data dan fungsi yang kemudian menghasilkan objek.
2.  Method: __init__
    Dibuat untuk menyimpan data item belanjaan ke dalam bentuk dictionary.
3.  Method: add_item
    Method untuk menambahkan data belanjaan. dengan tiga parameter yaitu nama, jumlah dan harga.
4.  Method: update_item_name
    Method untuk mengganti nama item belanjaan jika sebelumnya ada kesalahan dalam memasukkan nama item.
5.  Method: update_item_qty
    Method untuk mengubah jumlah dari suatu item belanjaan.
6.  Method: update_item_price
    Method untuk mengubah suatu harga dari item belanjaan.
7.  Method: delete_item
    Method untuk menghapus salah satu item belanjaan.
8.  Method: reset_transaction
    Method untuk menghapus seluruh item pada data belanjaan.
9.  Method: check_order
    Method untuk mengecek daftar barang belanjaan yang sudah input, memastikan bahwa itemnya sudah sesuai yang diinginkan.
10. Method: total_price
    Method untuk menghitung harga total dari semua item belanjaan yang sudah diinput.

TEST CASE

Test case 1
Customer ingin menambahkan dua item baru menggunakan method add_item(). Item yang ditambahkan adalah sebagai berikut:
a. Nama Item: Ayam Goreng, Qty: 2, Harga: 20000
b. Nama Item: Pasta Gii, Qty:3, Harga: 15000
output:
![Test case 1](https://user-images.githubusercontent.com/53332703/218124697-4c940eb6-41b0-404f-b8f8-3a32058844cd.png)

Test case 2
Ternyata Customer salah membeli salah satu item dari belanjaan yang sudah ditambahkan, maka Customer menggunakan method delete_item() untuk menghapus item. Item yang ingin dihapuskan adalah Pasta Gigi.
output:

![Test case 2](https://user-images.githubusercontent.com/53332703/218124739-42f7709a-5ede-4817-9be5-e3a9fa142022.png)

Test case 3
Ternyata setelah dipikir-pikir Customer salah memasukkan item yang ingin dibelanjakan! Daripada menghapusnya satu satu, maka Customer cukup menggunakan method reset_transaction() untuk menghapus semua item yang sudah ditambahkan.
output:
![Test case 3](https://user-images.githubusercontent.com/53332703/218124769-484d689a-1ffd-4d79-bfad-76b81a9cd2f8.png)

Test case 4
Setelah Customer selesai berbelanja, akan menghitung total belanja yang harus dibayarkan menggunakan method total_price(). Sebelum mengeluarkan Ouput total belanja akan menampilkan item item yang dibeli.
output:
![Test case 4](https://user-images.githubusercontent.com/53332703/218124791-b04dd4be-d806-43c1-b0a2-f9f87c24a53a.png)

KESIMPULAN
Demikikian program ini dibuat untuk memenuhi tugas project akhir kelas python dari course pacmann. Program yang dibuat belum sempurna, untuk
saran dan kritik sangat berguna bagi saya.
Terima kasih