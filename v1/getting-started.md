---
title: "Guia Inicial"
nav_order: 2
---

# 🏁 Guia Inicial

Bem-vindo ao **Agenda Power**! Este documento apresenta um guia rápido para configurar e começar a utilizar o sistema.

## 📝 Requisitos

Antes de começar, certifique-se de que possui os seguintes requisitos instalados:

- **Node.js** (versão 18 ou superior)
- **Yarn** (ou outro gerenciador de pacotes)
- **PostgreSQL** (para ambiente local)
- **Docker** (opcional para ambiente isolado)

## 📌 Como Rodar o Projeto

### 1️⃣ **Clone o repositório**

```bash
git clone git@github.com:seu-repo.git
cd seu-projeto
```

### 2️⃣ **Instale as dependências**

```bash
yarn install
```

### 3️⃣ **Configurar as variáveis de ambiente**

Crie um arquivo `.env` baseado no `.env.example` e configure as credenciais do banco e integrações.

### 4️⃣ **Executar o banco de dados (Docker)**

```bash
docker-compose up -d
```

### 5️⃣ **Rodar as migrações do banco**

```bash
yarn prisma migrate dev
```

### 6️⃣ **Iniciar o servidor**

```bash
yarn start:dev
```

Agora o projeto estará rodando localmente em `http://localhost:3000`.

---

# 📂 Visão Geral do Backend

O **backend** do Agenda Power é construído em **NestJS** com **Prisma** para o gerenciamento do banco de dados. A API segue uma abordagem modular para facilitar a escalabilidade.

## 🚀 Tecnologias Utilizadas

- **Framework:** NestJS
- **Banco de Dados:** PostgreSQL com Prisma ORM
- **Autenticação:** JWT + OAuth (Google & Apple)
- **Mensageria:** Notificações via WhatsApp e Email
- **Armazenamento:** AWS S3 para uploads
- **CI/CD:** GitHub Actions para automação de deploys

## 🛠️ Arquitetura do Projeto

A estrutura do backend é baseada em módulos para melhor separação de responsabilidades:

```bash
/src
  |-- modules/         # Módulos principais
  |   |-- auth/        # Autenticação e controle de acesso
  |   |-- users/       # Gerenciamento de usuários
  |   |-- appointments/ # Agendamentos
  |   |-- payments/    # Pagamentos e transações
  |   |-- notifications/ # Notificações automáticas
  |
  |-- common/          # Componentes compartilhados
  |   |-- decorators/  # Decorators reutilizáveis
  |   |-- guards/      # Proteção de rotas e autenticação
  |   |-- filters/     # Manipulação de exceções
  |   |-- utils/       # Funções utilitárias
  |
  |-- prisma/          # Configuração do banco de dados
  |   |-- schema.prisma # Modelo de dados Prisma
  |
  |-- main.ts         # Arquivo principal do servidor
```

---

# 🏢 Módulos do Sistema

Cada módulo representa uma funcionalidade principal do sistema.

## 🔒 **Autenticação**

- Login via Google e Apple
- Tokens JWT com Refresh Token
- Controle de permissões por **roles**

## 🗓 **Agendamentos**

- Criar, editar e cancelar agendamentos
- Horários disponíveis e gestão de bloqueios
- Agendamentos recorrentes

## 💸 **Financeiro**

- Contas a pagar e receber
- Métodos de pagamento (PIX, Cartão, Boleto)
- Relatórios financeiros

## 💼 **Produtos & Serviços**

- Cadastro de serviços
- Controle de estoque de produtos
- Pacotes de serviços

## 📢 **Notificações**

- WhatsApp e E-mail automatizados
- Notificações de lembrete

---

# 📊 API & Endpoints

Estrutura RESTful seguindo boas práticas.

## **Exemplo de Endpoints**

| Método | Rota            | Descrição                       |
| ------ | --------------- | ------------------------------- |
| `POST` | `/auth/login`   | Autentica o usuário             |
| `GET`  | `/users/me`     | Retorna dados do usuário logado |
| `GET`  | `/appointments` | Lista todos os agendamentos     |
| `POST` | `/payments`     | Realiza um pagamento            |

Para mais detalhes, consulte a documentação da API [Swagger](backend/swagger.md) _(Em construção)_.

---

# 🛍️ Fluxos do Sistema

## **Fluxo de Agendamento**

1. Usuário escolhe serviço e profissional
2. Consulta horários disponíveis
3. Confirma agendamento
4. Notificação enviada por WhatsApp

## **Fluxo de Pagamento**

1. Usuário seleciona método de pagamento
2. API processa pagamento e confirma status
3. Atualização no financeiro e envio de recibo

---

# 🔗 Integrações

- **WhatsApp API** → Envio de mensagens automáticas
- **Gateway de Pagamento** → Processamento de transações
- **Google & Apple Login** → Autenticação simplificada

---

# 📜 Regras de Negócio

- **Cancelamentos** devem ocorrer com até 24h de antecedência
- **Agendamentos** só podem ser criados em horários disponíveis
- **Pagamentos** devem ser registrados imediatamente após a transação

---

# 🎯 Atualizações e Manutenção

Este documento será atualizado conforme novas funcionalidades forem implementadas.
