# -Kubernetes
 # Kubernetes Installation on Ubuntu Server [Master node + Worker node]
 **First you have to launch two instances one is for the Master node and one is for the worker node.**
 **for the master node take (t2.small or t2.medium )instance type and for worker node take (t2.micro or you take any.)**
 **After the launching instances follow the followings**
 ## (Run this all commands on both nodes i.e.master as well as worker node)
```
1.  sudo apt-get update –y
```
```
2.  sudo apt-get install docker.io –y
```
```
3.  sudo apt-get install -y apt-transport-https ca-certificates curl gnupg
```
```
4.  sudo mkdir -p /etc/apt/keyrings
```
```
5.  curl -fsSL https://pkgs.k8s.io/core:/stable:/v1.30/deb/Release.key | sudo gpg --dearmor -o /etc/apt/keyrings/kubernetes-apt-keyring.gpg
```
```
6.  sudo chmod 644 /etc/apt/keyrings/kubernetes-apt-keyring.gpg```
```
```
7.  echo 'deb [signed-by=/etc/apt/keyrings/kubernetes-apt-keyring.gpg] https://pkgs.k8s.io/core:/stable:/v1.30/deb/ /' | sudo tee /etc/apt/sources.list.d/kubernetes.list
```
```
8. sudo chmod 644 /etc/apt/sources.list.d/kubernetes.list
```
```
9.  sudo apt-get update
```
```
10. sudo apt-get install -y kubectl kubeadm kubelet
```


