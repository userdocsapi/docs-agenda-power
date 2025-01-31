---
title: 'Authentication'
parent: 'Backend'
nav_order: 1
---

# Módulo: Authentication

O módulo **Authentication** gerencia a autenticação e controle de acesso dos usuários ao sistema.

## ➡️ Funcionalidades Principais

- **Autenticação de Usuários**  
  Login seguro utilizando credenciais ou autenticação via terceiros (Google, Apple, etc.).

- **Controle de Permissões**  
  Definição de níveis de acesso por meio de **roles** e permissões específicas.

- **Gerenciamento de Sessões**  
  Implementação de tokens JWT e Refresh Token para manter a segurança e controle das sessões.

- **Registro e Recuperação de Senha**  
  Cadastro de novos usuários e recuperação de acesso por e-mail.

## ➡️ Estrutura do Módulo

```bash
/authentication
│── index.md                        # Página inicial do módulo
│── permissions.md                   # Gerenciamento de permissões
│── user_account_status.md           # Status e ativação de contas de usuários
│── user_logs.md                     # Logs de autenticação e ações do usuário
│── user_roles.md                    # Definição e gerenciamento de roles
│── user_roles_permission.md         # Associação de permissões a roles
│── user_roles_theme.md              # Configuração de temas por usuário
│── users.md                         # Gerenciamento de usuários
```

## ➡️ Regras de Negócio

- Apenas usuários autenticados podem acessar funcionalidades restritas do sistema.
- Tokens de acesso têm um tempo de expiração configurável.
- Permissões são atribuídas com base no cargo do usuário dentro do sistema.
- O sistema deve registrar tentativas de login para auditoria e segurança.

## ➡️ Endpoints Relacionados

| Método  | Rota                             | Descrição |
|---------|----------------------------------|----------------------------------|
| `POST`  | `/auth/login`                   | Autentica um usuário e retorna um token |
| `POST`  | `/auth/register`                | Registra um novo usuário |
| `POST`  | `/auth/logout`                  | Invalida a sessão do usuário |
| `POST`  | `/auth/refresh`                 | Gera um novo token JWT |
| `POST`  | `/auth/password/reset`          | Envia um e-mail para redefinição de senha |
| `POST`  | `/auth/password/update`         | Atualiza a senha do usuário |
| `GET`   | `/auth/user`                    | Retorna os dados do usuário autenticado |

---

Este módulo é essencial para garantir a segurança e o gerenciamento de acessos ao sistema.