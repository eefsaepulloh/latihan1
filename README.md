#latihan1
# Cara penggunaan git
# Apa Itu Git ?
* Git adalah salah satu sistem pengontrol versi(Version Control System) pada proyek perangkat lunak yang diciptakan Linus Torvalds.
* Pengontrol versi bertugas memcatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri.
* Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja.
# Instalasi Git
* Download **Git**, Buka website resminya [git-scm.com](https://git-scm.com).
* Kemudian unduh Git sesuai dengan arsitektur komputer kita, Kalau
menggunakan 64bit, unduh yang 64bit. Begitu juga kalau
menggunakan 32bit.

![downloadgit](https://user-images.githubusercontent.com/56913656/67956393-9a592100-fc26-11e9-97f0-bd09cbf62134.png)
		
* Selamat, Git sudah terinstal di Windows. Untuk mencobanya,
		silahkan buka CMD atau PowerShell, kemudian ketik perintah
		``git --version``
		
 ![gitversion](https://user-images.githubusercontent.com/56913656/67958943-90d1b800-fc2a-11e9-97dc-9609400c9e97.png)
		
# Menambahkan Global Config
* Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi
*user.name dan user.email*
* konfigurasi ini bisa dilakukan untuk global repostiry atau individual
repository.
* apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi
kegagalan saat menjalankan perintah ``git commit``
* Config Global Repository
		
  ![gitconfig](https://user-images.githubusercontent.com/56913656/67959737-c3c87b80-fc2b-11e9-80b4-42c27fb6d5f8.png)

# Perintah Dasar Git
* ``git init`` , perintah untuk membuat repository local.
* ``git add`` , perintah untuk menambahkan file baru, atau perubahan pada file pada staging sebelum proses commit.
* ``git commit`` , perintah untuk menyimpan perubahan kedalam database git.
* ``git push -u origin master`` , perintah untuk mengirim perubahan pada repository local menuju server repository.
* ``git clone [url]``, perintah untuk membuat working directory yang diambil dari repositry sever.
* ``git remote add origin [url]`` , perintah untuk menambahkan remote server/reopsitory server pada local repositry (working directory)
* ``git pull`` , perintah untuk mengambil/mendownload perubahan terbaru dari server repository ke local repository.
# Membuat Reposiory Local
* Buka direktory aktif, misal: ``d:\labs_pemrograman1`` (bukamenggunakan Windows Explorer)
* klik kanan pada direktory aktif tersebut, dan pilih menu ``Git Bash``,sehingga muncul git bash commad
* Buat direktory project praktikum pertama dengan nama **latihan1**
		
  ![reposiorylocal](https://user-images.githubusercontent.com/56913656/68035814-ff7c4780-fcf6-11e9-94d4-8b58dc0462bf.png)
	 
* Sehingga terbentuk satu direktori baru dibawahnya, selanjutnyamasuk kedalam direktori tersebut dengan perintah cd *(changedirectory)*
* direktory aktif menjadi: ``d:\labs_pemrograman1\latihan1``
# Membuat Reposiory Local
* Jalankan perintah git init, untuk membuat repository local.
* Repository baru berhasil di inisialisasi, dengan terbentuknya satudirektori hidden dengan nama **.git**
* Pada direktori tersebut, semua perubahan pada *working directory* akan disimpan.
		
  ![gitinit](https://user-images.githubusercontent.com/56913656/68037108-9b0eb780-fcf9-11e9-9ec6-3b7deeaf4620.png)
		
# Menambahkan File baru pada repository
* Untuk membuat file dapat menggunakan text editor, lalu menyimpafilenya pada direktori aktif (repository)
* disini kita akan coba buat satu file bernama README.md (text file) ``$ echo “#Latihan 1” >> README.md``
		
  ![echo](https://user-images.githubusercontent.com/56913656/68037392-343dce00-fcfa-11e9-9166-35c047989044.png)
