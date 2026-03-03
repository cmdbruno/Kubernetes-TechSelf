# 🚀 Kubernetes TechSelf - Projeto SRE

Projeto desenvolvido com foco em práticas de SRE utilizando Kubernetes e Helm para deploy de aplicação containerizada.

---

## 📌 Sobre o Projeto

O **Kubernetes-TechSelf** tem como objetivo demonstrar a criação, organização e implantação de uma aplicação em ambiente Kubernetes utilizando Helm como gerenciador de pacotes.

Este projeto simula um cenário real de mercado, aplicando boas práticas de:

- Infraestrutura como Código (IaC)
- Gerenciamento de releases com Helm
- Organização de manifests Kubernetes
- Estruturação de projeto DevOps/SRE

---

## 🛠️ Tecnologias Utilizadas

- Kubernetes
- Helm
- Docker
- YAML
- Linux

---

## 📂 Estrutura do Projeto

```bash
Kubernetes-TechSelf/
│
├── helm/
│   ├── Chart.yaml
│   ├── values.yaml
│   └── templates/
│       ├── deployment.yaml
│       ├── service.yaml
│       └── ingress.yaml (se aplicável)
```

---

## ⚙️ Pré-requisitos

Antes de executar o projeto, é necessário ter instalado:

- Kubernetes (Minikube, Kind ou Cluster)
- kubectl
- Helm v3+
- Docker

Verifique as versões:

```bash
kubectl version --client
helm version
docker --version
```

---

## 🚀 Como Executar o Projeto

### 1️⃣ Clonar o repositório

```bash
git clone https://github.com/cmdbruno/Kubernetes-TechSelf.git
cd Kubernetes-TechSelf
```

### 2️⃣ Instalar o Chart com Helm

```bash
helm install techsafe ./helm
```

### 3️⃣ Verificar os recursos criados

```bash
kubectl get all
```

### 4️⃣ Verificar status do release

```bash
helm list
```

---

## 🔄 Atualizar o Deploy

Caso faça alterações nos templates ou `values.yaml`:

```bash
helm upgrade techsafe ./helm
```

---

## 🗑️ Remover o Deploy

```bash
helm uninstall techsafe
```

---

## 📊 Boas Práticas Aplicadas

- ✔ Separação de templates
- ✔ Uso de `values.yaml` para customização
- ✔ Deploy versionado via Helm
- ✔ Estrutura organizada para ambientes futuros (dev, hml, prod)

---

## 🎯 Objetivo Profissional

Este projeto faz parte do meu portfólio profissional como **Administrador de Servidores Linux / SRE**, demonstrando conhecimentos em:

- Orquestração de containers
- Deploy automatizado
- Gerenciamento de aplicações em Kubernetes
- Estruturação de projetos DevOps

---

## 👨‍💻 Autor

**Bruno Almeida de Carvalho**  
Administrador de Servidores Linux | Infraestrutura | Kubernetes | DevOps  

---

⭐ Se este projeto foi útil para você, deixe uma estrela no repositório!
