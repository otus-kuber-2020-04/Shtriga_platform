# Shtriga_platform

# Домашнее задание лекции 02

собрать образ:
```sh
cd kubernetes-intro/web
docker build -t kirsan/otus-hw02:web .
```

запустить контейнер через docker engine:
```sh
docker run -d -p 8000:8000 kirsan/otus-hw02:web
```

запустить pod:
```sh
kubect apply -f kubernetes-intro/web-pod.yaml
```
