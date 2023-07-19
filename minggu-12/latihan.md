# Praktikum Teknologi Cloud Computing - (Kubernetes for minikube)

1.open langkah pada link berikut
- buka power shell dan ketikan 
 > https://minikube.sigs.k8s.io/docs/start/
![1](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/55ff3f37-a0ca-47d2-8a01-5c97d051cf37)
- jika sudah dia akan membuat folder pada c:
lalu ketikan langkah ini
> Invoke-WebRequest -OutFile 'c:\minikube\minikube.exe' -Uri 'https://github.com/kubernetes/minikube/releases/latest/download/minikube-windows-amd64.exe' -UseBasicParsing
- jika sudah selesai buka system c dan periksa file minikubenya sudah didownload
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/c37c1bd4-1b2f-4636-8181-897fa6c1e129)
jika sudah copy langkah ini pastikan sudah close poweershell nya jika tidak akan terjadi error
> $oldPath = [Environment]::GetEnvironmentVariable('Path', [EnvironmentVariableTarget]::Machine)
if ($oldPath.Split(';') -inotcontains 'C:\minikube'){
  [Environment]::SetEnvironmentVariable('Path', $('{0};C:\minikube' -f $oldPath), [EnvironmentVariableTarget]::Machine)
}

- jika sudah buka cmd dan ketik
> minikube
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/982602ea-eb73-4366-8644-f02012084c53)
- ketik seperti dibawah dan pastikan sudah menjalankan docker
> minikube status
> minikube start
![image](https://github.com/saputrayudit/tekn-cloud-computing/assets/79730184/ac55af57-b022-467e-8cac-e17adc8558d6)
- jika sudah ketik seperti dibawah
> kubectl get po -A


