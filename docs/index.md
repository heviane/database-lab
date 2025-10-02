# Introduction

## O que é Banco de Dados?

É uma coleção organizada de informações (ou dados) estruturados, normalmente eletronicamente armazenadas em um sistema de computador.

## O que é um DBMS (Database Management System) ou SGBD (Software Gerenciador de Banco de Dados)?

Sistema de Gerenciamento de Banco de Dados.
É um software utilizado para acessar, manipular e monitorar um sistema de banco de dados de forma visual.
Oferece um conjunto de recursos e ferramentas.
Cada banco de dados tem os seus.

**Funcionalidades Básicas**:

- CRUD

## Tipos de Banco de Dados

### Bancos de Dados Relacionais (SQL)

Armazena dados estruturados, sendo organizado em tabelas, com colunas e linhas, que se relacionam entre si.
É o mais usado atualmente.

#### Caracteristicas

- Estrutura de Tabelas com Linhas/Tuplas/Registros (dados em si) e Colunas/Campos (definições).
- Relacionamento entre tabelas (Chaves Primárias e Estrangeiras)
- SQL (Structured Query Language)
- Integridade Referencial
- Normalização de dados
- Flexibilidade e Extensibilidade
- Segurança (Autenticacao, Autorização, Controle de Acesso, logs, backups)
- Transações ACID (Atomicity, Consistency, Isolation, Durability): Garante a consistencia e integridade dos dados.
  - Atomicity
  - Consistency
  - Isolation: Garante que uma escrita será realizada após a outra, ou seja, não permiti operações concorrentes.
  - Durability

### Bancos de Dados Não Relacionais (NoSQL - Not Only SQL)

Banco de dados onde os dados não são armazenados de forma estruturada (tabela), e sim de forma não estruturada ou semi-estruturadas.

**Estruturado** sempre possui uma estrutura e regras rigidas.
**Semi-estruturado** possui alguma estrutura, algumas regras, mas não é rigido.
Exemplo: JSON vs Tabela.

**Tipos:**

- Document
- Key-value
- Wide-column stores
- Graph

### Outros tipos de Bancos de Dados

- Orientado a Objetos
- Hierárquico

### Quando usar um ou outro? Uma visão geral

- Geralmente, NoSQL é mais rápido que SQL.
