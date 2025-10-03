# Consultas Avançadas

Consultas com junções e subconsultas.
Funções agregadas e agrupamento de resultados.
Indices.

## JOINS (junções)

São usadas para combinar dados de duas ou mais tebelas relacionadas em um única consulta.

### Tipos

- **INNER JOIN**: Retorna apenas as linhas que tem correspondencia em ambas as tabelas envolvidas na junção. A junção é feita com base em uma condição de igualdade especificada na clausula **ON**. Retorna apenas os dados que forem comuns nas tabelas envolvidas.
- **LEFT JOIN** ou **LEFT OUTER JOIN**: Retorna todas as linhas da tabela à esquerda da junção e as linhas correspondentes da tabela a direita. Se não houver correspondencia, os valores da tabela a direita serão null.
- **RIGHT JOIN** ou **RIGHT OUTER JOIN**: Retorna todas as linhas da tabela à direita da junção e as linhas correspondentes da tabela a esquerda. Se não houver correspondencia, os valores da tabela a esquerda serão null.
- **FULL JOIN** ou **FULL OUTER JOIN**: Retorna todas as linhas de ambas as tabelas envolvidas na junção, combinando-as com base em uma condição de igualdade. Se não houver correspondencia, os valores ausentes serão preenchidos com NULL.

## Subconsultas

Permitem realizar consultas mais complexas permitindo que você use o resultado de uma consulta como entrada para outra consulta.
Consultas aninhadas.

Podem ser usadas em várias partes de uma consulta:

- select
- from
- where
- having
- join

## Funções agregadas

Funções que realizam algum tipo de pré-processamento ou cálculo.

Funções Agregadoras:

- count()
- sum()
- avg()
- min()
- max()

## Agrupamento de Resultados

- select ... from ... group by ...

## Ordenação de Resultados

- select ... from ... order by ...

## Indices de Busca

Análise do Plano de Execução: Ela nos permite examinar as operações realizadas, as tabelas acessadas, os indices utilizados e outras informações importantes para identificar possíveis melhorias de desempenho.

São estruturas de dados que aceleram as pesquisas e as recuperações de funções no banco de dados.
Podem ser criados em uma ou mais colunas.
Permitem o acesso mais rápido.

Estrutura do comando:

```SQL
EXPLAIN
    SELECT *
    FROM {TABELA}
...
```

Análise do Plano de Execução: Quais tipos de campos que pode retornar.

- select_type: simple, subquery, join.
- table
- type: All, index, etc
- possible_keys: Os indices possíveis que podem ser utilizados na operação.
- key: O indice utilizado na operação, se aplicável.
- key_len: O comprimento do indice utilizado.
- ref: As colunas ou constantes usadas para acessar o indice.
- rows
