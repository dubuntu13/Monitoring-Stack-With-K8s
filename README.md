1. Clone the Repository:
```
git clone https://github.com/dubuntu13/K8s-Monitoring-Suite.git
cd K8s-Monitoring-Suite
```

2. Create the Namespace:
```
kubectl create namespace monitoring-stack
```

3. Set Up Persistent Storage:
```
kubectl apply -f storageclass.yml
cd prometheus-deploy
kubectl apply -f persistantvolumeClaim.yml
kubectl apply -f persistantvolume.yml
```

4. Deploy Prometheus:
```
kubectl apply -f prometheus-dep.yml
```

5. Access Services:

    Prometheus: http://nodeIP:30091
