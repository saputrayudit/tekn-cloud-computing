![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/53c56790-899a-4e51-a69d-bf7e0ccbcc7a)# Konfigurasi Image MySQL pada nginx
1. pull image nginx
> docker pull nginx:alpine
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/07576479-b04f-40f1-96c8-4df257b02d00)
2. check pada docker image sudah terpasang repository nya atau tidak
> docker images
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/3231ff32-e0de-4c15-95b8-3514d135e8e8)
3. membuat repo di web
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/2f71d732-cfd1-4773-b9bf-114b4889fbff)
4.membuat 2 repo dengan versi yang berbeda 
> docker tag nginx:alpine yuditsaputra/coba:1.0
> docker tag nginx:alpine yuditsaputra/coba:1.1
check juga hasilnya di
> docker images
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/74bf4950-94f7-44b6-b9ae-83b03e172e98)
5. jika sudah kita akan coba push repo ke web
> docker push yuditsaputra/coba:1.0
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/6f1da0fd-0eee-41a7-8c14-c80425b78802)
hasil
> ![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/00fe597c-0c63-454e-ac79-5cbb22dac1ad)
> docker push yuditsaputra/coba:1.1
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/4804c927-96b7-4dd9-b8fb-0810050a1bcd)
hasil
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/65e3bb05-ee0a-4eea-9797-9c18f53217c6)
6. selanjutnya kita akan memasang mysql
> docker run --name some-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=my-secret-pw -d mysql



