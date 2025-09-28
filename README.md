[Mini Project 2.py](https://github.com/user-attachments/files/22582580/Mini.Project.2.py)# MINI-PROJECT-2

**===== SISTEM INFORMASI NILAI KELAS B SMAN 2 BERAU =====**

**NAMA : ALISYA OCTA NOOR GHINA**

**NIM : 2509116017**

**KELAS : A**

# Flowchart
![Flowchart Mini Project 2-Halaman-1](https://github.com/user-attachments/assets/d2546973-c407-4be1-accb-562b78c509e7)
![Flowchart Mini Project 2-Halaman-2](https://github.com/user-attachments/assets/6e2c0f78-78bd-4f73-bf39-9ebf98834c7d)


# File Program
FILE : [Uploading Mini Project 2.py…]()


# Penjelasan Kode dan Output
<img width="614" height="154" alt="Screenshot (249) 1" src="https://github.com/user-attachments/assets/11a30895-1d32-4273-ad8e-3a3c840a3bb6" />\
**PENJELASAN**\
from prettytable import PrettyTable: Library ini digunakan untuk membuat tabel data yang rapi dan mudah dibaca.\
from pwinput import pwinput: Library ini digunakan untuk membuat input password tersembunyi (tidak muncul di layar saat diketik).\
Jika library ini belum terinstal, program akan error saat dijalankan—pengguna harus install dulu dengan pip install prettytable pwinput. Ini mempersiapkan tools untuk tampilan dan keamanan seluruh program.

<img width="549" height="333" alt="Screenshot (249)" src="https://github.com/user-attachments/assets/629e645d-f215-438b-9f3b-ae9f2251ecaf" />\
**PENJELASAN**\
Menggunakan beberapa list (daftar), seperti :
1. List Siswa (Menyimpan nama-nama siswa)
2. List No Absen (Menyimpan nomor absen yang sesuai urutan)
3. List Nilai Matematika (Menyimpan nilai untuk mata pelajaran Matematika)
4. List Nilai B.Indonesia (Menyimpan nilai untuk mata pelajaran Bahasa Indonesia)
5. List Nilai B.Inggris (Menyimpan nilai untuk mata pelajaran Bahasa Inggris)
6. List Mata Pelajaran (Daftar tetap/ Tuple untuk nama mata pelajaran. Tuple digunakan nanti di menu untuk tampilan pilihan dan tidak bisa diubah selama program berjalan. Berbeda dengan List yang bisa diubah ketika programnya berjalan.)

Menggunakan dictionary untuk menyimpan data. Dictionary ini seperti "kotak penyimpanan" sederhana.

<img width="666" height="202" alt="Screenshot (258)" src="https://github.com/user-attachments/assets/9a91087f-bd52-4608-a222-748add0f0c40" />\
**PENJELASAN**\
Pada "while True" program memulai loop tak terbatas untuk proses login sampai berhasil. Program akan meminta input username dan password. Loop ini memastikan pengguna bisa mencoba lagi jika gagal. Jika username ada di dictionary "users" dan password cocok dengan yang tersimpan, program mencetak "Login Berhasil ✅" dan me-return role pengguna yang kita masukkan. Ini akan mengakhiri fungsi dan mengembalikan nilai role ke pemanggil (seperti main program).
Jika kondisi if tidak terpenuhi (username/password salah), program mencetak "⚠ Login Gagal! Username atau password salah" dan loop berlanjut, meminta input ulang. Tidak ada batas percobaan, jadi pengguna bisa coba berkali-kali sampai benar.

<img width="666" height="238" alt="Screenshot (259)" src="https://github.com/user-attachments/assets/19daf650-9cc8-4792-ad4b-52be2a48444a" />\
**PENJELASAN**\
Pada fungsi tampilkan semua data terdapat library "PrettyTable". Pada tabel = PrettyTable(["Absen", "Nama", "Matematika", "B.Indonesia", "B.Inggris"]) dan for i in range(len(List_Siswa)): ... tabel.add_row([...]):
Program membuat objek tabel kosong dengan kolom-kolom tersebut menggunakan "PrettyTable". Kemudian, loop for berjalan dari 0 hingga panjang List_Siswa, menambahkan satu baris per siswa dengan data dari list: No_Absen[i], List_Siswa[i], Nilai_MTK[i], dll. Ini menyusun semua data menjadi tabel rapi.
Pada print(tabel): Program mencetak tabel lengkap ke layar, menampilkan semua siswa dalam format border yang indah.

<img width="510" height="387" alt="Screenshot (268)" src="https://github.com/user-attachments/assets/987f0788-c2ce-4472-bf04-f0f6f0d41298" />\
**OUTPUT**\
Pengguna memilih masuk sebagai Siswa. Pengguna memasukkan username dan password dengan benar. Program menampilkan menu yang dapat diakses oleh siswa.

<img width="510" height="375" alt="Screenshot (286)" src="https://github.com/user-attachments/assets/97e60841-9a3e-403e-b15e-fd18e6e5a442" />\
**OUTPUT**\
Program meminta pengguna memasukkan pilihannya, disini saya memilih menu 1 (Menampilkan semua nilai siswa). Program akan menampilkan semua nilai siswa dengan PrettyTable agar terlihat lebih rapi.

<img width="510" height="290" alt="Screenshot (274)" src="https://github.com/user-attachments/assets/0aa4d856-47f5-4e39-8be2-4615c1f8deb2" />\
**OUTPUT**\
Pengguna memilih masuk sebagai Siswa. Pengguna memasukkan username dan password yang salah. Program menampilkan pesan username/password salah. Program meminta pengguna untuk memasukkan kembali username dan password yang benar.

========================================================================================================================================================================================

<img width="783" height="261" alt="Screenshot (260)" src="https://github.com/user-attachments/assets/4f28384a-5b81-42b1-8fdf-b6e7171ccd25" />\
**PENJELASAN**\
Pada Fungsi Menampilkan Nilai Berdasarkan Absen,
Program akan meminta input nomor absen sebagai angka (menggunakan int() untuk konversi). Jika nomor absen ada di list "No_Absen", program akan mencari indeksnya (idx = No_Absen.index(absen)), membuat tabel kecil (tabel_menu2) dengan kolom ["Nama", "Matematika", "B.Indonesia", "B.Inggris"], program akan menambahkan satu baris data siswa tersebut (List_Siswa[idx], Nilai_MTK[idx], Nilai_BINDO[idx], dan Nilai_BING[idx].), dan mencetak tabelnya. Ini menampilkan nilai lengkap siswa yang dicari.
Jika absen tidak ada di No_Absen, program akan mencetak "⚠ Nomor Absen Tidak Ditemukan! ⚠" dan fungsi berhenti tanpa tampilan data.

<img width="510" height="328" alt="Screenshot (270)" src="https://github.com/user-attachments/assets/90aab1c4-f60b-4514-8c56-6a63c0f023de" />\
**OUTPUT**\
Program menampilkan menu yang dapat diakses Siswa. Pengguna memilih menu yang diinginkan. Disini saya memilih menu 2 (Melihat nilai berdasarkan absen). Pengguna memasukkan nomor absen yang ingin ia lihat nilainya, lalu program akan menampilkan nilai dari siswa dengan nomor absen tersebut. Program menampilkannya menggunakan PrettyTable.

<img width="510" height="268" alt="Screenshot (275)" src="https://github.com/user-attachments/assets/f2f242ed-4d46-4a6f-9329-37e833a6b51d" />\
**OUTPUT**\
Program menampilkan menu yang dapat diakses Siswa. Pengguna memilih menu yang diinginkan. Disini saya memilih menu 2 (Melihat nilai berdasarkan absen). Pengguna memasukkan huruf dan bukan angka, program akan menampilkan pesan Nama Siswa Tidak Ditemukan.

========================================================================================================================================================================================

<img width="755" height="203" alt="Screenshot (261)" src="https://github.com/user-attachments/assets/11c52da9-b329-4d61-b8ae-d6c6f628e186" />\
**PENJELASAN**\
Pada Fungsi Menampilkan Nilai Berdasarkan Nama,
Program akan meminta input nama siswa dalam huruf kapital. Jika nama yang dimasukkan cocok persis dengan salah satu elemen di List_Siswa (Harus kapital), program mencari indeksnya (idx = List_Siswa.index(nama)), membuat tabel kecil (tabel_menu3) dengan kolom ["Nama", "Matematika", "B.Indonesia", "B.Inggris"], program akan menambahkan satu baris data siswa tersebut (List_Siswa[idx], Nilai_MTK[idx], Nilai_BINDO[idx], dan Nilai_BING[idx].), dan mencetak tabelnya. Ini menampilkan nilai lengkap siswa yang dicari.
Jika nama tidak ada di List_Siswa (misalnya salah ketik atau huruf kecil), program mencetak "⚠ Nama Siswa Tidak Ditemukan! ⚠" dan fungsi berhenti tanpa tampilan data.

<img width="510" height="324" alt="Screenshot (272)" src="https://github.com/user-attachments/assets/e343fabc-0863-4143-aa54-dbd4391ae2ef" />\
**OUTPUT**\
Program menampilkan menu yang dapat diakses Siswa. Pengguna memilih menu yang diinginkan. Disini saya memilih menu 3 (Melihat nilai berdasarkan nama siswa). Pengguna memasukkan nama siswa yang ingin ia lihat nilainya, lalu program akan menampilkan nilai dari siswa dengan nama tersebut. Program menampilkannya menggunakan PrettyTable.

<img width="510" height="295" alt="Screenshot (288)" src="https://github.com/user-attachments/assets/1a9c1a1c-b908-4f8c-bf12-ee819f2f071a" />\
**OUTPUT**\
Program menampilkan menu yang dapat diakses Siswa. Pengguna memilih menu yang diinginkan. Disini saya memilih menu 3 (Melihat nilai berdasarkan nama siswa). Pengguna memasukkan huruf dan bukan angka, program akan menampilkan pesan Nama Siswa Tidak Ditemukan. Pengguna juga memasukkan nama siswa dengan tidak kapital, program akan menampilkan pesan Nama Siswa Tidak Ditemukan.

<img width="510" height="145" alt="Screenshot (273)" src="https://github.com/user-attachments/assets/1a6d3bbc-354f-49c4-bf5f-e960aca72f3a" />\
**OUTPUT**\
Program menampilkan menu yang dapat diakses Siswa. Pengguna memilih menu yang diinginkan. Disini saya memilih menu 4 (Keluar). Program akan menampilkan pesan Program Telah Selesai.

========================================================================================================================================================================================

<img width="665" height="379" alt="Screenshot (262)" src="https://github.com/user-attachments/assets/2569e867-4542-4a9a-aabe-e59ce3861d5b" />\
**PENJELASAN**\
Pada Fungsi Menambahkan Data,
Program akan meminta pengguna untuk menginput nama (teks kapital), absen (angka), dan tiga nilai mata pelajaran (angka). Jika input valid, program menambahkan data ke akhir list. Kemudian mencetak "Data Berhasil Ditambahkan ✅" dan memanggil tampilkan_data() untuk menampilkan tabel terupdate.
Pada blok try: ... except ValueError:
Jika input absen atau nilai bukan angka, program menangkap ValueError dan mencetak "⚠ Input Salah Harus Berupa Angka! ⚠", lalu fungsi berhenti tanpa menambah data.

<img width="510" height="548" alt="Screenshot (280)" src="https://github.com/user-attachments/assets/48c86dda-3b10-4c3a-9304-36639e2493a2" />\
**OUTPUT**\
Program menampilkan menu yang dapat diakses Guru. Pengguna memilih menu yang diinginkan. Disini saya memilih menu 2 (Menambahkan Data). Program akan menampilkan data siswa sebelum ditambah. Kemudian, pengguna memasukkan nama siswa, nomor absen, nilai matematika, nilai bahasa indonesia, dan nilai bahasa inggris. Program akan menampilkan pesan data berhasil ditambahkan dan menampilkan data siswa setelah ditambahkan menggunakan PrettyTable.

<img width="510" height="191" alt="Screenshot (281)" src="https://github.com/user-attachments/assets/a042343f-fe1d-42b6-bbc1-6bab610b9098" />\
**OUTPUT**\
Program menampilkan menu yang dapat diakses Guru. Pengguna memilih menu yang diinginkan. Disini saya memilih menu 2 (Menambahkan Data). Program akan menampilkan data siswa sebelum ditambah. Kemudian, pengguna memasukkan nama siswa, nomor absen, nilai matematika, nilai bahasa indonesia, dan nilai bahasa inggris. Disini Program memasukkan nomor absen dengan huruf lalu program menampilkan pesan input salah! harus berupa angka.

========================================================================================================================================================================================

<img width="696" height="527" alt="Screenshot (263)" src="https://github.com/user-attachments/assets/6618a937-43dd-47e1-bb85-3191a2f3d305" />\
**PENJELASAN**\
Pada Fungsi Mengubah Nilai,
Program menampilkan semua data siswa terlebih dahulu, kemudian program meminta pengguna untuk menginput absen sebagai angka. Jika bukan angka, tangkap error dan cetak "⚠ Input Salah! Harus Berupa Angka! ⚠". Jika absen yang dicari tidak ada, cetak "⚠ Nomor Absen Tidak ditemukan! ⚠".Jika absen yang dicari ada, cari indeks (idx = No_Absen.index(absen)). Kemudian tampilkan pilihan mata pelajaran. Program meminta input pilihan berupa angka, jika inputan pilihan bukan 1-3, cetak "⚠ Mata Pelajaran Tidak Tersedia! ⚠". Jika inputan pilihan tersedia 1-3, program meminta nilai baru (angka) dan update list yang sesuai (misalnya Nilai_MTK[idx] untuk MTK).
Jika selesai menginput nilai baru, cetak "Nilai Berhasil Diubah ✅" dan panggil tampilkan_data() untuk tampilan terupdate.

<img width="510" height="660" alt="Screenshot (282)" src="https://github.com/user-attachments/assets/5c44712e-9e54-4607-9874-e803f21c33d3" />\
**OUTPUT**\
Program akan menampilkan tabel data sebelum diubah nilainya, kemudian program akan meminta pengguna untuk menginput nomor absen siswa yang ingin diubah nilainya. Setelah itu program akan menampilkan pesan nila berhasil diubah dan menampilkan tabel yang sudah terubah nilai siswanya.

========================================================================================================================================================================================

<img width="665" height="358" alt="Screenshot (264)" src="https://github.com/user-attachments/assets/e94aad6b-3f2f-40b7-96ee-19816c6d9db2" />\
**PENJELASAN**\
Pada Fungsi Menghapus Data,
Program menampilkan semua data siswa terlebih dahulu, kemudian program akan meminta input absen berupa angka. Jika bukan angka, tangkap error dan cetak "⚠ Input Salah! Harus Berupa Angka! ⚠". Jika absen yang dicari tidak ada, cetak "⚠ Nomor Absen Tidak Ditemukan! ⚠". Jika absen yang dicari ada, cari indeks (idx = No_Absen.index(absen)), lalu hapus elemen di posisi itu dari semua list: List_Siswa.pop(idx), No_Absen.pop(idx), Nilai_MTK.pop(idx), dll. Ini menghapus seluruh data siswa sekaligus. Kemudian cetak "Data Berhasil Dihapus ✅" dan panggil tampilkan_data() untuk tampilan tersisa.

<img width="510" height="506" alt="Screenshot (283)" src="https://github.com/user-attachments/assets/bee776a0-6abc-4013-9aa1-3f2488258295" />\
**OUTPUT**\
Program akan menampilkan tabel data sebelum dihapus, kemudian program akan meminta pengguna untuk menginput nomor absen siswa yang ingin dihapus datanya. Setelah itu program akan menampilkan pesan data berhasil dihapus dan menampilkan tabel yang sudah terhapus data siswanya. 

========================================================================================================================================================================================

<img width="665" height="453" alt="Screenshot (265)" src="https://github.com/user-attachments/assets/99df5b9a-2af5-4451-b67d-7dffa4ef8f88" />\
**PENJELASAN**\
Pada Fungsi Menu Siswa,
Program memulai loop tak terbatas untuk menu siswa dan menampilkan 4 pilihan yang bisa diakses oleh siswa: lihat semua nilai, lihat nilai berdasarkan absen, lihat nilai berdasarkan nama, dan keluar. Kemudian, program akan meminta input pilihan menu berupa angka. Jika bukan angka, tangkap error dan cetak "⚠ Input Salah! Harus Berupa Angka! ⚠", lalu loop ulang. Jika pilihan bukan 1-4, cetak "⚠ Menu Pilihan Tidak Tersedia! ⚠" dan loop ulang. Jika pilihan tersedia di menu 1-4, panggil fungsi sesuai pilihan. Jika memilih 4, cetak pesan "Program Selesai" dan break untuk hentikan loop.

<img width="510" height="387" alt="Screenshot (268)" src="https://github.com/user-attachments/assets/6673b4bb-25d4-4616-9498-270fd7ed95c2" />\
**OUTPUT**\
Pengguna memilih masuk sebagai Siswa. Pengguna memasukkan username dan password dengan benar. Program menampilkan menu yang dapat diakses oleh Siswa.

<img width="510" height="145" alt="Screenshot (273)" src="https://github.com/user-attachments/assets/f435063e-088b-45ad-8cda-bc15634d463f" />\
**OUTPUT**\
Program meminta pengguna memasukkan pilihannya, disini saya memilih menu 4 (Keluar) dan program menampilkan pesan program selesai.

<img width="510" height="139" alt="Screenshot (289)" src="https://github.com/user-attachments/assets/c6f8b944-116a-4734-9dbe-b76b16fdaae7" />\
**OUTPUT**\
Program meminta pengguna memasukkan pilihannya, disini saya memilih menu 5 yang tidak tersedia dan program akan menampilkan pesan menu pilihan tidak tersedia.

========================================================================================================================================================================================

<img width="625" height="507" alt="Screenshot (266)" src="https://github.com/user-attachments/assets/7a2830d0-4f04-4b61-bdf7-f798585b33f0" />\
**PENJELASAN**\
Pada Fungsi Menu Guru,
Program memulai loop tak terbatas untuk menu guru dan menampilkan 5 pilihan yang bisa diakses oleh guru: lihat semua nilai, menambah data, mengubah nilai, menghapus data dan keluar. Kemudian, program akan meminta input pilihan menu berupa angka. Jika bukan angka, tangkap error dan cetak "⚠ Input Salah! Harus Berupa Angka! ⚠", lalu loop ulang. Jika pilihan bukan 1-5, cetak "⚠ Menu Pilihan Tidak Tersedia! ⚠" dan loop ulang. Jika pilihan tersedia di menu 1-5, panggil fungsi sesuai pilihan. Jika memilih 5, cetak pesan "Program Selesai" dan break untuk hentikan loop.

<img width="510" height="394" alt="Screenshot (278)" src="https://github.com/user-attachments/assets/74de0a47-8122-4a6b-9275-9bd015196b6c" />\
**OUTPUT**\
Pengguna memilih masuk sebagai Guru. Pengguna memasukkan username dan password dengan benar. Program menampilkan menu yang dapat diakses oleh Guru.

<img width="510" height="168" alt="Screenshot (285)" src="https://github.com/user-attachments/assets/173322e4-aa99-461d-acdd-e07937db14d1" />\
**OUTPUT**\
Program meminta pengguna memasukkan pilihannya, disini saya memilih menu 5 (Keluar) dan program menampilkan pesan program selesai.

<img width="510" height="163" alt="Screenshot (284)" src="https://github.com/user-attachments/assets/97f813a4-4a00-40c3-9cb3-603573f57211" />\
**OUTPUT**\
Program meminta pengguna memasukkan pilihannya, disini saya memilih menu 6 yang tidak tersedia dan program akan menampilkan pesan menu pilihan tidak tersedia.

========================================================================================================================================================================================

<img width="697" height="481" alt="Screenshot (267)" src="https://github.com/user-attachments/assets/2fa6afbf-2025-48c3-89c8-feeb1a7cebd4" />\
**PENJELASAN**\
Pada Fungsi Menu Utama,
Program memulai loop utama, program akan menampilkan pilihan role di awal. Kemudian program akan meminta input role berupa angka. Jika bukan angka, cetak "⚠ Input Salah! Harus Berupa Angka! ⚠" lalu loop ulang.
Jika pilih 1 (Siswa), panggil login(), lalu jalankan menu_siswa(). Setelah menu selesai, break hentikan loop utama (program berhenti total).
Jika pilih 2 (Guru), panggil login(), lalu jalankan menu_guru(). Setelah menu selesai, break hentikan loop utama (program berhenti total).
Jika pilih 3, program akan cetak pesan "Program Selesai" dan menghentikan program.
Jika role bukan 1-3, cetak "⚠ Menu Pilihan Tidak Tersedia! ⚠" lalu loop ulang, pengguna diminta untuk memasukkan kembali pilihan yang benar.

<img width="510" height="290" alt="Screenshot (274)" src="https://github.com/user-attachments/assets/488f6612-5d8e-49f0-b19f-c5fc15222b0e" />\
**OUTPUT**\
Pengguna memilih masuk sebagai Siswa. Pengguna memasukkan username dan password yang salah. Program menampilkan pesan username/password salah. Program meminta pengguna untuk memasukkan kembali username dan password yang benar.

<img width="510" height="303" alt="Screenshot (276)" src="https://github.com/user-attachments/assets/267b6cca-5e19-4de4-9834-7fec4fb9aa8d" />\
**OUTPUT**\
Pengguna memilih masuk sebagai Guru. Pengguna memasukkan username dan password yang salah. Program menampilkan pesan username/password salah. Program meminta pengguna untuk memasukkan kembali username dan password yang benar.

<img width="510" height="264" alt="Screenshot (277)" src="https://github.com/user-attachments/assets/42e2a461-3471-4d16-a986-c49512d9fba4" />\
**OUTPUT**\
Pengguna memilih menu keluar dan program menampilkan pesan Program Selesai.


