# kubectl commands

## General convention

```bash
kubectl <action> <object_type> <arguments>
```

→ [kubectl Cheat Sheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)

## Most common commands

Command | Action
------- | ------
`kubectl apply -f <manifest_file>.yaml` | Apply the Kubernetes definition written in a manifest file (YAML)
`kubectl cluster-info --context <context_name>` | Display Kubernetes cluster information for a given context (see config.json file)
`kubectl get nodes` | Displays Kubernetes cluster nodes
`kubectl get ns` | Displays namespaces

## Recipes

### Deploy a nginx web server

```bash
# creates a deployment based on nginx image
kubectl create deployment nginx --image=nginx --port=80

# exposes the service through a nodeport on port 30000
kubectl create service nodeport nginx --tcp=80:80 --node-port=30000

# displays all objects
kubectl get all

# accesses the website (should work from WSL and Windows)
curl localhost:30000

# cleans-up
kubectl delete svc,deploy nginx
```
