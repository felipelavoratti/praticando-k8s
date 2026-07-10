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

# Kubernetes Lab

Laboratório de estudos em Kubernetes, DevOps e Cloud.

## Objetivo

Este repositório documenta minha jornada de aprendizado em Kubernetes e tecnologias relacionadas, com foco em prática.

O objetivo é evoluir gradualmente de um ambiente local para um ambiente semelhante ao utilizado em produção.

## Ambiente

* Sistema Operacional: Windows 10 + WSL
* Docker
* kind (Kubernetes in Docker)
* kubectl

## Estrutura do projeto

```text
kubernetes-lab/
├── README.md
├── anotacoes.md
├── desafios.md
├── manifests/
└── aulas/
```

## Progresso

### Aula 1 – Preparação do ambiente

* [x] Instalação do Docker
* [x] Instalação do kubectl
* [x] Instalação do kind
* [x] Criação do primeiro cluster Kubernetes

### Aula 2 – Conhecendo o cluster

* [x] `kubectl cluster-info`
* [x] `kubectl get nodes`
* [x] `kubectl get namespaces`
* [x] `kubectl get pods -A`
* [x] Primeiro Pod com nginx

### Próximos passos

* [ ] Entender Pods
* [ ] Deployments
* [ ] ReplicaSets
* [ ] Services
* [ ] Ingress
* [ ] ConfigMaps
* [ ] Secrets
* [ ] Persistent Volumes
* [ ] Helm
* [ ] GitHub Actions
* [ ] ArgoCD

## Comandos aprendidos

``bash
kubectl cluster-info

kubectl get nodes

kubectl get namespaces

kubectl get pods

kubectl get pods -A

kubectl run nginx --image=nginx

kubectl delete pod nginx
``

## Aprendizados

* O `kubectl` se comunica com o API Server.
* O estado do cluster é armazenado no `etcd`.
* O namespace `kube-system` contém os componentes internos do Kubernetes.
* Um Pod não é o mesmo que um container.
* A primeira execução de uma imagem pode demorar porque ela precisa ser baixada; nas próximas execuções a imagem já está armazenada no node.

## Objetivo final

Construir um laboratório completo contendo:

* Kubernetes
* Docker
* PostgreSQL
* Redis
* Ingress
* Prometheus
* Grafana
* Loki
* GitHub Actions
* ArgoCD
* Terraform
* Cloud
