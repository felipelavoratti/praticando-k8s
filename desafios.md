# Desafios Kubernetes Lab

## Aula 2 - Primeiro contato

### Desafio 1

Criar um cluster Kubernetes local usando kind.

Status:
- [x] Concluído


### Desafio 2

Criar um Pod nginx.

Comando utilizado:

``bash
kubectl run nginx --image=nginx

[x] Status:

[x] Concluído
  Perguntas para revisar
- O que é um Pod?
-  Qual a diferença entre Pod e Container?
 - Quem recebe os comandos enviados pelo kubectl?
- Qual a função do API Server?
- Qual a função do namespace kube-system?
- Próximos desafios
-  Criar um Deployment
 - Escalar réplicas
 - Atualizar uma imagem
 - Fazer rollback
- Criar um Service
