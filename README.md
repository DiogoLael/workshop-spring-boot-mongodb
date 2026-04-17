# 📌 API de Usuários e Posts com MongoDB

Este projeto é uma API REST desenvolvida com foco na gestão de usuários e seus respectivos posts, utilizando MongoDB como banco de dados. A aplicação segue boas práticas de arquitetura em camadas, uso de DTOs e consultas personalizadas.

---

## 🚀 Tecnologias utilizadas

* Java
* Spring Boot
* Spring Data MongoDB
* MongoDB
* Maven

---

## 📂 Estrutura do projeto

A aplicação foi organizada seguindo o padrão em camadas:

* **Resource (Controller)**: Responsável pelos endpoints da API
* **Service**: Contém as regras de negócio
* **Repository**: Interface de acesso ao banco de dados
* **Domain (Entities)**: Representação das entidades (User, Post)
* **DTOs**: Objetos de transferência de dados

---

## ⚙️ Funcionalidades

### 👤 Usuários

* Inserir usuário
* Atualizar usuário (PUT)
* Deletar usuário
* Buscar todos os usuários
* Buscar usuário por ID

### 📝 Posts

* Criar posts vinculados a usuários
* Buscar post por ID
* Listar posts de um usuário

### 💬 Comentários

* Adicionar comentários aos posts

### 🔍 Consultas

* Consultas simples com Query Methods
* Consultas personalizadas utilizando `@Query`

---

## 🔗 Endpoints principais

### Usuários

* `GET /users` → Lista todos os usuários
* `GET /users/{id}` → Busca usuário por ID
* `POST /users` → Cria um novo usuário
* `PUT /users/{id}` → Atualiza um usuário
* `DELETE /users/{id}` → Remove um usuário

### Posts

* `GET /posts/{id}` → Busca post por ID
* `GET /users/{id}/posts` → Lista posts de um usuário

---

## ▶️ Como executar o projeto

1. Clone o repositório:

```bash
git clone git@github.com:DiogoLael/workshop-spring-boot-mongodb.git
```

2. Acesse a pasta do projeto:

```bash
cd workshop-spring-boot-mongodb
```

3. Configure o MongoDB (local ou remoto)

4. Execute o projeto:

```bash
./mvnw spring-boot:run
```

---

## 🧠 Conceitos aplicados

* Arquitetura em camadas
* Padrão DTO (Data Transfer Object)
* Relacionamento entre documentos (User ↔ Post)
* Banco NoSQL (MongoDB)
* Consultas personalizadas
* Boas práticas em APIs REST

---

## 👨‍💻 Autor

Desenvolvido por **Diogo Lael**
