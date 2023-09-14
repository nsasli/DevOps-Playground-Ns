# DevOps-Playground-Ns


>> Langkah 1: Membuat Aplikasi Sederhana
Buat direktori baru untuk proyek Anda dan masuk ke dalamnya:
mkdir my-web-app
cd my-web-app

>> Buat file Python yang disebut app.py dalam direktori tersebut dengan isi berikut:
>>Langkah 2: Membuat Docker Container

Sekarang, mari buat Docker container untuk aplikasi kita:

Buat file Dockerfile dalam direktori proyek dengan isi berikut:

Buat file requirements.txt 

Bangun Docker image dari Dockerfile:

docker build -t my-web-app .


Langkah 3: Jalankan Container Lokal

Sekarang, mari jalankan container lokal untuk memastikan aplikasi kita berjalan dengan baik:

docker run -p 8080:8080 my-web-app

Anda sekarang dapat membuka browser atau menggunakan perintah curl untuk mengakses aplikasi Anda di http://localhost:8080. Anda harus melihat pesan "Hello, World!".

=====
selanjutnya kira akan belajar mendeploy ke kubernetes

Langkah 4: Deploy ke Kubernetes

Selanjutnya, mari deploy aplikasi kita ke Kubernetes menggunakan minikube:

Pastikan minikube telah diinstal dan dijalankan:

minikube start (kalo belum terinstall bisa pake brew install minikube)

Buat file YAML yang disebut deployment.yaml dengan konfigurasi seperti yang ada di file .yaml


