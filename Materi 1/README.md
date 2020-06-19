# Materi ke-1 - Docker For Beginners - Linux
-------------------------------------------------------
## Login ke akun Docker Hub
-------------------------------------------------------


supaya kita dapat mengakses terminal maka dilakukan login pada akun Docker Hub

-----------------------------------------------------------------------
## Task 0: Prerequisites
-----------------------------------------------------------------------

Pada *Prerequisites* ini dilakukan clone repo github untuk mendapatkan linux_tweet_app kemudian dilanjutkan dengan langkah selanjutnya yaitu pada **Task 1: Run some simple Docker containers** untuk memulai container baru dengan menggunakan image alphine dan mengecek daftar image yang tersedia.
Yang ditunjukkan pada hasil dibawah.



**Run an interactive Ubuntu container**

Mengakses image ubuntu untuk menjalankan terminal dari ubuntu, kemudian dilakukan perintah :
```
$ ls /
$ ps aux
$ cat /etc/issue
```
> perintah $ ls / digunakan untuk melihat file yang ada pada direktori ubuntu
> perintah $ ps aux digunakan untuk melihat container yang sedang berjalan saat ini
> perintah $ cat /etc/issue digunakan untuk menampilkan container yang digunakan saat ini

dengan hasil pada gambar dibawah



kemudian dilakukan perintah exit untuk keluar dari image ubuntu yang sedang dijalankan dan kemudian mengetikkan perintah *cat /etc/issue* untuk menampilkan versi VM yang digunakan setelah keluar dari ubuntu
dengan hasil gambar dibawah



**Run a background MySQL container**

Yang pertama dilakukan yaitu menjalankan MySQL container baru



Selanjutnya melihat proses yang sedang berjalan pada container



Selanjutnya yaitu melihat versi MySQL container yg sedang berjalan kemudian Menjalankan perintah untuk memberikan shell interaktif ( sh) di dalam MySQL container dan mengetikkan perintah *mysql --user=root --password=$MYSQL_ROOT_PASSWORD --version* kemudian ketikkan perintah *exit* untuk keluar dari terminal



--------------------------------------------------------------------------

## Task 2: Package and run a custom app using Docker
--------------------------------------------------------------------------

Pertama, berpindah pada direktori *linux_tweet_app* yang diawal tadi sudah diclone kemudian menampilkan isi Dockerfile



Selanjutnya melakukan Ekspor variabel ke DockerId untuk mendapatkan akses gratis dari variabel ini kemudian dilanjutkan dengan menampilkan isi DockerId



Selanjutnya yaitu membuat Image Docker baru



Selanjutnya memulai container baru dari image yang telah dibuat




Mematikan dan menghapus web yang telah dijalankan



--------------------------------------------------------------------------
## Task 3: Modify a running website
--------------------------------------------------------------------------

Memulai aplikasi web dan pasang direktori saat ini ke dalam container




**Modify the running website**

Menyalin yang baru *index.html* ke dalam container dengan mengetikkan perintah *cp index-new.html index.html* dan hasilnya dengan menjalankan


Hentikan dan hapus container yang sedang berjalan, kemudian menjalankan kembali versi saat ini tanpa bind mount, kemudian lihat hasilnya 


Berhenti dan lepaskan container yang berjalan saat ini


**Update the image**

Membuat image baru dengan versi 2.0


Melihat daftar image


**Test the new version**

Menjalankan container baru dari versi image yang baru 

Menjalankan container baru lain, kali ini dari versi image yang lama


**Push your images to Docker Hub**

Melihat daftar image pada host Docker


Login ke Docker Hub



Melakukan push image *linux_tweet_app versi 1.0 dan versi 2.0* ke akun Docker Hub


Hasil Setelah dilakukan push image ke akun Docker Hub

