# Установка Minikube
### Установка kubectl
```sh
###################################################################################################################################
sudo apt-get update && sudo apt-get install -y apt-transport-https
###################################################################################################################################
root@Ubunty-22:/home/noneraspad# sudo apt-get update && sudo apt-get install -y apt-transport-https
Hit:1 http://ru.archive.ubuntu.com/ubuntu jammy InRelease                                        
Hit:2 https://download.docker.com/linux/ubuntu jammy InRelease                                   
Get:3 http://security.ubuntu.com/ubuntu jammy-security InRelease [110 kB]
Get:4 http://security.ubuntu.com/ubuntu jammy-security/main amd64 Packages [1 051 kB]
Get:5 http://ru.archive.ubuntu.com/ubuntu jammy-updates InRelease [119 kB]
Hit:6 http://ru.archive.ubuntu.com/ubuntu jammy-backports InRelease     
Get:7 http://ru.archive.ubuntu.com/ubuntu jammy-updates/main i386 Packages [547 kB]
Get:8 http://ru.archive.ubuntu.com/ubuntu jammy-updates/main amd64 Packages [1 263 kB]
Get:9 http://security.ubuntu.com/ubuntu jammy-security/main i386 Packages [383 kB]              
Get:10 http://security.ubuntu.com/ubuntu jammy-security/universe amd64 Packages [823 kB]
Get:11 http://ru.archive.ubuntu.com/ubuntu jammy-updates/universe i386 Packages [675 kB]
Get:12 http://ru.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 Packages [1 020 kB]                              
Get:13 http://security.ubuntu.com/ubuntu jammy-security/universe i386 Packages [580 kB]                                  
Fetched 6 571 kB in 7s (881 kB/s)                                                                                        
Reading package lists... Done
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
apt-transport-https is already the newest version (2.4.11).
0 upgraded, 0 newly installed, 0 to remove and 8 not upgraded.
root@Ubunty-22:/home/noneraspad#

###################################################################################################################################
curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
###################################################################################################################################
root@Ubunty-22:/home/noneraspad# curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
Warning: apt-key is deprecated. Manage keyring files in trusted.gpg.d instead (see apt-key(8)).
OK
root@Ubunty-22:/home/noneraspad#

###################################################################################################################################
echo "deb https://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee -a /etc/apt/sources.list.d/kubernetes.list
###################################################################################################################################
root@Ubunty-22:/home/noneraspad# echo "deb https://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee -a /etc/apt/sources.list.d/kubernetes.list
deb https://apt.kubernetes.io/ kubernetes-xenial main
root@Ubunty-22:/home/noneraspad#

###################################################################################################################################
sudo apt-get update
###################################################################################################################################
root@Ubunty-22:/home/noneraspad# sudo apt-get update
Hit:1 http://security.ubuntu.com/ubuntu jammy-security InRelease                                                         
Hit:2 https://download.docker.com/linux/ubuntu jammy InRelease                                                           
Hit:4 http://ru.archive.ubuntu.com/ubuntu jammy InRelease                                           
Get:3 https://packages.cloud.google.com/apt kubernetes-xenial InRelease [8 993 B]
Hit:5 http://ru.archive.ubuntu.com/ubuntu jammy-updates InRelease
Hit:6 http://ru.archive.ubuntu.com/ubuntu jammy-backports InRelease
Get:7 https://packages.cloud.google.com/apt kubernetes-xenial/main amd64 Packages [69,9 kB]
Fetched 78,9 kB in 3s (31,4 kB/s)    
Reading package lists... Done
W: https://apt.kubernetes.io/dists/kubernetes-xenial/InRelease: Key is stored in legacy trusted.gpg keyring (/etc/apt/trusted.gpg), see the DEPRECATION section in apt-key(8) for details.
root@Ubunty-22:/home/noneraspad#

###################################################################################################################################
sudo apt-get install -y kubectl
###################################################################################################################################
```

### Установка Minikube
root@Ubunty-22:/home/noneraspad# curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 \
> curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 \
  && chmod +x minikube
```sh
|  % Total  | % Received | % Xferd | Average |  Speed |   Time  |  Time   |   Time  | Current |
| --------- | ---------- | ------- | ------- | ------ | ------- | ------- | ------- | ------- |
| --------- | ---------- | ------- |  Dload  | Upload |  Total  |  Spent  |   Left  |  Speed  |
|  34 89.3M |  34 30.7M  |    0    |  1316k  |    0   | 0:01:09 | 0:00:23 | 0:00:46 |  2048k  |
```




### Настройка автодополнения команд



### Краткое знакомство с кластером
