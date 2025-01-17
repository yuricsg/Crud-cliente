# CRUD de Clientes - Spring Boot

Este projeto é uma aplicação **CRUD** (Criar, Ler, Atualizar, Deletar) de clientes utilizando **Spring Boot**, **JPA** (Java Persistence API) e **H2 Database**. A aplicação permite gerenciar informações de clientes, como nome, CPF, renda, data de nascimento e quantidade de filhos, através de uma API REST.

## Funcionalidades

- **Cadastrar um novo cliente**: Endpoint para inserir novos clientes na base de dados.
- **Listar todos os clientes**: Endpoint para listar todos os clientes cadastrados, com suporte à paginação.
- **Consultar um cliente**: Endpoint para buscar um cliente específico pelo ID.
- **Atualizar dados de um cliente**: Endpoint para atualizar as informações de um cliente existente.
- **Deletar um cliente**: Endpoint para remover um cliente do banco de dados.

## Tecnologias Utilizadas

- **Spring Boot**: Framework para desenvolvimento de aplicações Java.
- **Spring Data JPA**: Implementação de JPA para interação com o banco de dados.
- **H2 Database**: Banco de dados em memória, utilizado para armazenar os dados.
- **Jackson**: Biblioteca para conversão entre objetos Java e JSON.
- **Postman**: Utilizado para testar os endpoints da API.

## Pré-requisitos

- **Java 17 ou superior**.
- **Maven** para gerenciamento de dependências e build da aplicação.

## Como Rodar o Projeto

### 1. Clonando o repositório

Para começar a trabalhar com este projeto, primeiro clone o repositório para sua máquina local. Abra seu terminal e execute o seguinte comando:

```bash
git clone https://github.com/SEU_USUARIO/crud-clientes.git
```
## 2. Configurando o Projeto

Após clonar o repositório, navegue até a pasta do projeto:

```bash
cd crud-clientes
```

## 3. Build do Projeto

Certifique-se de que o Maven está instalado em sua máquina. Caso não tenha o Maven, você pode instalar seguindo as instruções do Maven.

Com o Maven instalado, execute o comando para baixar as dependências e compilar o projeto:

```bash
mvn clean install
```

## 4. Testando os Endpoints

Agora, você pode testar os endpoints utilizando uma ferramenta como Postman.

### Endpoints disponíveis:
#### POST /clients - Cadastrar um novo cliente.

```json
{
  "name": "João Silva",
  "cpf": "12345678901",
  "income": 2500.50,
  "birthDate": "1990-05-10",
  "children": 2
}
```

#### GET /clients - Listar todos os clientes (paginado).

Parâmetros de paginação:

- page (número da página, padrão: 0)
- size (quantidade de itens por página, padrão: 10)
  
#### GET /clients/{id} - Consultar um cliente específico pelo ID.
#### PUT /clients/{id} - Atualizar um cliente.

```json
{
  "name": "João Silva",
  "cpf": "12345678901",
  "income": 3000.00,
  "birthDate": "1990-05-10",
  "children": 3
}
```
#### DELETE /clients/{id} - Deletar um cliente pelo ID.

