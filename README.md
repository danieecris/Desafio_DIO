# Desafio DIO — Sistema Bancário em Python

Projeto desenvolvido como desafio da plataforma [DIO (Digital Innovation One)](https://www.dio.me/), implementando um sistema bancário simples utilizando **Programação Orientada a Objetos (POO)** em Python.

## Funcionalidades

- Cadastro de clientes (Pessoa Física com CPF, nome, data de nascimento e endereço)
- Criação de contas correntes vinculadas a clientes
- Depósito em conta
- Saque com controle de limite por operação e limite diário de saques
- Extrato com histórico de transações
- Listagem de contas cadastradas
- Limite de 2 transações por dia por conta
- Decorator de log para registrar as operações realizadas

## Estrutura do Projeto

```
desafio_Dio/
└── Desafio/
    └── main.py   # Código principal com todas as classes e o menu interativo
```

## Como Executar

Pré-requisito: Python 3.8 ou superior instalado.

```bash
cd Desafio
python main.py
```

## Principais Classes

| Classe | Descrição |
|---|---|
| `Cliente` / `PessoaFisica` | Representa o cliente do banco |
| `Conta` / `ContaCorrente` | Gerencia saldo, saques e depósitos |
| `Historico` | Armazena e filtra o histórico de transações |
| `Transacao` / `Saque` / `Deposito` | Abstração das operações financeiras |
| `ContasIterador` | Iterador customizado para listar contas |

## Conceitos Aplicados

- Classes abstratas (`ABC`, `abstractmethod`)
- Herança e polimorfismo
- Properties (`@property`)
- Decorators (`@log_transacao`)
- Generators (`gerar_relatorio`)
- Iteradores customizados (`__iter__`, `__next__`)
- Métodos de classe (`@classmethod`)
