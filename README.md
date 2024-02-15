# developers-summit-2024

Demo Repository.

- hello-server.yaml
  - A manifest file that the pod does not start
- hello-server-answer.yaml
  - The correct manifest

## How to use

1. Set up a Kubernetes cluster and execute the following command

```
kubectl apply -f hello-server.yaml
```

2. Please fix the manifest. The manifest should be able to access the hello-server using port-forward.

```
kubectl port-forward svc/hello-server 8080:8080
# Access the hello-server
curl localhost:8080
```
