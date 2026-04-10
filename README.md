# 📚 Sistema de Biblioteca

Projeto acadêmico que representa a modelagem de um sistema de biblioteca utilizando diagramas UML, incluindo casos de uso e diagrama de classes.

---

## 🎯 Objetivo

Desenvolver a estrutura de um sistema capaz de gerenciar operações de uma biblioteca, como empréstimos, reservas e controle de usuários.

---

## 👥 Atores do Sistema

* Aluno
* Professor
* Bibliotecário

---

## ⚙️ Funcionalidades

O sistema permite:

* 🔍 Buscar livros
* 📖 Realizar empréstimos
* 📌 Reservar livros
* 🕒 Consultar histórico
* ➕ Cadastrar livros
* 👤 Gerenciar usuários
* 🔄 Registrar devoluções
* 💰 Aplicar multas

---

## 🧠 Estrutura do Sistema (Classes)

### 👤 Usuário (classe abstrata)

* id
* nome
* email
* Métodos:

  * autenticar()
  * buscarLivro()

### 🎓 Aluno

* matrícula
* Métodos:

  * reservar()
  * emprestar()

### 👨‍🏫 Professor

* departamento
* Métodos:

  * reservar()
  * emprestar()

### 📚 Bibliotecário

* registro
* Método:

  * cadastrarLivro()

### 📖 Livro

* título
* autor
* disponível
* Método:

  * verificarDisponibilidade()

### 🔄 Empréstimo

* dataEmprestimo
* dataDevolucao
* Método:

  * calcularMulta()

### 💰 Multa

* valor
* paga
* Método:

  * registrarPagamento()

---

## 🖼️ Diagrama UML

![Diagrama](diagrama.png)

---

## 🛠️ Tecnologias Utilizadas

* UML (Modelagem)
* Markdown
* GitHub

---

## 📂 Estrutura do Projeto

* `diagrama.md` → descrição dos diagramas
* `diagrama.png` → imagem do diagrama UML
* `diagrama.uml` → arquivo de modelagem

---

## 👨‍💻 Autor

* Luan Candido

---

## 📌 Observações

Este projeto tem fins acadêmicos e representa apenas a modelagem do sistema, não sua implementação em código.

