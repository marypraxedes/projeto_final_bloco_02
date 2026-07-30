# 💊 Farmácia API

API REST desenvolvida para um sistema de comércio eletrônico de uma farmácia, permitindo o gerenciamento de categorias e produtos, com relacionamento entre entidades, persistência em banco de dados e autenticação de usuários utilizando Spring Security e JWT.

O projeto foi desenvolvido durante o **Bootcamp Java Full Stack da Generation Brasil**, aplicando conceitos de desenvolvimento backend com Java e Spring Boot.

---

## 🚀 Tecnologias utilizadas

* Java
* Spring Boot
* Spring Data JPA
* Hibernate
* Spring Security
* JWT (JSON Web Token)
* MySQL
* Maven
* Jakarta Validation
* Git e GitHub
* Insomnia para testes da API

---

## 📌 Funcionalidades

### 🔹 Categoria

CRUD completo de categorias:

* Listar todas as categorias
* Buscar categoria por ID
* Buscar categorias por tipo
* Cadastrar categoria
* Atualizar categoria
* Remover categoria

---

### 🔹 Produto

CRUD completo de produtos:

* Listar todos os produtos
* Buscar produto por ID
* Buscar produtos por nome
* Cadastrar produto
* Atualizar produto
* Remover produto

---

### 🔹 Relacionamento

O sistema possui relacionamento entre:

**Categoria (1) → (N) Produtos**

Uma categoria pode possuir vários produtos, enquanto cada produto pertence a uma categoria.

---

## 🔐 Autenticação e Segurança

Implementação de autenticação utilizando:

* Spring Security
* JWT
* BCrypt para criptografia de senhas

Funcionalidades:

* Cadastro de usuários
* Login com geração de token JWT
* Proteção dos endpoints da API
* Controle de acesso através de autenticação por token

---

## 🗂️ Estrutura do projeto

```
src/main/java/com/generation/farmacia

├── controller
│   ├── CategoriaController
│   ├── ProdutoController
│   └── UsuarioController
│
├── model
│   ├── Categoria
│   ├── Produto
│   ├── Usuario
│   └── UsuarioLogin
│
├── repository
│   ├── CategoriaRepository
│   ├── ProdutoRepository
│   └── UsuarioRepository
│
├── service
│   └── UsuarioService
│
└── security
    ├── SecurityConfig
    ├── JwtService
    ├── JwtAuthFilter
    ├── UserDetailsImpl
    └── UserDetailsServiceImpl
```

---

## 🛢️ Banco de dados

Banco utilizado:

```
MySQL
```

Principais tabelas:

* `tb_categorias`
* `tb_produtos`
* `tb_usuarios`

---

## 🧪 Testes

A API foi testada utilizando o Insomnia, validando:

✅ Cadastro e autenticação de usuários
✅ Geração e validação de token JWT
✅ Operações CRUD de categorias
✅ Operações CRUD de produtos
✅ Relacionamento entre produtos e categorias

---

## 📍 Endpoints principais

### Usuários

```
POST /usuarios/cadastrar
POST /usuarios/logar
```

### Categorias

```
GET    /categorias
GET    /categorias/{id}
GET    /categorias/tipo/{tipo}
POST   /categorias
PUT    /categorias
DELETE /categorias/{id}
```

### Produtos

```
GET    /produtos
GET    /produtos/{id}
GET    /produtos/nome/{nome}
POST   /produtos
PUT    /produtos
DELETE /produtos/{id}
```

---

## 👩‍💻 Desenvolvido por

**Maryane Praxedes**

Estudante de Engenharia de Software | Desenvolvedora Java Backend

🔗 GitHub: https://github.com/marypraxedes

🔗 LinkedIn: https://www.linkedin.com/marypraxedes
