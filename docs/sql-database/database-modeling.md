# Modelagem de Banco de Dados

## MER (Modelo Entidade Relacionamento)

É um modelo conceitual para representar a estrutura geral do banco de dados.
Descreve as entidades, attributos das entidades e as relações entre as entidades.
É representado através de diagramas DER.

Não leva em consideração os detalhes de implementação, pois isso pode variar de acordo com o SGBD usado.

## DER (Diagrama Entidade Relacionamento)

É a representação gráfica do MER.

## Componentes

### Entidades

São nomeadas com substantivos concretos ou abstratos que representem de forma clara sua função dentro do domínio.
São representações das tabelas.
Ex: Users, Products, Orders, etc.
No diagrama é representada por um retângulo.

### Atributos

São as caracteristicas ou propriedades das entidades. Eles descrevem informações especificas sobre uma entidade.
No diagrama são representados por elipses ou uma notação UML (Retangulo com nome da entidade no topo e uma lista abaixo contendo os atributos).

### Relacionamentos

Representam as associações entre as entidades.
No diagrama são representados por losangos.
Nomeie os relacionamentos com significados de forma a deixar claro o que a relação faz.

#### Cardinalidades

- 0:1
  - Cardinalidade opcional.
- 1:1
- 1:N
- N:N
  - geralmente se utiliza uma terceira tabela para armazenar este tipo de relação.

## Databases

- **Tabelas**: É usada para armazenar dados de forma organizada. Cada tabela em um banco de dados relacional tem um nome único e é dividida em colunas e linhas.
- **Colunas**: É uma estrutura dentro de uma tabela que representa um att especifico dos dados armazenados. Cada coluna tem um nome unico e um tipo de dados associado que define o tipo de informações que pode ser armazenado nela, como numeros, textos, datas, etc.
- **Registros**: Também conhecido como linha ou tupla, é uma instância individual de dados em uma tabela.
- **Tipos de Dados**: Podem variar entre os diversos SGBD, os mais comuns são:
  - integer
  - decimal/numeric
  - character/varchar
  - date/time
  - boolean
  - text (texto longo)
- **Restrição de valor**:
  - Not null
  - Unique
  - Default
- **Chaves Primárias**
- **Chaves Estrangeiras**
- **Auto Incremento**

## Operações CRUD

## Chaves Primárias

- Identifica exclusivamente
- Não pode conter valores nulos
- Uma tabela pode ter apenas uma PK

## Chaves Estrangeiras

É usada para estabelecer e manter a integridade dos dados entre tabelas relacionadas.

- Pode ser nula (registro órfão)
- É possível ter mais de uma (ou nenhuma) em uma tabela.

## Restrições

- **ON DELETE**: Especifica o que acontece com os registros dependentes quando um registro pai é excluido.
- **ON UPDATE**: Define o comportamento dos registros dependentes quando um registro pai é atualizado.
- CASCADE, SET NULL, SET DEFAULT E RESTRICT.

## Tools

- [https://app.creately.com](https://app.creately.com)
- [https://app.quickdatabasediagrams.com](https://app.quickdatabasediagrams.com): Permite criar diagramas de forma descritiva.
- [https://clients.cloudclusters.io](https://clients.cloudclusters.io)