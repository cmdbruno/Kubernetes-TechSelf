# 🚀 Kubernetes TechSafe - Projeto SRE

## 📌 Sobre o Projeto

Este projeto demonstra a implementação de uma aplicação baseada em microsserviços utilizando Kubernetes com gerenciamento via Helm.

A solução contempla práticas de SRE voltadas para:

- Alta disponibilidade
- Monitoramento de saúde (Liveness Probe)
- Automação de backups com CronJob
- Gerenciamento de deploy com Helm

---

## 🏗️ Arquitetura da Solução

- Kubernetes (Minikube)
- Helm Chart customizado
- Deployment configurável via values.yaml
- Service ClusterIP
- Liveness Probe HTTP
- CronJob automatizado para backup

Fluxo:

Usuário → Service → Pod (Nginx)  
Kubelet → Liveness Probe → Health Check  
CronJob → Job → Backup automatizado

---

## 🛠️ Tecnologias Utilizadas

- Kubernetes
- Helm
- Docker
- Minikube
- kubectl

---

## 🚀 Como Executar o Projeto

### 1️⃣ Iniciar o cluster Kubernetes

```bash
minikube start --memory=4096 --cpus=2 --driver=docker
