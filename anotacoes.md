# Anotações Kubernetes Lab

## Aula 1 - Preparação do ambiente

Ambiente utilizado:

- Windows 10
- WSL
- Docker
- kind
- kubectl

## Aula 2 - Prática com Kubernetes

### Comandos utilizados

Ver informações do cluster:

## Comandos

kubectl cluster-info

Listar nodes:

kubectl get nodes

Listar namespaces:

kubectl get namespaces

Listar todos os pods:

kubectl get pods -A

Criar primeiro Pod:

kubectl run nginx --image=nginx

Remover Pod:

kubectl delete pod nginx
Conceitos aprendidos
Cluster

Conjunto de máquinas responsáveis por executar aplicações e controlar o Kubernetes.

Node

Máquina onde os componentes Kubernetes executam.

Pod

Menor unidade de execução do Kubernetes.

Um Pod pode conter um ou mais containers.

Namespace

Forma de separar recursos dentro do cluster.

Exemplo:

default → aplicações do usuário
kube-system → componentes internos do Kubernetes
API Server

Porta de entrada do Kubernetes.

O kubectl envia comandos para o API Server.

Fluxo:

kubectl → API Server → etcd → resposta

Observação

O primeiro download da imagem nginx demorou mais porque a imagem ainda não estava no node.

Nas próximas execuções, o container iniciou mais rápido, com imagem já baixada anteriormente.

---
