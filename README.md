## Desafio Técnico

## Engenheiro de Dados

### Objetivo

Desenvolvimento de um processo de ETL com foco na disponibilização de dados de modo a atender os requisitos descritos abaixo.

Esse teste deve avaliar a qualidade técnica na manipulacão de dados, otimizacão de performance, tratamento de qualidade e particionamento dos dados.

**Os dados de pessoas foram gerados de forma aleatória, utilizando a biblioteca FakerJS e FakerJS-BR**

LEMBRE-SE: A entrega deve conter TODOS os passos para o avaliador executar o programa (keep it simple).

### Caso

Você deverá implementar um programa, para ler, tratar e disponiblizar os dados para outras área consumirem.

Bases:
- Dados de funcionários de 3 diferentes filiais.</br>
- Dados de vendas de todas as filiais.</br>

Link: [dados]

### Requisitos

1 - Realizar as tratativas informadas abaixo salvando as informações em formato parquet. É interessante organizar os dados respeitando alguma regra de "camadas de dados". Justifique os critérios utilizados.</br>
2 - Desenvolvimento do processo utilizando linguagem Python/Scala com o framework de preferência (Spark será considerado diferencial).</br>

### Data Quality

1 - Realizar o tratamento da coluna `document` </br>
2 - Detectar através da coluna `document` se o registro é um CPF ou CNPJ, adicionando uma nova coluna</br>
3 - Realizar o tratamento da coluna `birthDate`</br>
4 - Existe outras colunas para fazer esses tratamentos? Se sim, aplicar as correções</br>

### Agregação dos dados 
Gerar bases atendendo as respostas abaixo:
1 - Top 5 melhores vendedores</br>
2 - Qual é o valor médio vendido por estado?</br>
4 - Qual é o CNPJ que vendeu menos?</br>
5 - Último carro vendido de cada vendedor, filial e data da venda.</br>

### Particionamento de dados tratados com as regras descritas acima

1 - Particionar em arquivos por estado</br>
2 - Particionar em arquivos por ano/mes/dia através da coluna `birthDate` ou data da venda (`date`), quando aplicável.</br>

### Arquitetura

Apresentar um documento com a arquitetura proposta para execução desse projeto em nuvem (AWS de preferência). Desde a ingestão, orquestração, processamento, disponibilização e ferramentas de consumo dos dados.

 - Apresentação poderá ser feita na sua própria máquina. </br>
 - O projeto deve ser disponibilizado em um repositório git de sua prefêrencia desde que o avaliador tenha acesso.

[dados]: ../dados/
