# 📚 Sistema de Estoque para Sebo

A ideia surgiu justamente para tornar esse processo mais organizado e eficiente. Como ex-funcionário, sei o quanto um sistema simples, visual e funcional pode ajudar nas tarefas cotidianas como localizar um livro, dar baixa após a venda e organizar os espaços físicos do sebo.

Este projeto também tem como objetivo mostrar como soluções reais podem ser construídas com base em experiências práticas de trabalho, servindo como exemplo para quem está começando a aprender ou desenvolvendo sistemas similares.


## 🚀 Funcionalidades

- Cadastro de livros com título, autor, ano, gênero e preço
- Registro e controle de vendedores
- Organização do estoque por fileiras físicas (ex: Fileira A, Fileira B)
- Alocação de livros por fileira e vendedor
- Visualização e atualização do estoque
- Remoção de livros do estoque (baixa após venda)

## 🧱 Modelagem do Banco de Dados

O sistema usa um modelo relacional com as seguintes entidades:

- **Livro**
  - `id`, `titulo`, `autor`, `ano`, `genero`, `preco`

- **Vendedor**
  - `id`, `nome`

- **Fileira**
  - `id`, `nome`, `capacidade`

- **Estoque**
  - `id`, `livro_id`, `vendedor_id`, `fileira_id`, `quantidade`

### 🔗 Relacionamentos

- Um **livro** pode estar em vários registros de **estoque**
- Um **vendedor** pode ser responsável por vários registros de **estoque**
- Cada **fileira** pode conter vários livros
- Cada **registro de estoque** conecta um livro a uma fileira e a um vendedor, com a quantidade

## 🛠️ Tecnologias Utilizadas

- Linguagem: `Python` / `JavaScript` (dependendo da versão)
- Banco de Dados: `SQLite`
- Interface: HTML/CSS ou React/Flutter (dependendo da implementação)
- Ferramenta de modelagem: [dbdiagram.io](https://dbdiagram.io) ou brModelo


