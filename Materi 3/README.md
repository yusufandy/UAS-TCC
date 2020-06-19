# Materi ke-3 - Application Containerization and Microservice Orchestration

Melakukan login ke akun Docker Hub untuk menampilkan terminal


----------------------------------------------------------------------------------------------------------------------------------------------------------------

## Step-0

Melakukan clone repository untuk mendapaktan kode demo, mengubah direktory, dan memeriksa demo


Memeriksa daftar file yang ada didalam **step0**


Melihat script python yang ada pada file *linkextractor.py*


Ketika menjalankan perintah *./linkextractor.py http://example.com/* terdapat hasil output **bash: ./linkextractor.py: Permission denied**, Maka dilakukan pemeriksaan izin pada file dengan menggunakan perintah *ls -l linkextractor.py*, Supaya skrip dapat dieksekusi dapat dilakuakn dengan menggunakan perintah *chmod a+x linkextractor.py* atau dengan menggunakan perintah *python linkextractor.py*


----------------------------------------------------------------------------------------------------------------------------------------------------------------

## Step-1

Memeriksa daftar file yang terdapat didalam **step1**


Melihat isi dari Dockerfile


Membuat Image Docker yang diberi nama *linkextractor:step1*


Melihat dafatr image dan menjalankan container dan meng-ekstrak tautan dari beberapa halaman web


Melihat halaman web dengan lebih banyak tautan


----------------------------------------------------------------------------------------------------------------------------------------------------------------

## Step-2

Memeriksa daftar file yang terdapat didalam **step2**


Melihat script *linkextractor.py* yang sudah diperbaharui


Membuat Docker image baru


Melihat daftar image yang berjalan


Menjalankan container *linkextractor:step2*


Menjalankan container *linkextractor:step1*


----------------------------------------------------------------------------------------------------------------------------------------------------------------

## Step-3

Memeriksa daftar file yang ada didalam **step3** dan Melihat isi Dockerfile


Melihat isi dari file *main.py*


Membuat Docker image baru dengan nama *linkextractor:step3*


Menjalankan container, kemudian melihat daftar container, dilanjutkan dengan membuat request HTTP dan mengambil respon yang berisi tautan yang diekstrak, Lalu melihat log container yang sedang berjalan


Menghapus container


----------------------------------------------------------------------------------------------------------------------------------------------------------------

## Step-4

Melihat daftar file yang ada didalam **step4**


Melihat isi dari file *docker-compose.yml*


Melihat isi dari file *www/index.php*


Membuat layanan yang terpisah


Melihat daftar container yang sedang berjalan, Mengakses interface dari web, Melakukan modifikasi pada **www/index.php** untuk mengganti link yang awalnya **Link Extractor** menjadi **Super Link Extractor**, Mereset perubahan, Menghentikan layanan


----------------------------------------------------------------------------------------------------------------------------------------------------------------

## Step-5

Melihat daftar file yang ada didalam **step5** dan melihat isi dari *www/Dockerfile*


Melihat isi dari *api/main.py*


Melihat isi dari file *docker-compose.yml* yang telah diperbaharui


Membuat layanan


Mengekstran tautan dari beberapa halaman web menggunakan interface web, Melihat perubahan dalam layanan yang berjalan dan memverifikasi bahwa perubahan yang dibuat secara lokal tidak mencerminkan dalam layanan yang berjalan, Me-Reset perubahan


Menghentikan layanan yang berjalan


----------------------------------------------------------------------------------------------------------------------------------------------------------------

## Step-6

Melihat daftar file yang ada didalam **step6**


Melihat isi dari *api/linkextractor.rb*


Melihat isi dari *api/Dockerfile* dan isi dari file *docker-compose.yml*


Membuat layanan baru


Mengakses API, Menghentikan layanan yang berjalan, Melihat log

