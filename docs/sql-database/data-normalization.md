# Normalização de Dados

É um processo no qual se organiza e estrutura um banco de dados relacional de forma a eliminar redundâncias e anomalias, garantindo a consistência e integridade dos dados.

## Formas Normais

### 1FN: Atomicidade de dados

Estabelece que cada valor em uma tabela deve ser atômico, ou seja, indivisível.
Nenhum campo deve conter múltiplos valores ou listas.
Ex: O campo **endereço** contendo múltiplos valores, como rua, número, cidade, bairro e estado.
Para atingir a 1FN, precisamos dividir o campo "endereço" em colunas separadas.

### 2FN

Estabele que uma tabela deve estar na 1FN.
Todos os atts não chave devem depender totalmente da chave primária.

> **OBS**: Se a tabela tem uma PK simples, então não existe a possibilidade de termos dependência parcial e por tanto ela já se encontra na 2FN.

### 3FN

Uma tabela deve estar na 2FN.
Nenhuma coluna não-chave deve depender de outra coluna não-chave.

## Resumo

- **1FN**: Garante que cada valor seja atômico e que os registros sejam únicos e identificáveis.
- **2FN**: Garante que os atts não-chave dependam totalmente da PK, evitando dependencias parciais.
- **3FN**: Elimina dependencias transitivas entre os atts não-chave, garantindo que cada att não-chave dependa apenas da PK, não havendo dependencias indiretas entre eles.