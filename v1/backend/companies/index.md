---
title: 'Companies'
parent: 'Backend'
nav_order: 1
---

# Módulo: Companies

O módulo **Companies** gerencia as informações e configurações das empresas cadastradas no sistema.

## ➡️ Funcionalidades Principais

- **Cadastro e Gestão de Empresas**  
  Criação, atualização e exclusão de empresas no sistema.

- **Configuração de Página Pública**  
  Personalização da página pública da empresa, incluindo informações de contato, redes sociais e agendamentos.

- **Gestão de Funcionários e Papéis**  
  Administração de colaboradores, definição de cargos e permissões.

## ➡️ Estrutura do Módulo

```bash
/companies
│── index.md                        # Página inicial do módulo
│── companies.md                     # Gestão de empresas
│── company_page_bio.md              # Informações da página pública
│── company_page_bio_instagram.md    # Integração com Instagram
│── company_page_bio_whatsapp.md     # Integração com WhatsApp
│── company_settings.md              # Configurações gerais da empresa
│── employee_roles.md                # Gestão de papéis e permissões
│── employees.md                      # Gerenciamento de funcionários
```

## ➡️ Regras de Negócio

- Cada empresa pode ter múltiplos funcionários, com permissões específicas.
- A página pública pode ser personalizada com cores, logotipo e redes sociais.
- Apenas administradores podem editar as configurações da empresa.
- As empresas podem ativar ou desativar o agendamento online.

## ➡️ Endpoints Relacionados

| Método  | Rota                                     | Descrição |
|---------|------------------------------------------|----------------------------------|
| `GET`   | `/companies`                            | Lista todas as empresas |
| `POST`  | `/companies`                            | Cria uma nova empresa |
| `PUT`   | `/companies/{id}`                       | Atualiza os dados de uma empresa |
| `DELETE`| `/companies/{id}`                       | Remove uma empresa |
| `GET`   | `/companies/{id}/settings`             | Obtém configurações da empresa |
| `PUT`   | `/companies/{id}/settings`             | Atualiza configurações |
| `GET`   | `/companies/{id}/employees`            | Lista funcionários da empresa |
| `POST`  | `/companies/{id}/employees`            | Adiciona um funcionário |
| `DELETE`| `/companies/{id}/employees/{employee_id}` | Remove um funcionário |

---

Essa documentação cobre os principais aspectos do módulo **Companies**. Caso precise de ajustes ou mais detalhes, basta me avisar!

