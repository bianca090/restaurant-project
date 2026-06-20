# 🍽️ Sabor Express

O **Sabor Express** é uma aplicação de linha de comando (CLI) desenvolvida em Python para gerenciar cadastros e estados de restaurantes. Este projeto foi desenvolvido com foco prático como parte dos meus estudos de Python na plataforma **Alura**.

O principal objetivo foi consolidar conceitos fundamentais da linguagem, como manipulação de dicionários e listas, estruturas condicionais, tratamento de exceções, laços de repetição e modularização por meio de funções.

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

---

## 🚀 Funcionalidades

O sistema oferece um menu interativo com as seguintes opções:
1. **Cadastrar restaurante:** Permite adicionar um novo restaurante informando o nome e a categoria (por padrão, inicia como desativado).
2. **Listar restaurantes:** Exibe de forma tabular e alinhada o nome, a categoria e o status de ativação de todos os restaurantes cadastrados.
3. **Alternar estado do restaurante:** Permite ativar ou desativar um restaurante existente buscando pelo seu nome.
4. **Sair:** Encerra a execução do programa com segurança.

---

## 🛠️ Tecnologias e Conceitos Aplicados

- **Python 3**
- **Manipulação de Coleções:** Uso prático de listas e dicionários (`list[dict]`) para simular um banco de dados em memória.
- **Formatação de Strings:** Uso do método `.ljust()` para garantir um alinhamento visual organizado na listagem do terminal, além de *f-strings*.
- **Estruturas de Controle e Loops:** Condicionais (`if/elif/else`) e laços (`for`) para percorrer e validar dados.
- **Tratamento de Erros:** Bloco `try/except` para capturar entradas inválidas do usuário e evitar que a aplicação quebre de forma inesperada.
- **Interação com o Sistema Operacional:** Uso da biblioteca nativa `os` para limpar o console (`os.system('cls')`) melhorando a experiência visual (UX) no terminal.

---

## 📁 Estrutura do Código

O projeto é centralizado no arquivo `app.py`, estruturado com as seguintes funções principais:
- `exibir_nome_do_programa()` / `exibir_subtitulo()`: Gerenciamento visual do menu.
- `cadastrar_novo_restaurante()`: Captura dados e faz o `.append()` na lista.
- `listar_restaurants()`: Varre a lista aplicando lógicas condicionais para exibição do status.
- `alternar_estado_restaurante()`: Altera o estado booleano do campo `ativo` via inversão lógica (`not`).
- `escolher_opcao()`: Controla o fluxo principal através do input do menu.
