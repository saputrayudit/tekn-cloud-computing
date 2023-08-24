# Praktikum Teknologi Cloud Computing - Minggu 11 (Application Containerization & Microservice Orchestration)

## Setup

![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/22b4b5d0-f4bc-4b74-b0fc-17771254310f)
```
//Mengclone repository dari url github
$ git clone https://github.com/ibnesayeed/linkextractor.git

//Berpindah ke direktori linkextractor
$ cd linkextractor

//Berpindah ke branch demo
$ git checkout demo
```
---
## Step 0: Basic Link Extractor Script

![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/0ebf6f8c-b7a4-493e-bed3-08ecf990fbc4)
```
//Berpindah ke branch step0
$ git checkout step0

//Menampilkan struktur folder
$ tree
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/471c8fe0-0f8d-4f61-844f-6029b331943c)
```
//Menampilkan isi file linkextractor.py
$ cat linkextractor.py

//Menjalankan file linkextractor.py
$ ./linkextractor.py http://example.com/
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/e371efcf-b6dc-4b07-8cd5-0685a4b22d6c)
```
//Melihat hak/izin akses file linkextractor.py
$ ls -l linkextractor.py

//Menjalankan file linkextractor.py
$ python linkextractor.py
```
---
## Step 1: Containerized Link Extractor Script

![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/1914aeef-b705-49cf-b6aa-cec275745117)
```
//Berpindah ke branch step1
$ git checkout step1

//Menampilkan struktur folder
$ tree
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/62d5e2c4-9320-4717-9e0e-2d67e1fa8e05)
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/fe0dc329-c469-4a84-83e7-d582e1f5a13d)
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/90e07f7f-f142-4c81-ab88-318f747871e8)
```
//Menampilkan isi file Dockerfile
$ cat Dockerfile

//Membuat image
$ docker image build -t linkextractor:step1 .

//Menampilkan daftar image
$ docker image ls

//Menjalankan container
$ docker container run -it --rm linkextractor:step1 http://example.com/
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/99ca422e-16ad-4553-8cf6-c2691f835ff6)
```
//Menjalankan container
$ docker container run -it --rm linkextractor:step1 https://training.play-with-docker.com/
```
---
## Step 2: Link Extractor Module with Full URI and Anchor Text

![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/fd2bc5b7-275d-4bd7-a9d2-f3ddfc2119c3)
```
//Berpindah ke branch step2
$ git checkout step2

//Menampilkan struktur folder
$ tree
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/9266cb70-7037-4915-be4c-3da8cd7c4b46)
```
//Menampilkan isi file linkextractor.py
$ cat linkextractor.py
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/f7550219-d7eb-4a19-8474-691fa92df74c)
```
//Membuat image
$ docker image build -t linkextractor:step2 .
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/32a66f51-5856-4dec-b6f6-2f7600f57765)
```
//Menampilkan daftar image
$ docker image ls
```
![acmo-16](acmo-16.png)
```
//Menjalankan container
$ docker container run -it --rm linkextractor:step2 https://training.play-with-docker.com/
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/735a5db0-5a66-4a7b-a8b0-e9e17e93799e)
```
//Menjalankan container
$ docker container run -it --rm linkextractor:step1 https://training.play-with-docker.com/
```
---
## Step 3: Link Extractor API Service
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/8b6a21df-b7e9-4bb7-9a9d-0b117f44c0b2)
```
//Berpindah ke branch step3
$ git checkout step3

//Menampilkan struktur folder
$ tree
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/4b38738b-db36-45b2-bf2a-4141be9e0db7)
```
//Menampilkan isi file Dockerfile
$ cat Dockerfile
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/40026832-adfb-4c15-bb42-68af04afafc5)
```
//Menampilkan isi file main.py
$ cat main.py
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/3c74013d-7723-4813-8ee2-788e4a578520)
```
//Membuat image
$ docker image build -t linkextractor:step3 .
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/c28fc953-9218-4ee7-9bb7-4c1c5dcf2391)
```
//Menjalankan container
$ docker container run -d -p 5000:5000 --name=linkextractor linkextractor:step3

//Menampilkan daftar container
$ docker container ls
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/a10b4d9b-bc02-4757-b802-fbae568fd503)
```
//Membuat permintaan HTTP
$ curl -i http://localhost:5000/api/http://example.com/
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/f5aaa4c6-0790-4fb4-a45b-a9b911fd073d)
```
//Melihat catatan container
$ docker container logs linkextractor

//Menghapus container
$ docker container rm -f linkextractor
```
---
## Step 4: Link Extractor API and Web Front End Services

![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/98b24234-a127-4750-85ba-66ead75dbdf4)
```
//Berpindah ke branch step4
$ git checkout step4

//Menampilkan struktur folder
$ tree
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/c35db1ea-f8f8-4f0f-869c-47bb78f0e53d)
```
//Menampilkan isi file docker-compose.yml
$ cat docker-compose.yml
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/489cce98-1f5c-49eb-b71d-4b8dbd8b9eb0)
```
//Menampilkan isi file www/index.php
$ cat www/index.php
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/0f4ec80d-3026-4a94-961b-05e53137a7bb)
```
//Menjalankan layanan docker compose
$ docker-compose up -d --build
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/45d4329b-84cb-4f8f-b08b-aa62069dafbb)
```
//Menampilkan daftar container
$ docker container ls
```
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/3be16acb-05f1-4729-b811-154ec3422cd3)
```
//Menghubungakan dengan layanan API
$ curl -i http://localhost:5000/api/http://example.com/
```
