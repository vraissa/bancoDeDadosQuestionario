# Questionario

## O que é redundância de dados?
É uma duplicidade ou repetição desnecessaria de informações em diferentes partes do banco de dados. Ocorre quando os mesmos dados são armazenados em varias tabelas ou quando uma mesma informação é repetida em várias  linhas da mesma tabela.

## O que é inconsistência de dados?
É quando existem inconsistências nas informações  armazenadas em diferentes partes do banco de dados. Isso pode acontecer devido a problemas como duplicação inadequada de dados, falta de coordenação na atualização dos dados ou falhas no processo de validação e verificação dos dados inseridos.

## Nomeie pelo menos 2 bancos de dados entre Consistência e Tolerância de Particionamento
**_Apache Cassandra_**: Cassandra é um banco de dados distribuído altamente escalável e altamente disponível. Ele foi projetado para oferecer alta tolerância a falhas e é conhecido por sua capacidade de lidar com grandes volumes de dados em vários nós de forma distribuída. No modelo de consistência do Cassandra, é adotada a consistência eventual, o que significa que as atualizações nos dados são propagadas de forma assíncrona nos diferentes nós, permitindo uma maior disponibilidade e desempenho.

**_Riak_**: Riak é um banco de dados distribuído de chave-valor que também enfatiza a consistência e a tolerância a falhas. Ele utiliza o conceito de modelo de consistência chamado "eventualmente consistente" para garantir a disponibilidade e escalabilidade. No Riak, as operações de gravação são enviadas para nós diferentes de forma independente, o que pode resultar em inconsistências temporárias nos dados, mas que são resolvidas conforme a replicação ocorre.

## O que significa SQL?
SQL significa Structured Query Language (Linguagem de Consulta Estruturada, em português). É uma linguagem de programação usada para gerenciar e manipular bancos de dados relacionais. O SQL foi projetado para permitir que os usuários definam, manipulem e recuperem dados armazenados em um banco de dados relacional.

## Em uma tabela de dados que é a Primary Key ou Chave Primária?
A Primary Key (chave primária) é um campo ou conjunto de campos que identifica exclusivamente cada registro na tabela. A chave primária garante a unicidade dos registros e é usada para indexar e acessar os dados de forma eficiente.

## Em uma tabela de dados que é a Foreign Key ou Chave Estrangeira?
A Foreign Key (chave estrangeira) é um campo ou conjunto de campos que estabelece uma relação entre duas tabelas. A chave estrangeira cria uma associação entre os registros de uma tabela com os registros de outra tabela, permitindo a criação de relacionamentos entre elas.

## O que significa que um relacionamento entre duas entidades é UM para UM?
Um relacionamento entre duas entidades é chamado de "um para um" quando um único registro em uma entidade está relacionado a no máximo um registro em outra entidade, e vice-versa. Isso significa que cada registro em uma entidade está associado a apenas um registro correspondente na outra entidade, e não há duplicação de relacionamentos.

## O que significa que um relacionamento entre duas entidades é UM para MUITOS?
Um relacionamento entre duas entidades é chamado de "um para muitos" quando um único registro em uma entidade está relacionado a vários registros em outra entidade, mas cada registro nessa segunda entidade está associado a apenas um registro correspondente na primeira entidade. Em outras palavras, um lado do relacionamento possui cardinalidade "um" e o outro lado possui cardinalidade "muitos".

## O que significa que um relacionamento entre duas entidades é de MUITOS para MUITOS?
Um relacionamento entre duas entidades é chamado de "muitos para muitos" quando vários registros em uma entidade estão relacionados a vários registros em outra entidade. Nesse tipo de relacionamento, cada registro em uma entidade pode estar associado a vários registros correspondentes na outra entidade, e vice-versa.

## Defina o que é um banco de dados
Um banco de dados é um sistema organizado de armazenamento e gerenciamento de dados, projetado para facilitar o armazenamento, recuperação, modificação e análise eficiente de informações. Ele é usado para armazenar e organizar dados de maneira estruturada, de modo que possam ser facilmente acessados, atualizados e utilizados por aplicativos e usuários.

## Defina o conceito de atributo
Um atributo é uma característica específica ou propriedade de uma entidade ou objeto armazenado em uma tabela. Também é conhecido como campo ou coluna. Os atributos representam as informações individuais que são armazenadas para cada instância de uma entidade.

##SQL Movies DB
## **Explique o conceito de normalização e por que ele é usado**
A normalização tem como objetivo principal eliminar anomalias e redundâncias nos dados, reduzindo a duplicação de informações e melhorando a eficiência das operações de consulta e manipulação dos dados. Ela é baseada em uma série de regras, conhecidas como formas normais, que definem critérios para a organização dos dados em tabelas.
As formas normais mais comumente utilizadas são:

**1ª** Forma Normal (1NF): Nessa forma normal, os dados são atomicamente indivisíveis, ou seja, não devem ser divididos em partes menores. Cada valor em uma tabela deve ser atômico, e não deve conter múltiplos valores.

**2ª** Forma Normal (2NF): Nessa forma normal, os dados devem estar na 1NF e, adicionalmente, não deve haver dependência parcial dos atributos não chave em relação à chave primária. Isso significa que todos os atributos não chave de uma tabela devem depender completamente da chave primária.

**3ª** Forma Normal (3NF): Nessa forma normal, os dados devem estar na 2NF e, além disso, não deve haver dependência transitiva entre os atributos não chave. Isso significa que nenhum atributo não chave deve depender de outro atributo não chave.
