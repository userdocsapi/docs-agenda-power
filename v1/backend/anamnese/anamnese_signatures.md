---
title: 'Anamnese signatures'
parent: 'Anamnese'
nav_order: 1
---

# Anamnese signatures (Assinaturas da Anamnese)

O módulo **Anamnese Signatures** gerencia as assinaturas digitais associadas aos formulários de anamnese preenchidos pelos clientes. Essas assinaturas garantem a validade e autenticidade dos registros.

## ➡️ Funcionalidades Principais

- **Registro de Assinaturas Digitais**  
  Armazena a assinatura digital do cliente no momento do preenchimento do formulário.

- **Validação de Assinaturas**  
  Garante que cada anamnese assinada seja vinculada corretamente ao cliente e ao formulário preenchido.

- **Armazenamento Seguro**  
  Salva os registros de assinatura com informações do dispositivo utilizado, data e hora da assinatura.

## ➡️ Estrutura do Módulo

```bash
/anamnese/anamnese_signatures.md  # Gerenciamento de assinaturas digitais da anamnese
```

## ➡️ Tabela de Dados

| Campo                    | Tipo        | Descrição |
|--------------------------|------------|------------------------------------------------|
| `id`                     | `UUID`     | Identificador único da assinatura. |
| `anamnese_form_id`       | `UUID`     | Referência ao formulário de anamnese. |
| `customer_id`            | `UUID`     | Referência ao cliente que assinou. |
| `signed_at`              | `Datetime` | Data e hora da assinatura. |
| `signed_local_file_path` | `String`   | Caminho do arquivo da assinatura local. |
| `signed_device_info`     | `String`   | Informações do dispositivo utilizado. |
| `signed_device_model`    | `String`   | Modelo do dispositivo utilizado. |
| `signed_platform`        | `String`   | Plataforma utilizada (Web, Mobile, etc.). |
| `created_at`             | `Datetime` | Data de criação do registro. |
| `updated_at`             | `Datetime` | Última atualização do registro. |

## ➡️ Endpoints Relacionados

| Método  | Rota                                       | Descrição |
|---------|-------------------------------------------|--------------------------------------|
| `POST`  | `/anamnese/signatures`                   | Registra uma nova assinatura. |
| `GET`   | `/anamnese/signatures/{id}`              | Retorna os detalhes de uma assinatura. |
| `GET`   | `/anamnese/signatures?customer_id={id}`  | Lista assinaturas de um cliente. |

A funcionalidade de assinaturas da anamnese é essencial para garantir a integridade das informações e a validação legal dos documentos preenchidos pelos clientes.