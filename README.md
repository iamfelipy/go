# GraphQL Server em Go

Projeto base: [devfullcycle/13-GraphQL](https://github.com/devfullcycle/13-GraphQL)

## Como rodar no Dev Container (VSCode)

Certifique-se de instalar a extensão "Dev Containers" no VSCode e abrir o projeto usando ela para uma melhor experiência de desenvolvimento.

### 1. Instale as dependências e rode o servidor

```sh
go mod tidy
go run cmd/server/server.go
```

### 2. Crie a tabela `categories` no SQLite3

Execute o comando abaixo dentro do container para criar a tabela:

```sh
sqlite3 data.db "create table categories (id string, name string, description string);"
```

### 3. Crie a tabela `courses` no SQLite3

Execute o comando abaixo dentro do container para criar a tabela:

```sh
sqlite3 data.db "create table courses (id string, name string, description string, category_id string);"
```