# Roadmap de Estudos de Banco de Dados para Desenvolvedores

Este guia foi criado para desenvolvedores de software iniciantes que desejam se tornar proficientes no uso e na compreensão de bancos de dados.

Objetivos: Desenvolver habilidades de criar, modelar e consultar banco de dados.

Marque os itens conforme avança nos estudos!

---

## Módulo 1: Fundamentos Essenciais

*O objetivo aqui é construir uma base sólida, independentemente da tecnologia que você usará no futuro.*

- [ ] **O que é um Banco de Dados?**
  - [ ] Entender o propósito: armazenar, organizar e recuperar dados de forma eficiente.
  - [ ] Diferença entre um banco de dados e uma planilha (Excel, Google Sheets).
  - [ ] Importância para aplicações de software.
- [ ] **Tipos de Bancos de Dados: A Grande Divisão**
  - [ ] **Relacionais (SQL):** Estrutura rígida com tabelas, linhas e colunas (Ex: PostgreSQL, MySQL, SQL Server).
  - [ ] **Não Relacionais (NoSQL):** Estruturas flexíveis (Ex: MongoDB, Redis, Cassandra).
  - [ ] Quando usar um ou outro? Uma visão geral.

---

## Módulo 2: O Mundo Relacional (SQL)

*Este é o tipo de banco de dados mais comum e um conhecimento obrigatório para qualquer dev.*

- [ ] **Conceitos-Chave do Modelo Relacional**
  - [ ] Tabelas, Colunas (Atributos) e Linhas (Registros).
  - [ ] Tipos de Dados (`INTEGER`, `VARCHAR`, `TEXT`, `DATE`, `BOOLEAN`, etc.).
  - [ ] **Chaves (Keys):**
    - [ ] `Primary Key` (Chave Primária): O identificador único de cada linha.
    - [ ] `Foreign Key` (Chave Estrangeira): Como as tabelas se relacionam.
  - [ ] Constraints (Restrições): `NOT NULL`, `UNIQUE`, `CHECK`.
- [ ] **SQL Básico: A Linguagem para "Conversar" com o Banco**
  - [ ] **CRUD (Create, Read, Update, Delete):**
    - [ ] `SELECT`: Para ler/consultar dados (`FROM`, `WHERE`, `ORDER BY`, `LIMIT`).
    - [ ] `INSERT INTO`: Para criar novos registros.
    - [ ] `UPDATE`: Para modificar registros existentes.
    - [ ] `DELETE`: Para remover registros.
- [ ] **Relacionamentos e Junções (JOINs)**
  - [ ] Entender os tipos de relacionamento: Um-para-Um (1:1), Um-para-Muitos (1:N) e Muitos-para-Muitos (N:M).
  - [ ] Como combinar dados de múltiplas tabelas: `INNER JOIN`, `LEFT JOIN`.
- [ ] **Agrupamento e Funções de Agregação**
  - [ ] `GROUP BY`: Para agrupar linhas que têm os mesmos valores.
  - [ ] Funções: `COUNT()`, `SUM()`, `AVG()`, `MAX()`, `MIN()`.
  - [ ] `HAVING`: Para filtrar resultados depois do agrupamento.
- [ ] **Modelagem de Dados**
  - [ ] Como desenhar um esquema de banco de dados para uma aplicação (Diagrama Entidade-Relacionamento).
  - [ ] **Normalização:** O que é e por que é importante (entender as 3 primeiras formas normais).
- [ ] **Tópicos Intermediários de SQL**
  - [ ] Subqueries (Subconsultas): Uma `SELECT` dentro de outra.
  - [ ] `Transactions` (Transações): Garantindo a integridade dos dados com `COMMIT` e `ROLLBACK`.
  - [ ] `Indexes` (Índices): Como acelerar drasticamente suas consultas.

---

## Módulo 3: O Universo Não Relacional (NoSQL)

*Ideal para aplicações que precisam de alta escalabilidade e flexibilidade.*

- [ ] **Por que NoSQL?**
  - [ ] Flexibilidade de esquema.
  - [ ] Escalabilidade horizontal.
  - [ ] Big Data e aplicações em tempo real.
- [ ] **Principais Tipos de Bancos NoSQL**
  - [ ] **Documento (Ex: MongoDB):** Armazena dados em formato similar a JSON.
  - [ ] **Chave-Valor (Ex: Redis):** Estrutura de dados super simples e rápida, ideal para cache.
  - [ ] **Grafos (Ex: Neo4j):** Focado em relacionamentos complexos (redes sociais, recomendações).

---

## Módulo 4: Conectando o Banco de Dados à sua Aplicação

*Onde a teoria encontra a prática do dia a dia do desenvolvedor.*

- [ ] **Drivers de Banco de Dados vs. ORMs/ODMs**
  - [ ] **Drivers:** Bibliotecas para executar queries diretamente.
  - [ ] **ORM (Object-Relational Mapper):** Ferramentas que mapeiam tabelas para objetos no seu código (Ex: Sequelize, TypeORM, Hibernate).
- [ ] **Migrations (Migrações de Banco de Dados)**
  - [ ] O que são e por que são essenciais para trabalho em equipe.
- [ ] **Connection Pooling**
  - [ ] O que é e por que melhora a performance da sua aplicação.

---

## Módulo 5: Tópicos Avançados e Boas Práticas

- [ ] **Performance e Otimização:** Como usar `EXPLAIN` para analisar uma query.
- [ ] **Segurança:** Prevenção de **SQL Injection**.
- [ ] **Conceitos de Arquitetura:** Replicação e Sharding.
