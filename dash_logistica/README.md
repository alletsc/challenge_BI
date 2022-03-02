# Dashboard de Logistica

<p aling='center'>
        <img width="600" height="300" src="https://raw.githubusercontent.com/alletsc/challenge_BI/main/src/images/process.png">

## Problema de negócio:

A pessoa que gerencia a área de logística da Fast Sheep, está enfrentando algumas mudanças em sua área por conta do aumento da demanda dos serviços de logística no período da **pandemia**. Ela quer **manter a qualidade** de seu serviço, mas para isso precisa acompanhar constantemente as métricas do seu departamento para tomar as melhores decisões. Quando nos contou isso, analisamos que para auxiliar nesse desafio precisaremos fazer um dashboard para logística. Para isso, vamos visualizar algumas métricas muito importantes para a área.

## O que quero visualizar nesse relatório?

1. Visualizar o nível médio de estoque disponível por ano;

2. Visualizar o valor do estoque por ano;

3. Visualizar a média de dias para o produto ser entregue por mês, ano e UF;

4. Quantidade de pedidos por UF;

5. Quantidade de pedidos por mês, ano e UF;

6. Quantidae de pedidos entregues, com entrega em andamento e atrasados;

7. Faturamento por ano;

8. UFs com maior valor de faturamento;

9. Faturamento por categoria de produto;

10. Faturamento por mês;


## Extração

Os dados brutos utilizados neste relatório foram fornecidos pela empresa em 4 arquivos .csv divididos em:

> Tabela Estoque.csv;

>Tabela Pedidos.csv;

>Tabela  Veículos.csv

>Tabela Produtos.csv

## Transformação

Limpeza dos  dados extraídos,  aplicação das regras de negócio e validação dos dados na staging area como preparação para carga.

Tabela | Transformações
:------ | :--------------
Tabela Estoque | Normalização dos dados; Correção da coluna `data_atualizacao` substituindo valores e alteração do tipo usando a localidade.
Tabela Pedidos | Alterar região de origem dos dados; Normalização dos dados;  Criação das colunas `data_column_name` e `hora_column_name`; Alteração do tipo das colunas `id_column_name`, `hora_column_name`, `data_column_name`; Correção das colunas `Latitude` e `Longitude`; Remoção de valores em branco;
Tabela Produtos | Normalização dos dados;
Tabela Veículos | Normalização dos dados; Correção da coluna `ID_Veículo`;
Medidas |  Calendário; Faturamento;  Valor do estoque; Pedidos entregue; Pedido atrasados; Pedidos Trânsito.

## Load

Estrutura do Data Warehouse

<p aling='center'>
        <img width="600" height="300" src="https://raw.githubusercontent.com/alletsc/challenge_BI/main/src/images/logo/rel_tabelas.png?token=AQYHTDKPSGYU6HPPLJKL6SLBW3FZ6">

## Analysis

<p aling='center'>
        <img width="600" height="300" src="https://raw.githubusercontent.com/alletsc/challenge_BI/main/src/images/logo/dash_1.png?token=AQYHTDMQG2FCHMMAQ7P4U4DBW3FEC">

<p aling='center'>
        <img width="600" height="300" src="https://raw.githubusercontent.com/alletsc/challenge_BI/main/src/images/logo/dash_2.png?token=AQYHTDNB75ZXE2OOFG6T5QLBW3FG6">

### Habilidade exercitadas nesse projeto

- Desing de dashboards;

- Funções Dax (Data Analysis Expressions);

- ETL com Power BI Desktop.



