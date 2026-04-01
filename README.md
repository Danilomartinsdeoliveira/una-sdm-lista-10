# 🎬 OscarFilmeApi

API desenvolvida em ASP.NET Core para gerenciamento de filmes indicados ao Oscar.

---

## 🚀 Tecnologias Utilizadas

* .NET 10
* ASP.NET Core Web API
* Entity Framework Core (InMemory)
* Swagger (Swashbuckle)

---

## 📦 Funcionalidades

A API permite:

* ✅ Cadastrar filmes indicados ao Oscar
* ✅ Listar todos os filmes
* ✅ Filtrar apenas os vencedores
* ✅ Atualizar dados de um filme
* ✅ Remover filmes
* ✅ Exibir estatísticas

---

## 📁 Estrutura do Projeto

* **Models** → Classe `Filme`
* **Data** → `AppDbContext`
* **Controllers** → `FilmesController`

---

## ▶️ Como Executar

No terminal:

```bash
dotnet run
```

Acesse no navegador:

```
http://localhost:5295/swagger
```

---

## 🧪 Rotas da API

### 🔹 POST /api/filmes

Cadastra um novo filme

📌 Regra:

* O ano de lançamento não pode ser menor que 1929

---

### 🔹 GET /api/filmes

Lista todos os filmes

---

### 🔹 GET /api/filmes/vencedores

Retorna apenas filmes vencedores

---

### 🔹 PUT /api/filmes/{id}

Atualiza um filme

📌 Regra:

* Ao marcar `Venceu = true`, o sistema exibe no console:

```
Temos um novo vencedor: [Nome do Filme]!
```

---

### 🔹 DELETE /api/filmes/{id}

Remove um filme pelo ID

---

### 🔹 GET /api/filmes/estatisticas

Retorna:

* Total de filmes cadastrados
* Total de filmes vencedores

---

## ⚠️ Observação Importante

A aplicação utiliza banco de dados **InMemory**.

👉 Isso significa que:

> Todos os dados são perdidos ao reiniciar a aplicação.

---

## 📸 Evidências (prints)

Foram realizados testes das seguintes rotas:

* POST
* GET
* GET (vencedores)
* PUT
* DELETE

*(Inserir prints aqui)*

---

## 👨‍🏫 Disciplina

Sistemas Distribuídos e Mobile
Centro Universitário UNA

---

## 👨‍💻 Autor

Danilo Martins de Oliveira

---
