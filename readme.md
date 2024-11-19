# 🌐 URL Shortener System

![AWS](https://img.shields.io/badge/AWS-Serverless-orange?style=flat&logo=amazonaws)  
![Status](https://img.shields.io/badge/Status-In%20Development-blue?style=flat&logo=github)  
![License](https://img.shields.io/badge/License-MIT-green?style=flat&logo=open-source-initiative)

## 📋 Sobre o Projeto

O **URL Shortener System** é uma aplicação **serverless** desenvolvida na AWS para encurtamento de URLs. Seu principal
objetivo é ser escalável, fácil de manter e com custos operacionais reduzidos, eliminando a necessidade de servidores
dedicados.

### 🚀 Principais Funcionalidades

1️⃣ **Gerar e armazenar URLs curtas**

- Criação de links curtos armazenados em um bucket **S3**.
- Registro de informações adicionais, como a URL original e tempo de expiração.

2️⃣ **Gerenciamento de redirecionamento**

- Verificação do código da URL curta.
- Validação do prazo de expiração antes de redirecionar o usuário.

---

## 🛠️ Arquitetura e Tecnologias

- **Serverless Framework** para automação e implantação.
- **AWS Lambda**: Funções para processamento de URLs.
- **AWS S3**: Armazenamento de dados.
- **AWS API Gateway**: Exposição das APIs.
- **AWS DynamoDB** *(opcional)*: Gerenciamento de metadados (se necessário).

---

## 🎯 Como Executar o Projeto?

### 🖥️ Pré-requisitos:

- [Node.js](https://nodejs.org/) (v14 ou superior)
- [AWS CLI](https://aws.amazon.com/cli/) configurado
- [Serverless Framework](https://www.serverless.com/) instalado globalmente

### 🏗️ Instalação:

1. Clone o repositório:
   ```bash
   git clone https://github.com/usuario/url-shortener.git
   cd url-shortener

2. Instale as dependências
   ```bash
   npm install

### 🚀 Deploy na AWS:

1. Configure o perfil do AWS CLI:
   ```bash
   aws configure
   
2. Realize o deploy:
   ```bash
   serverless deploy


### 🧪 Testes
Utilize ferramentas como [#Postman](https://www.postman.com) Para testar as APIs geradas pelo API Gateway.  
Exemplos de endpoints e payloads estão no arquivo docs/endpoints.md
