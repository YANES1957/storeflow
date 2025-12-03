# StoreFlow PetShop - Microservices

Projeto de microserviços para gerenciamento de um petshop.

## Microserviços

- **order-service**: gerenciamento de pedidos
- **product-service**: cadastro de produtos
- **customer-service**: cadastro de clientes

## Tecnologias

- Java 17
- Spring Boot
- Maven
- Docker / Kubernetes (Rancher Desktop)

## Como rodar

1. Build: #!/bin/bash

# =========================
# Configurações iniciais
# =========================
GITHUB_USER="YANES1957"
REPO_NAME="storeflow"
PROJECT_DIR="/c/Users/Yan/storeflow"

# Criar pasta do projeto se não existir
mkdir -p /c/Users/Yan/storeflow
cd /c/Users/Yan/storeflow || exit

# Inicializar Git se não tiver
if [ ! -d ".git" ]; then
    git init
    git remote add origin https://github.com/YANES1957/storeflow.git
fi

# Criar README.md básico
cat > README.md <<EOL
# StoreFlow PetShop - Microservices

Projeto de microserviços para gerenciamento de um petshop.

## Microserviços

- **order-service**: gerenciamento de pedidos
- **product-service**: cadastro de produtos
- **customer-service**: cadastro de clientes

## Tecnologias

- Java 17
- Spring Boot
- Maven
- Docker / Kubernetes (Rancher Desktop)

## Como rodar

1. Build: `mvn clean package`
2. Build Docker: `docker build -t storeflow/<service>:latest .`
3. Rodar: `docker run -p <porta>:<porta> storeflow/<service>:latest`
