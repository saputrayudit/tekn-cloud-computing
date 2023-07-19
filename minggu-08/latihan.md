# Praktikum Teknologi Cloud Computing - Minggu 8 (LATIHAN)

## Step 1: Setup

---
1. Membuat folder proyek

    ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/e8624679-e432-4e41-97f9-01e00792104d)

    ```
    //Membuat folder baru dengan nama composetest
    $ mkdir composetest

    //Berpindah ke folder composetest
    $ cd composetest/

    //Membuka code editor vscode
    $ code .
    ```
2. Membuat file app.py

    ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/2aa8daa2-99ed-4498-ab7a-7d29773370f1)
3. Membuat file requirements.txt

    ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/08c39698-4542-4ac6-b779-66036ff601b1)

---
## Step 2: Create a Dockerfile
---
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/fe774a0c-fe7b-4d14-9f5d-3c7b74fac428)
---
## Step 3: Define services in a Compose file

![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/0dde448e-16a0-4aa9-8846-d20642548e70)

---
## Step 4: Build and run your app with Compose
---
1. Menjalankan perintah docker-compose up

    ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/ce8f50a8-cefc-4533-9fa9-ba95e9ecd8a0)

    ```
    //Mulai menjalankan aplikasi
    $ docker-compose up
    ```
2. Membuka url http://localhost:5000/ untuk melihat hasilnya

   ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/ce4268c5-f86e-491e-992f-8360502990ab)

3. Merefresh halaman

    ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/7e5b26e8-5d10-4de2-8e72-d2e10243c4de)

4. Membuka terminal lain dan menjalankan perintah docker image ls

    ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/65809589-2920-4b3f-ae47-6e00f82044fe)

    ```
    //Melihat daftar lokal image
    $ docker image ls
    ```
---
## Step 5: Edit the Compose file to add a bind mount

![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/bcbbffef-5733-4731-bf76-91c03df1bb8c)
---
## Step 6: Re-build and run the app with Compose
1. Menjalankan perintah docker-compose up

    ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/9e25d0c8-43d6-4d3d-86a9-303d3896fc37)

    ```
    //Mulai menjalankan aplikasi
    $ docker-compose up
    ```
2. Mengecek pada browser

    ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/065ed804-57e7-46a8-b455-c20a40e96245)


---
## Step 7: Update the application
1. Merubah file app.py
   ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/40494109-e47a-4715-8bb3-b0cc31ce0266)

2. Mengecek hasilnya pada browser

    ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/c9232569-5621-43c0-851d-320cba89fd36)

---
## Step 8: Experiment with some other commands
1. Menjalankan perintah docker lainnya

   ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/70ca7240-efa6-42f3-b2d9-64e1b20967fa)


    ```
    //Menjalankan aplikasi pada latar belakang
    $ docker-compose up -d

    //Melihat aplikasi yang sedang berjalan
    $ docker-compose ps
    ```
2. Menjalankan perintah docker lainnya

  ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/a04ca4bf-41df-454b-b094-c3e8a8c0f065)


    ```
    //Menjalankan dan melihat variabel yang tersedia
    $ docker-compose run web env

    //Menghentikan aplikasi
    $ docker-compose stop

    //Menghapus containers
    $ docker-compose down --volumes
    ```
