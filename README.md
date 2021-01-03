# ec2_-kubernetes
curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
<br>
chmod +x ./kubectl
<br>

### kubectlコマンドとして実行できるように
sudo mv ./kubectl /usr/local/bin/kubectl<br>
<br>
sudo apt-get update && sudo apt-get install docker.io -y<br>

<br>
curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/<br>

<br>
minikube version<br>

<br>
sudo apt-get install -y conntrack<br>

<br>
sudo -i<br>

<br>
minikube start --vm-driver=none<br>
<br>
kubectl create deployment --image nginx my-nginx<br>
<br>
kubectl get pods<br>
<br>
### serviceが中継することで、コンテナのポートへ通信を受け渡してくれる
kubectl expose deployment my-nginx --port=80 --type=LoadBalancer<br>
<br>

# 参考サイト
https://www.radishlogic.com/kubernetes/running-minikube-in-aws-ec2-ubuntu/<br>
https://www.youtube.com/watch?v=PeRE90mSHQo<br>
