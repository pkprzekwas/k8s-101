# k8s 101

## Minikube

https://minikube.sigs.k8s.io/docs/

### Installing minikube addons

```bash
# enabling k8s dashboard
minikube addons enable dashboard

# enabling metrics server
minikube addons enable metrics-server
```

### Using k8s dashboard

```bash
# port forwarding
kubectl -n kubernetes-dashboard port-forward svc/kubernetes-dashboard 8088:80
```

After setting up port forward in one of your bash sessions open your browser of choice and go to `localhost:8088`.

## Step 01

```bash
nest new --skip-git testapp
```
