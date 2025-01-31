---
title: 'Guia de Inicialização'
nav_order: 2
---

# Guia de Inicialização

Este documento fornece um passo a passo para configurar e executar o projeto, além de informações sobre o Swagger para documentação da API.

## ➡️ Pré-requisitos
Antes de iniciar, certifique-se de ter instalado:

- **Node.js** (versão recomendada: `>=18.x`)
- **Yarn** (versão recomendada: `>=1.x`)
- **Docker** (opcional, para rodar o banco de dados localmente)
- **PostgreSQL** (caso prefira rodar o banco sem Docker)

## ➡️ Configuração do Projeto
1. **Clone o repositório**
   ```bash
   git clone https://github.com/seu-repo.git
   cd nome-do-projeto
   ```

2. **Instale as dependências**
   ```bash
   yarn install
   ```

3. **Configure as variáveis de ambiente**
   - Copie o arquivo `.env.example` e renomeie para `.env`
   - Preencha os valores necessários, como conexão com o banco de dados

4. **Rodando o Banco de Dados com Docker** *(opcional)*
   ```bash
   docker-compose up -d
   ```

5. **Executando as migrações do Prisma**
   ```bash
   yarn prisma migrate dev
   ```

6. **Inicie o servidor**
   ```bash
   yarn start:dev
   ```

## ➡️ Acessando a Documentação da API (Swagger)
O Swagger é utilizado para fornecer uma interface interativa da API. Para acessá-lo:

- Inicie o servidor e acesse:
  ```
  http://localhost:3000/api/docs
  ```

No Swagger, você pode:
- Visualizar todos os endpoints disponíveis
- Testar requisições diretamente
- Entender os parâmetros necessários para cada endpoint

## ➡️ Estrutura do Projeto
```bash
/nome-do-projeto
│── /backend              # API NestJS
│    ├── /src
│    │    ├── /modules   # Módulos principais
│    │    ├── /common    # Utilitários globais
│    │    ├── main.ts    # Arquivo principal
│    ├── /prisma         # Configuração do Prisma
│    ├── .env            # Arquivo de configuração
│    ├── package.json    # Dependências do projeto
│── /frontend            # Aplicativo React Native
│── /docs                # Documentação do projeto
```

## ➡️ Comandos Úteis

| Comando | Descrição |
|---------|------------|
| `yarn dev` | Inicia o servidor em modo de desenvolvimento |
| `yarn build` | Compila o projeto para produção |
| `yarn prisma studio` | Acessa o banco de dados via interface gráfica |
| `yarn test` | Executa os testes automatizados |

## Conclusão
Seguindo esses passos, o ambiente estará configurado e pronto para desenvolvimento. Caso tenha dúvidas, consulte a documentação interna ou entre em contato com a equipe técnica.