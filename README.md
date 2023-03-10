### ISIS_Lab4
Kubernetes. Знакомство с абстракциями pod, replicaset, deployment resources

### Инструкция Docker
Склонировать репозиторий
```
git clone https://github.com/shadowHD-bit/ISIS_LAB4.git
```
Создать образ
```
docker build . -t nodejs-docker
```
Запустить образ
```
docker run -p 80:8080 -d nodejs-docker
```
Перейти на локальную страницу
```
localhost:80
```

### Инструкция K8s
Склонировать репозиторий
```
git clone https://github.com/shadowHD-bit/ISIS_LAB4.git
```
Создать Pod
```
kubectl apply -f .\node-pod.yaml
```
Создать Deployment
```
kubectl apply -f .\node-deployment.yaml
```
Создать ReplicaSet
```
kubectl apply -f .\node-replicaset.yaml
```

Или использовать команду
```
kubectl create deployment isis4-dep --image alx5874/my-repository:nodejs-docker-isis4
```

Посмотреть информацию о ресурсах созданного Deployment
```
kubectl describe node
```
