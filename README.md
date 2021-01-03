# ec2_-kubernetes
curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
<br>
chmod +x ./kubectl
<br>

# kubectlコマンドとして実行できるように
sudo mv ./kubectl /usr/local/bin/kubectl
<br>
sudo apt-get update && sudo apt-get install docker.io -y
<br>
curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/
<br>
minikube version
<br>
sudo -i
<br>
minikube start --vm-driver=none
<br>

# 参考サイト
https://www.radishlogic.com/kubernetes/running-minikube-in-aws-ec2-ubuntu/
