# 💊 Farmácia API

API REST desenvolvida durante o **Bootcamp Java Full Stack da Generation Brasil**.
O projeto consiste em um sistema de **Comércio Eletrônico de uma Farmácia**, permitindo o gerenciamento de categorias e produtos através de operações CRUD.

A aplicação foi construída utilizando **Java e Spring Boot**, aplicando conceitos de arquitetura REST, persistência de dados com JPA/Hibernate e relacionamento entre entidades.

---

## 🚀 Tecnologias utilizadas

* Java
* Spring Boot
* Spring Web
* Spring Data JPA
* Hibernate
* MySQL
* Maven
* Jakarta Validation
* Git e GitHub
* Insomnia

---

## 📌 Funcionalidades

### Categorias

* Cadastrar categoria
* Listar todas as categorias
* Buscar categoria por ID
* Buscar categorias pelo tipo
* Atualizar categoria
* Remover categoria

### Produtos

* Cadastrar produto
* Listar todos os produtos
* Buscar produto por ID
* Buscar produtos pelo nome
* Atualizar produto
* Remover produto

---

## 🔗 Relacionamento entre entidades

O projeto possui um relacionamento **Um para Muitos (1:N)** entre Categoria e Produto.

```
Categoria
    |
    | 1
    |
    | N
Produto
```

Uma categoria pode possuir vários produtos, enquanto cada produto pertence a uma única categoria.

---

## 🗂️ Modelo de dados

### Categoria

| Campo | Tipo   |
| ----- | ------ |
| id    | Long   |
| tipo  | String |

### Produto

| Campo     | Tipo       |
| --------- | ---------- |
| id        | Long       |
| nome      | String     |
| preco     | BigDecimal |
| estoque   | Integer    |
| foto      | String     |
| categoria | Categoria  |

---

## 📁 Estrutura do projeto

```
src/main/java/com/generation/farmacia

├── controller
│   ├── CategoriaController.java
│   └── ProdutoController.java
│
├── model
│   ├── Categoria.java
│   └── Produto.java
│
├── repository
│   ├── CategoriaRepository.java
│   └── ProdutoRepository.java
│
└── FarmaciaApplication.java
```

---

## ⚙️ Configuração do banco de dados

Banco utilizado:

```
db_farmacia
```

Configuração no arquivo `application.properties`:

```
spring.datasource.url=jdbc:mysql://localhost/db_farmacia
spring.datasource.username=root
spring.datasource.password=root
```

---

## 🧪 Testes da API

Os testes dos endpoints foram realizados utilizando o Insomnia.

Principais rotas:

### Categoria

```
GET     /categorias
GET     /categorias/{id}
GET     /categorias/tipo/{tipo}
POST    /categorias
PUT     /categorias
DELETE  /categorias/{id}
```

### Produto

```
GET     /produtos
GET     /produtos/{id}
GET     /produtos/nome/{nome}
POST    /produtos
PUT     /produtos
DELETE  /produtos/{id}
```

---

## 👩‍💻 Desenvolvimento

Projeto desenvolvido individualmente como parte do **Performance Goal Check - Bloco 02** do Bootcamp Java Full Stack da Generation Brasil.

---

## Autora

**Maryane Praxedes**

GitHub: https://github.com/marypraxedes
