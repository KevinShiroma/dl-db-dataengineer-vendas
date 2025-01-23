# Projeto de Ingestão de Dados com Databricks

Este projeto foi desenvolvido para consolidar meus conhecimentos sobre Big Data e suas ferramentas, utilizando o Databricks como plataforma principal. O objetivo é criar um processo de ingestão de dados de ponta a ponta, finalizando na visualização dos dados no Power BI. <br>

![Trazendo os dados CSV](https://github.com/KevinShiroma/dl-db-dataengineer-vendas/blob/main/img/7.PNG?raw=true)

## Objetivos do Projeto

- Demonstrar a ingestão de dados utilizando o Databricks.
- Implementar uma arquitetura de dados eficiente e escalável.
- Visualizar os dados processados no Power BI.

## Aprendizados

Durante o desenvolvimento deste projeto, aprendi conceitos importantes, incluindo:

- **Delta Lakehouse**: A importância do Delta Lake na construção de um Lakehouse eficiente.
- **Apache Spark e PySpark**: Compreensão do funcionamento do Apache Spark e como utilizar PySpark para processamento de dados.
- **Arquitetura Medallion**: Desenvolvimento e implementação da arquitetura medallion para organização dos dados.
- **Estratégias de Carga de Dados**: Diferenciação entre cargas de dados FULL e Incremental, e quando utilizar cada uma.
- **Boas Práticas com Delta Lake**: Aplicação de boas práticas ao trabalhar com Delta Lake para garantir a integridade e eficiência dos dados.

## Tecnologias Utilizadas

- Databricks
- Apache Spark
- PySpark
- Delta Lake
- Power BI

## Desenvolvimento

### Landing Zone
Após o provisionamento do Databricks e a criação do DBFS , foi criado um notebook para colocar os dados de um CSV sobre um relatório de vendas na Landing Zone.<br>
![Trazendo os dados CSV](https://github.com/KevinShiroma/dl-db-dataengineer-vendas/blob/main/img/1.PNG?raw=true)

### Camada Bronze
Em seguida os dados foram colocados na camada bronze para persistir os dados.<br>
![Trazendo os dados CSV](https://github.com/KevinShiroma/dl-db-dataengineer-vendas/blob/main/img/2.PNG?raw=true)

E assim podemos visualizar o Dataframe criado.<br>
![Trazendo os dados CSV](https://github.com/KevinShiroma/dl-db-dataengineer-vendas/blob/main/img/3.PNG?raw=true)

### Camada Silver
Com isso, podemos colocar nossos dados na camada Silver para realizar o tratamento dos dados.<br>
![Trazendo os dados CSV](https://github.com/KevinShiroma/dl-db-dataengineer-vendas/blob/main/img/4.PNG?raw=true)

### Camada Gold
Em seguida, podemos criar a tabela fato e suas dimensões para que possa ser criado o dashboard. <br>
![Trazendo os dados CSV](https://github.com/KevinShiroma/dl-db-dataengineer-vendas/blob/main/img/5.PNG?raw=true)

### Power BI
Com a camada Gold criada, nos conectamos com o Power BI e finalmente criar nosso dashboard, bem como a visualização dos dados para o relatório de vendas.<br>
![Trazendo os dados CSV](https://github.com/KevinShiroma/dl-db-dataengineer-vendas/blob/main/img/6.PNG?raw=true)


1. Clone este repositório:
   ```bash
   git clone https://github.com/seu_usuario/seu_repositorio.git
