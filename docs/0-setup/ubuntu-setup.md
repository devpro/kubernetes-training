# Setup training environment on Ubuntu

## kubectl

```bash
# downloads the Google Cloud public signing key
sudo curl -fsSLo /usr/share/keyrings/kubernetes-archive-keyring.gpg https://packages.cloud.google.com/apt/doc/apt-key.gpg

# adds the Kubernetes apt repository
echo "deb [signed-by=/usr/share/keyrings/kubernetes-archive-keyring.gpg] https://apt.kubernetes.io/ kubernetes-xenial main" \
  | sudo tee /etc/apt/sources.list.d/kubernetes.list

# updates apt package index with the new repository and installs kubectl
sudo apt-get update
sudo apt-get install -y kubectl
```

→ [Official documentation](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)
