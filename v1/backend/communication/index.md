---
title: 'Communication'
parent: 'Backend'
nav_order: 1
---

# Módulo: Communication

O módulo **Communication** gerencia os meios de comunicação do sistema, incluindo notificações, mensagens pré-definidas e templates de e-mail.

## ➡️ Funcionalidades Principais

- **Templates de E-mail**  
  Gerenciamento de modelos de e-mail para comunicação automatizada.

- **Notificações**  
  Envio de notificações para clientes e administradores.

- **Mensagens Pré-Definidas**  
  Configuração de mensagens padrão para facilitar a comunicação.

- **Integração com WhatsApp**  
  Configuração e envio de mensagens automatizadas via WhatsApp.

## ➡️ Estrutura do Módulo

```bash
/communication
│── index.md                   # Página inicial do módulo
│── email_templates.md         # Modelos de e-mails
│── notifications.md           # Notificações e alertas
│── predefined_messages.md     # Mensagens pré-definidas
│── whatsapp_config.md         # Configuração do WhatsApp
```

## ➡️ Regras de Negócio

- Todas as notificações seguem um padrão configurável.
- Mensagens automáticas podem ser ativadas ou desativadas conforme a necessidade.
- O envio de notificações pode ser limitado por regras de permissão e preferências do usuário.

## ➡️ Endpoints Relacionados

| Método  | Rota                         | Descrição |
|---------|------------------------------|--------------------------------|
| `GET`   | `/notifications`             | Lista todas as notificações |
| `POST`  | `/notifications`             | Cria uma nova notificação |
| `GET`   | `/email_templates`           | Lista os templates de e-mail |
| `POST`  | `/email_templates`           | Cria ou atualiza um template |
| `GET`   | `/whatsapp/config`           | Retorna as configurações do WhatsApp |

