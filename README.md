# Sistema de Gerenciamento de Biblioteca

Este projeto implementa um sistema simples de gerenciamento de uma biblioteca utilizando SQLite. O sistema permite registrar autores, livros e empréstimos, fornecendo uma base para um sistema mais complexo.

## Funcionalidades

- Cadastro de autores com nome e nacionalidade.
- Cadastro de livros com título, autor, ano de publicação e gênero.
- Registro de empréstimos de livros, incluindo data de empréstimo e devolução.

## Estrutura do Banco de Dados

O banco de dados contém três tabelas principais:

1. **Autores**
   - `AutorID`: Identificador único do autor.
   - `Nome`: Nome do autor.
   - `Nacionalidade`: Nacionalidade do autor.

2. **Livros**
   - `LivroID`: Identificador único do livro.
   - `Titulo`: Título do livro.
   - `AutorID`: Referência ao autor do livro.
   - `AnoPublicacao`: Ano de publicação do livro.
   - `Genero`: Gênero do livro.

3. **Emprestimos**
   - `EmprestimoID`: Identificador único do empréstimo.
   - `LivroID`: Referência ao livro emprestado.
   - `DataEmprestimo`: Data do empréstimo.
   - `DataDevolucao`: Data da devolução (pode ser nula).
   - `NomeUsuario`: Nome do usuário que fez o empréstimo.

## Como Usar

1. Certifique-se de ter Python e SQLite instalados em sua máquina.
2. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/sistema-biblioteca.git
