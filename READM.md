# Kubernetes Lab

Laboratório de estudos DevOps e Kubernetes.

## Ambiente

- Windows 10
- WSL
- Docker
- kind
- kubectl

## Objetivo

Aprender Kubernetes na prática, evoluindo de um ambiente local para conceitos utilizados em produção.

## Progresso

### Kubernetes

- [x] Instalar kubectl
- [x] Instalar kind
- [x] Criar primeiro cluster
- [x] Criar primeiro Pod nginx

### Próximos passos

- [ ] Entender Pods
- [ ] Deployments
- [ ] Services
- [ ] Volumes
- [ ] Ingress
- [ ] CI/CD
- [ ] GitOps

## Primeiro laboratório

Cluster criado usando kind:
kind create cluster --name homedevops

Primeiro Pod:
kubectl run nginx --image=nginx

Verificar Pods:
kubectl get pods
