# Banco de Dados
#### O que é um banco de Dados Relacional? 
  - Um banco de dados Relacional é um tipo de banco de dados que organiza os dados em tabelas, essas tabelas são compostas por linhas e colunas.
    Cada linha representa um registro único, e cada coluna representa um atributo ou uma categoria de dados. As tabelas podem ser ligadas entre si por meio de relações que são estabelecidas através de chaves, uma chave primária identifica de forma única cada registro em uma tabela, e uma chave estrangeira em outra tabela aponta para essa chave primária, criando um vínculo entre os dados.
      - Um **exemplo** é o *Sistema Bancário*

#### O que é um banco de Dados Não Relacional?
- Um banco de Dados Não Relacional é um tipo de banco que não utiliza a estrutura tradicional de tabelas, colunas e linhas diferente dos bancos de dados relacionais ele não se baseia em relações entre tabelas, em vez disso, ele armazena os dados de forma mais flexível, dependendo do modelo que é usado isso o torna ideal para lidar com grandes volumes de dados não estruturados ou semi-estruturados, como redes sociais.
  - **Exemplo** é o uma *plataforma de rede social como o Facebook*   
#### O que é normalização e seu objetivo?
  - A normalização é um processo fundamental no design de bancos de dados relacionais. Em resumo, é um conjunto de regras e técnicas que serve para organizar os dados da maneira mais eficiente possível processo consiste em dividir uma tabela grande e complexa em tabelas menores e mais simples, conectando-as através de chaves. O objetivo principal é garantir que cada informação esteja armazenada em um único lugar, eliminando a redundância e garantindo a consistência dos dados.

## Tabela Não Normalizada
#### Séries

| Nome da Série      |    Gênero      | Temporadas  |  Plataforma   |
|--------------------|---------------------|-------------|---------------|
| Brilhante Victoria |Infantil/Comédia     |      4      | Netflix       |
| Rick and Morty     |Animção/Comédia      |      8      | Amazon Prime  |
| Mentirosos         |Ficção/Suspense      |      1      | Prime Video   |
| Ginny e Georgia    |Drama/Romace/suspense|      3      | Netflix       |
| Lost Girl          |Drama/Fantasia       |      5      | Amazon Video  |
| O Exorcista        |Terror/Suspense      |      2      | Prime Video   |
| Eu Nunca...        |Drama/Romance/Comédia|      4      | Netflix       |

## Normalização até a 3º Formal Normal
### 1º Forma Normal
| Nome da Série      |      Gênero         | Temporadas  |  Plataforma   |
|--------------------|---------------------|-------------|---------------|
| Brilhante Victoria | Infantil            |      4      | Netflix       |
| Brilhante Victoria | Comédia             |      4      | Netflix       |
| Rick and Morty     | Animação            |      8      | Amazon Prime  |
| Rick and Morty     | Comédia             |      8      | Amazon Prime  |
| Mentirosos         | Ficção              |      1      | Prime Video   |
| Mentirosos         | Suspense            |      1      | Prime Video   |
| Ginny e Georgia    | Drama               |      3      | Netflix       |
| Ginny e Georgia    | Romance             |      3      | Netflix       |
| Ginny e Georgia    | Suspense            |      3      | Netflix       |
| O Exorcista        | Terror              |      2      | Prime Video   |
| O Exorcista        | Suspense            |      2      | Prime Video   |
| Eu Nunca...        | Drama               |      4      | Netflix       |
| Eu Nunca...        | Romance             |      4      | Netflix       |
| Eu Nunca...        | Comédia             |      4      | Netflix       |
### 2º Forma Normal
