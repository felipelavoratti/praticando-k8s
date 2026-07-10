# Checkpoint - Kubernetes Lab

## Estado atual

Data: 2026-07-10

## Ambiente

- Windows 10
- WSL funcionando
- Docker funcionando
- kubectl instalado
- kind instalado

## Cluster

Cluster criado:
kind create cluster --name homedevops

Node:
kubectl get nodes

Resultado esperado:
homedevops-control-plane Ready


O que já foi feito
[x] Instalação do kubectl

[x] Instalação do kind

[x] Criação do cluster Kubernetes

[x] Primeiro Pod criado:

kubectl run nginx --image=nginx

[x] Entendido:

kubectl conversa com API Server
API Server consulta o etcd
kube-system contém componentes internos do Kubernetes
Pod não é igual a container
Imagem Docker pode ficar em cache no node
GitHub


Aula 3 - Investigação de Pods

Objetivos:

kubectl get pod -o wide
kubectl describe pod
kubectl logs
kubectl exec
entender IP do Pod
entender Node
analisar eventos
Primeiro comando para executar ao retornar
kubectl get pods


---
> "Quero continuar meu laboratório Kubernetes. Já fiz o checkpoint. Estou na Aula 3: investigação de Pods."

aprender o fluxo Git pelo terminal e manter esse checkpoint atualizado automaticamente com 'git commit'
