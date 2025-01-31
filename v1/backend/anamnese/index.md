---
title: 'Anamnese'
parent: 'Backend'
nav_order: 1
---

# Módulo: Anamnese

O módulo **Anamnese** gerencia os formulários de anamnese preenchidos pelos clientes, permitindo o registro de informações relevantes para a prestação de serviços.  

## ➡️ Funcionalidades Principais

- **Formulários de Anamnese**  
  Permite a criação e personalização de formulários para coleta de informações dos clientes.

- **Respostas de Anamnese**  
  Armazena as respostas enviadas pelos clientes, garantindo o histórico de informações.

- **Detalhamento das Respostas**  
  Estrutura as respostas em diferentes formatos, incluindo texto, múltipla escolha e booleano.

- **Assinaturas Eletrônicas**  
  Registra a assinatura do cliente para validação formal dos dados informados.

## ➡️ Estrutura do Módulo

```bash
/anamnese
│── index.md                     # Página inicial do módulo
│── anamnese_forms.md             # Gerenciamento de formulários de anamnese
│── anamnese_questions.md         # Perguntas dos formulários de anamnese
│── anamnese_question_items.md    # Opções de resposta para múltipla escolha
│── anamnese_answers.md           # Respostas preenchidas pelos clientes
│── anamnese_answers_details.md   # Detalhes específicos das respostas
│── anamnese_signatures.md        # Registro de assinaturas eletrônicas
```

## ➡️ Regras de Negócio

- Cada formulário de anamnese pode conter múltiplas perguntas de diferentes tipos.
- As respostas de anamnese devem estar associadas a um cliente e a um formulário específico.
- O sistema deve permitir apenas a edição de formulários antes de seu uso.
- Assinaturas eletrônicas são opcionais, mas recomendadas para formalização das respostas.

## ➡️ Endpoints Relacionados

| Método  | Rota                             | Descrição |
|---------|----------------------------------|----------------------------------|
| `GET`   | `/anamnese/forms`               | Lista todos os formulários disponíveis |
| `POST`  | `/anamnese/forms`               | Cria um novo formulário |
| `PUT`   | `/anamnese/forms/{id}`          | Atualiza um formulário existente |
| `DELETE`| `/anamnese/forms/{id}`          | Remove um formulário |
| `GET`   | `/anamnese/questions`           | Lista todas as perguntas cadastradas |
| `POST`  | `/anamnese/questions`           | Cria uma nova pergunta |
| `GET`   | `/anamnese/answers`             | Lista todas as respostas enviadas |

