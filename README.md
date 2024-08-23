---------------------------------------------------------------------------------------------------------------
CARA INSTALL MANUAL
---------------------------------------------------------------------------------------------------------------
1. Pastikan sudah terinstall web server Apache, PHP, MySQL, dan phpmyadmin di komputer.
	Bagi pengguna OS Windows, untuk memudahkan silahkan download XAMPP atau WAMP SERVER.
	WAMP SERVER download disini http://www.wampserver.com
	XAMPP download disini https://www.apachefriends.org
2. Buat folder dengan nama "cmssekolahku" dalam direktori xampp/htdocs, jika mengunakan XAMPP atau
	dalam direktori www jika menggunakan WAMP.
3. Extract file cms-sekolahku-v2.x.x.zip ke dalam folder "cmssekolahku"
4. Buka phpMyAdmin di browser dengan mengetikan localhost/phpmyadmin
5. Pilih menu "DATABASE" kemudian buat database dengan nama "db_cms_sekolahku"
6. Jika point 5 sukses, database dengan nama "db_cms_sekolahku" akan muncul disamping kiri.
7. Klik database tersebut dan pilih menu "IMPORT", kemudian browse file dengan nama "db_cms_sekolahku.sql"
	yang saya sertakan dalam folder hasil download.
8.	Selesai.

- Silahkan buka browser dan ketikan URL : localhost/cmssekolahku
- Untuk login ke halaman administrator, ketikan URL: localhost/cmssekolahku/login
- Default username dan password yaitu "administrator"
- CATATAN : Sampai langkah 7 seharusnya program sudah bisa dijalankan,
	untuk memastikan konfigurasi database sudah benar atau belum,
	silahkan buka file "database.php" yang ada di dalam folder "cmssekolahku/application/config/database.php"
	dengan menggunakan Code Editor sejenis Notepad++ atau Sublime Text.
	Lihat baris 78, 79, dan 80, silahkan sesuaikan 3 baris tersebut dengan konfigurasi masing-masing.
---------------------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------------------
CARA INSTALL MENGGUNAKAN "INSTALLER"
---------------------------------------------------------------------------------------------------------------
1. Pastikan sudah terinstall web server Apache, PHP, MySQL, dan phpmyadmin di komputer.
	Bagi pengguna OS Windows, untuk memudahkan silahkan download XAMPP atau WAMP SERVER.
	WAMP SERVER download disini http://www.wampserver.com
	XAMPP download disini https://www.apachefriends.org
2. Buat folder dengan nama "cmssekolahku" dalam direktori xampp/htdocs, jika mengunakan XAMPP atau
	dalam direktori www jika menggunakan WAMP.
3. Extract file cms-sekolahku-v2.x.x.zip ke dalam folder "cmssekolahku"
4. Buka phpMyAdmin di browser dengan mengetikan localhost/phpmyadmin
5. Pilih menu "DATABASE" kemudian buat database dengan nama "db_cms_sekolahku"
6. Buka Browser kemudian ketik "localhost/cmssekolahku/install"
7. Ikuti sesuai petunjuk yang ditampilkan
8. Selesai
---------------------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------------------
CARA UPGRADE DARI 2.4.12 KE 2.4.13
---------------------------------------------------------------------------------------------------------------
*) UNTUK MENGHINDARI KESALAHAN, Silahkan backup terlebih dahulu source web dan database yang digunakan saat ini.
*) PROSES UPGRADE PASTIKAN DILAKUKAN DI LOCALHOST. SANGAT TIDAK DISARANKAN DILAKUKAN LANGSUNG DI HOSTING
- Replace "file" "webmaster.php" di dalam folder "application/config"
- Replace semua "file" dan "folder" di dalam folder "assets"
- Replace semua "file" dan "folder" di dalam folder "views"
- Replace semua "file" dan "folder" di dalam folder "application/controllers"
- Replace semua "file" di dalam folder "application/core"
- Replace semua "file" di dalam folder "application/helpers"
- Replace semua "file" di dalam folder "application/hooks"
- Replace semua "file" di dalam folder "application/libraries"
- Replace semua "file" di dalam folder "application/models"
- Import file DATABASE_UPGRADE.sql di phpmyadmin
---------------------------------------------------------------------------------------------------------------
