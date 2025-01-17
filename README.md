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
