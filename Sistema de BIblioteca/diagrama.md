# 📌 Diagrama de Casos de Uso

## Atores
- Aluno
- Professor
- Bibliotecário

## Casos de Uso
- Buscar Livro
- Realizar Empréstimo
- Reservar Livro
- Consultar Histórico
- Cadastrar Livro
- Gerenciar Usuários
- Registrar Devolução
- Aplicar Multa

---

# 📌 Diagrama de Classes

## Classe Usuario (abstrata)
- id: int
- nome: string
- email: string
+ autenticar()
+ buscarLivro()

## Classe Aluno herda Usuario
- matricula: string
+ reservar()
+ emprestar()

## Classe Professor herda Usuario
- departamento: string
+ reservar()
+ emprestar()

## Classe Bibliotecario herda Usuario
- registro: string
+ cadastrarLivro()

## Classe Livro
- titulo: string
- autor: string
- disponivel: boolean
+ verificarDisponibilidade()

## Classe Emprestimo
- dataEmprestimo: date
- dataDevolucao: date
+ calcularMulta()

## Classe Multa
- valor: double
- paga: boolean
+ registrarPagamento()