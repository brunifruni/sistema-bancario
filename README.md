# 💸 Sistema Bancário em Python

Este projeto é um sistema bancário de terminal desenvolvido em Python com foco em princípios de orientação a objetos (POO), boas práticas de arquitetura e uso de herança, polimorfismo e abstração. Idealizado como parte dos meus estudos práticos em desenvolvimento backend e estruturas de software.

## 🚀 Funcionalidades

- 📥 Depósitos  
- 💸 Saques com controle de limite e quantidade por conta  
- 📄 Geração de extrato  
- 👤 Cadastro de clientes (Pessoa Física)  
- 🏦 Criação de contas correntes  
- 🧾 Histórico de transações com data/hora  
- 📋 Listagem de contas com iterator customizado  

## 🧠 Conceitos aplicados

- Programação Orientada a Objetos (POO)  
  - Herança (`PessoaFisica` herdando de `Cliente`)  
  - Abstração com `Transacao` (classe abstrata)  
  - Polimorfismo (sobrescrita do método `sacar`)  
- Iterator personalizado (`contasIterador`)  
- Decoradores para log de transações (`@log_transacao`)  
- Boas práticas de encapsulamento e separação de responsabilidades  

## 🏗️ Estrutura principal

Cliente -> PessoaFisica
Conta -> ContaCorrente
Transacao -> Saque / Deposito
Historico -> registra e filtra transações


## 🖥️ Como utilizar

1. Clone o repositório:  
   ```bash
   git clone https://github.com/seu-usuario/sistema-bancario-python.git
   cd sistema-bancario-python
   
2. Execute o sistema:
  ```bash
  python nome_do_arquivo.py

3. Use o menu interativo no terminal:
  ```csharp
================ MENU ================
[d] Depositar
[s] Sacar
[e] Extrato
[nc] Nova conta
[lc] Listar contas
[nu] Novo usuário
[q] Sair

### 📌 Requisitos
Python 3.10+

Apenas bibliotecas padrão do Python (sem dependências externas)

### 🎯 Possíveis melhorias futuras
Persistência de dados (ex: JSON, SQLite)

Interface gráfica (Tkinter, PyQt)

Validação avançada de CPF e datas

Modularização do código para escalabilidade

Implementação de testes automatizados

### 🤝 Contribuições
Contribuições são muito bem-vindas! Abra uma issue ou envie um pull request com melhorias e sugestões.

### 🧑‍💻 Sobre mim
Sou Bruna, estudante de Análise e Desenvolvimento de Sistemas com foco em Cibersegurança, apaixonada por tecnologia, código limpo e soluções práticas.
