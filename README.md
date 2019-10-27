#latihan1
CARA PEMBUATAN REPOSITORY LOCAL dan PEMBUATAN FILE README.md MENGGUNAKAN GIT
LANGKAH-LANGKAH :
1. INSTALL GIT
~Bisa di download pada website https://git-scm.com/. Kemudian unduh sesuai arsitektur komputer kita,jika menggunakan 64bit,unduh yg 64bit. Begitu juga dengan yang 32bit.

![Screenshot (26)](https://user-images.githubusercontent.com/57055098/67630124-0c430a80-f8b5-11e9-9ae1-1783941ebef2.png)

~Buka GIT yang telah di download tadi, ikuti langkah (klik next) sampai proses install selesai.(ini untuk yang tidak berbayar/ free)

![Screenshot (2)](https://user-images.githubusercontent.com/57055098/67630199-98a1fd00-f8b6-11e9-83b2-cd3186852d8f.png)

proses install selesai

![Screenshot (12)](https://user-images.githubusercontent.com/57055098/67630214-03533880-f8b7-11e9-9776-b05e18b45fb0.png)

untuk memastikan sudah terinstall,coba dengan cara buka CMD/ PowerShell melalui W + R atau pun search "CMD" di Windows Explore. Setelah itu ketik perintah "git --version" lalu enter, jika versi telah muncul maka git sudah terpasang dan dapat digunakan.

![Screenshot (27)](https://user-images.githubusercontent.com/57055098/67630292-d3586500-f8b7-11e9-82a0-945b4965f57e.png)

2. SIGN UP
~sebelum membuat Repository, silakan sign up di https://github.com/ . Isi username, email, dan password.

![Screenshot (13)](https://user-images.githubusercontent.com/57055098/67630335-a6588200-f8b8-11e9-9946-20a8b70ab73e.png)

~Verifikasi email yang di kirimkan ke email anda, selanjutnya anda akan dialihkan ke laman Github untuk membuat Repository baru

![Screenshot (16)](https://user-images.githubusercontent.com/57055098/67630378-2ed72280-f8b9-11e9-8a41-901948b7686b.png)

3. BUAT REPOSITORY LOCAL
~Sebelum membuat Repository dilaman Github. terlebih dahulu buka direktory aktif dengan search git pada Windows Explore atau klik kanan sembarang di tampilan dekstop ataupun di Folder yang sudah kalian tentukan.

![Screenshot (17)](https://user-images.githubusercontent.com/57055098/67630445-2d5a2a00-f8ba-11e9-81b6-60c1e29d3b0e.png)

~Lalu klik "Git Base Here", kemudian akan muncul Git Base Command

![Screenshot (18)](https://user-images.githubusercontent.com/57055098/67630485-11a35380-f8bb-11e9-8263-4f2956278b4e.png)

~Saat pertama kali menggunakan git, perlu dilakukan "Global Config" atau konfigurasi "user.name" dan "user.email". Apabila belum melakukan konfigurasi bisa terjadi kegagalan saat menjalankan perintan "git commit". Dengan perintah sebagai berikut ;
$ git config --global user.name "username"
$ git config --global user.email "email"

![Screenshot (29)](https://user-images.githubusercontent.com/57055098/67630627-4dd7b380-f8bd-11e9-9237-404670119e99.png)

~Setelah melakukan global config, lanjutkan dengan membuat direktory project yang akan kalian buat, misal: latihan1 dengan perintah
$ mkdir latihan1
$ cd latihan1
( nama tidak boleh sama dengan project yang pernah kalian buat )

![Screenshot (30)](https://user-images.githubusercontent.com/57055098/67630685-38af5480-f8be-11e9-80f5-b05ff678e732.png)

~ Setelah itu masukan perintah "git init" untuk membuat Repository baru.

![Screenshot (31)](https://user-images.githubusercontent.com/57055098/67630756-3ef20080-f8bf-11e9-8cec-7cbf3dd584e1.png)

(Jika Repository baru berhasil di inisialisasi, maka terbentuklah satu direktori hidden dengan nama ".git").
~Untuk menambahkan file baru pada repository dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif(repository). disini kita mencoba membuat file bernama README.md (text file)
$ echo "#Nama_Project" >> README.md dan untuk melihat file ketik perintah $ ls -l 

![Screenshot (34)](https://user-images.githubusercontent.com/57055098/67630943-baed4800-f8c1-11e9-8bd9-76e1d24fd36c.png)

~Untuk menambahkan file yang baru dbuat tadi, gunakan perintah "git add".
$ git add README.md

![Screenshot (35)](https://user-images.githubusercontent.com/57055098/67630996-b9704f80-f8c2-11e9-8ef8-59360c114c97.png)

(File README.md berhasil ditambahkan dan jika salah memasukkan perintah dan terjadi eror, bisa dilakukan kembali).
~Setelah itu, untuk menyimpan perubahan yang ada kedalaman database repository lokal, bisa menggunakan perintah ;
$ git commit -m "komentar commit" (misal nama komentar "File Pertama Saya")

![Screenshot (36)](https://user-images.githubusercontent.com/57055098/67631022-3ac7e200-f8c3-11e9-8f03-7e593e9dc37c.png)

~Kemudian, menambahkan remote repository untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses banyak user. berikut perintahnya : $ git remote add origin [URL]
(URL bisa didapatkan saat melakukan Repository Server).
Berikut cara untuk mengetahui URL Anda :

PEMBUATAN REPOSITORY SERVER
  -Buat Repository Server, dengan menggunakan laman github https://github.com
  Jika belum membuat akun buatlah Akun terlebih dahulu. Caranya ada diatas number "2. SIGN UP". Jika sudah mempunyai akun Anda bisa
  Sign   in. Sehabis itu Anda bisa klik Start a Project atau dari menu icon ( + ) di pojok kanan atas, lalu pilih New Repository
  
  ![Screenshot (37)](https://user-images.githubusercontent.com/57055098/67631116-95157280-f8c4-11e9-923d-d7bd2e2a6cda.png)
  
  ![Screenshot (38)](https://user-images.githubusercontent.com/57055098/67631123-9e9eda80-f8c4-11e9-8e64-74da3e1a57df.png)
  
  -Setelah itu, isi Nama Repository dan Description sesuai keinginan Anda , misal : labspy01 . Lalu klik "Create Repository".
  
  ![Screenshot (39)](https://user-images.githubusercontent.com/57055098/67631145-d574f080-f8c4-11e9-82f4-0ce9ef97c7f5.png)
  
  -Selanjutnya, akan muncul repository baru atau laman seperti gambar dibawah. Lalu copy URL tersebut untuk melanjutkan perintah
  repository lokal di Git Bash Command.
  
  ![Screenshot](https://user-images.githubusercontent.com/57055098/67631209-a0b56900-f8c5-11e9-8ef4-57bc2af9b03d.png)
  
  -URL tersebut digunakan untuk perintah Remote Repository. Berikut perintahnya : $ git remote add origin [URL] contoh hasil :
  
  ![Screenshot (40)](https://user-images.githubusercontent.com/57055098/67631231-0c97d180-f8c6-11e9-984f-ae4582834438.png)

KEMBALI KE REPOSITORY LOCAL atau GIT BASE COMMAND
~Setelah menambahkan remote repository, selanjutnya lakukan PUSH (mengirim perubahan ke server). Untuk mengirim perubahan dari repository local ke reposiroty server bisa menggunakan perintah "git push".
$ git push -u origin master

![Screenshot (41)](https://user-images.githubusercontent.com/57055098/67631281-b24b4080-f8c6-11e9-91f1-0a562bacad19.png)

~Kemudian perintah itu akan meninta memasukkan Username dan Password pada ada akun github.com.

![Screenshot (42)](https://user-images.githubusercontent.com/57055098/67631320-3a314a80-f8c7-11e9-92c0-4f1fe4bde3bf.png)

~Selanjutnya, melakukan Clone Repository digunakan untuk chekout repository atau pada dasarnya yaitu meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (Working Directory). Untuk melakukan cloning bisa menggunakan perintah git Clone [URL]. Untuk mengetahui URL bisa menggunakan URL pada perintah Remote Repository karna sama saja atau URL bisa dicopy dari clone or download klik, lalu akan muncul URL dari file tersebut.

![Screenshot (23)](https://user-images.githubusercontent.com/57055098/67631340-6d73d980-f8c7-11e9-9095-c09dd61db135.png)

Setelah log in, untuk melihat hasilnya pada server repository buka kembali laman baru *https://github.com . Arahkan pada repositorinya misal : febrijumawan27/labspy01

![Screenshot (43)](https://user-images.githubusercontent.com/57055098/67631378-24705500-f8c8-11e9-8cac-0c8fc3331b52.png)

Repository Anda sudah bisa digunakan. Klik pada lambang pensil dan Anda bisa membuat project di file README.md tersebut.

![Screenshot (44)](https://user-images.githubusercontent.com/57055098/67631410-ac565f00-f8c8-11e9-8e2f-3c543d7151e4.png)

File README.md sudah bisa di edit

![Screenshot (45)](https://user-images.githubusercontent.com/57055098/67631425-eb84b000-f8c8-11e9-9948-69674398d79d.png)

TERIMAKASIH SUDAH MEMBACA
<<TUGAS MATA KULIAH BAHASA PEMROGRAMAN>>
<<DOSEN PENGAMPU AGUNG NUGROHO, S.Kom., M.Kom.>>
