---
title: Introdução
nav_order: 1
---
# **Documentação – AgendaPower**

### **📂 Estrutura da Documentação**

- **🔹 Visão Geral** → Objetivo e tecnologias utilizadas
- **🔹 Arquitetura** → Estrutura do projeto e pastas
- **🔹 Módulos** → Funcionalidades principais do sistema
- **🔹 API & Endpoints** → Estrutura e exemplos de requisições
- **🔹 Fluxos do Sistema** → Como os módulos interagem
- **🔹 Integrações** → APIs externas e serviços conectados
- **🔹 Regras de Negócio** → Validações e regras aplicáveis

---

## **📖 Visão Geral**

Sistema desenvolvido para **[finalidade do projeto]**, oferecendo **[principais recursos]**.  
Utilizamos tecnologias modernas para garantir **escalabilidade** e **segurança**.

### **🚀 Tecnologias**

- **Backend:** NestJS, Prisma, PostgreSQL
- **Frontend:** React Native
- **Autenticação:** Google & Apple Login
- **Infraestrutura:** AWS (EC2, S3, RDS)
- **Pagamento:** [Gateway de pagamento]

---

## **🛠 Arquitetura**

A estrutura do projeto segue um modelo **modular**, garantindo organização e escalabilidade.

{Estrutura}

---

## **📦 Módulos**

Cada módulo representa uma funcionalidade principal do sistema.

### **🔹 Autenticação**

- Login via Google e Apple
- Tokens JWT com Refresh Token
- Controle de permissões por **roles**

### **🔹 Agendamentos**

- Criar, editar e cancelar agendamentos
- Horários disponíveis e gestão de bloqueios
- Agendamentos recorrentes

### **🔹 Financeiro**

- Contas a pagar e receber
- Métodos de pagamento (PIX, Cartão, Boleto)
- Relatórios financeiros

### **🔹 Produtos & Serviços**

- Cadastro de serviços
- Controle de estoque de produtos
- Pacotes de serviços

### **🔹 Notificações**

- WhatsApp e E-mail automatizados
- Notificações de lembrete

---

## **🖥 API & Endpoints**

Estrutura RESTful seguindo boas práticas.

### **🔹 Exemplo de Endpoints**

| Método | Rota            | Descrição                       |
| ------ | --------------- | ------------------------------- |
| `POST` | `/auth/login`   | Autentica o usuário             |
| `GET`  | `/users/me`     | Retorna dados do usuário logado |
| `GET`  | `/appointments` | Lista todos os agendamentos     |
| `POST` | `/payments`     | Realiza um pagamento            |

- `- [Documentação da API (Swagger)](backend/swagger.md) *(Em construção)*`

---

## **🔄 Fluxos do Sistema**

### **🔹 Fluxo de Agendamento**

1. Usuário escolhe serviço e profissional
2. Consulta horários disponíveis
3. Confirma agendamento
4. Notificação enviada por WhatsApp

### **🔹 Fluxo de Pagamento**

1. Usuário seleciona método de pagamento
2. API processa pagamento e confirma status
3. Atualização no financeiro e envio de recibo

---

## **🔗 Integrações**

- **WhatsApp API** → Envio de mensagens automáticas
- **Gateway de Pagamento** → Processamento de transações 
- **Google & Apple Login** → Autenticação simplificada

---

## **📜 Regras de Negócio**

- **Cancelamentos** devem ocorrer com até 24h de antecedência
- **Agendamentos** só podem ser criados em horários disponíveis
- **Pagamentos** devem ser registrados imediatamente após a transação

---

## **📍 Telas e Fluxos**

(Tela inicial, telas principais do sistema, descrição dos fluxos visuais)

---

## **📌 Atualizações e Manutenção**

Este documento será atualizado conforme novas funcionalidades forem implementadas.

---

### **✅ Conclusão**

Com o tempo, novas seções podem ser adicionadas conforme necessário.