# Kubernetes cluster setup

In order to practice, we need at least a Kubernetes cluster to work on, with admin permissions.

:bulb: Before using a real environment, that may come with a price and a professional procedure, it is easier to start small with a sandbox environment.

## Documentation

- [k3d](https://k3d.io/)
- [kataCoda playground](https://www.katacoda.com/courses/kubernetes/playground)
- [kind](https://kind.sigs.k8s.io/)

## Exercise

### Success criteria

- [ ] Have the command `kubectl get nodes` display at least one element
- [ ] Find the correct context name to execute `kubectl cluster-info --context <context_name>`
- [ ] Display Kubernetes cluster version
- [ ] Find and display kubectl configuration file

### Tips

- Docker should be installed first (except for remote environment like the one provided by KataKoda)

### Help

- [Ubuntu based configuration](../0-help/ubuntu-based-configuration.md)
- Use [kind-cluster-config.yml](../../manifests/kind-cluster-config.yml) to avoid issues with WSL
or restart WSL if a service can't be reached from Windows

## Next

Jump to next section: [3. Dashboard](../3-dashboard/dashboard.md)
