## 1) python docker 
```sh
docker pull caonguyen14/taipy:latest
docker run caonguyen14/taipy:latest
```

## 2) github ci
change hello world -> hello taipy on hello.py and waiting github action run

```sh
docker pull caonguyen14/taipy:latest
docker run caonguyen14/taipy:latest
```

## 3) ftp server on k8s
kubectl apply -f k8s-ftp-server/deployment.yaml

```sh
kubectl get pod -A | grep ftp
kubectl port-forward deploy/my-ftp 8081:21
access ftp://127.0.0.1:8021 user/pass1234
```
