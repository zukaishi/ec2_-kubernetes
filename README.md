# ec2_-kubernetes
curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
<br>
chmod +x ./kubectl
<br>
kubectlコマンドとして実行できるように<br>
sudo mv ./kubectl /usr/local/bin/kubectl<br>