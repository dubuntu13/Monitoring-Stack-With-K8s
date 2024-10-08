# monitoringStack-cluster
Here’s a step-by-step guide to get started with the K8s Monitoring Suite:

    Clone the Repository:

    bash

git clone https://github.com/dubuntu13/K8s-Monitoring-Suite.git
cd K8s-Monitoring-Suite

Create the Namespace:

bash

kubectl apply -f namespace.yaml

Set Up Persistent Storage:

bash

kubectl apply -f storage.yaml

Deploy Prometheus:

bash

kubectl apply -f prometheus.yaml

Deploy Zabbix, Grafana, and Loki (Follow instructions in each specific YAML file in the repository):

bash

kubectl apply -f zabbix.yaml

Access Services:

    Prometheus: http://<node-ip>:30091
