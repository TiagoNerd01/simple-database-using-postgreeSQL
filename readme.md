# 1- Introdução
## 1.1- O que é SQL?
- SQL significa Linguagem de Consulta estruturada e é frequentimente pronunciada como *Sequel*
- É usado para interagir com dados armazenados em bancos de dados, permitindo que os
usuários façam cálculos complexos como encontrar **“Gasto Total?”** em grandes conjuntos de dados.
##  1.2- Porque aprender SQL?
- **Falar com os dados**: Permite comunicar diretamente com sistemas de dados.
- **Alta demanda**: Há uma alta demanda por habilidades em SQL em várias funções técnicas
- **Caminhos de carreira**: É essencial para:
    - Desenvolvedores de software
    - Analistas de dados
    - Cientistas de dados
    - Engenheros de dados
- **Padrão da indústria**: É uma linguagem padrão usada com ferramentas como **Power BI, Tableau, Kafka, Spark e Synapse**.
## 1.3 Sistema de Gerenciamento de Banco de Dados (DBMS)
- Um **DBMS (Sistema de Gerenciamento de Banco de Dados)** atua como interface entre o usuário e o banco de dados.
  - Hospedagem do Servidor: Os bancos de dados normalmente são hospedados em um **servidor ou na nuvem**.
  - Disponibilidade 24/7: Esses sistemas geralmente funcionam o tempo todo para garantir que os dados estejam sempre acessíveis
  - Interação: **Aplicativos (APP </>)**, ferramentas de **BI (Power BI)** e usuários enviam consultas **SQL** ao **DBMS** para gerenciar e recuperar dados.
## 1.4 Tipos de banco de dados
| **Categoria**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | **Exemplos** |
|---------------|--------------|
|Relacional     | Microsoft SQL Server, MySQL, PostgreSQL, Amazon Redshift    |
|Documento      | MongoDB      |
|Grafo          | Neo4j        |
|Chave-valor   | Redis, Amazon DynamoDB |
|Base de coluna| Apache Cassandra (GitHub)
## 1.5 Estrutura de Banco de Dados
- Bancos de dados **relacionais** seguem uma organização hierárquica:
    - **Servidor**: O host principal contendo um ou mais bancos de dados
    - **Banco de Dados**: Contêiner de alto nível para dados, como **“Vendas”** ou **“RH”**.
    - **Esquema**: Agrupamentos lógicos dentro de um banco de dados, como **“Pedidos”** ou **“Clientes”**
    - **Tabela**: Onde os dados são fisicamente armazenados em linhas e colunas.
## 1.6 Componentes de uma tabela 
- **Colunas**: Categorias verticais definindo tipos de dados
- **Linhas**: Registros horizontais individuais
- **Célula**: Uma unidade única de dado na interseção de linha e coluna.
- **Chave primária**: Identificador único para cada registro em uma tabela.
- **Armazenamento**: Tabelas são armazenadas  arquivos de banco de dados em disco físico.
## 1.7 Tipos de Dados
- **SQL** usa tipos de dados específicos para definir que tipo de informação pode ser armazenada:
- **Numéricos**:
    - **INT** - números inteiros
    - **DECIMAL** - Valores numéricos com frações
- **Texto/String**
    - **CHAR** - Strings de comprimento fixo
    - **VARCHAR** - Strings de comprimento variável 
- **Data & Hora**
    - **DATE**- Formato 'YYY-MM-DD'
    - **TIME**- Formato 'HH:MM:SS'
## 2 Tipos de comando SQL
### DDL (linguagem de definição de dados)
- Usada para definir ou modificar a estrutura do banco de dados
    - **CREATE** – Criar novos bancos de dados ou tabelas.
    - **ALTER** – Modificar a estrutura existente
    - **DROP** – Deletar um banco ou tabela.
### DQL (Linguagem de consulta de dados)
- Usada para recuperar dados do banco de dados.
    - **SELECT** – O comando principal para buscar dados.
### DML (Linguagem de Manipulação de Dados)
- Usada para gerenciar dados dentro das tabelas
    - **INSERT** – Adicionar novos registros.
    - **UPDATE** – Modificar registros existentes
    - **DELETE** – Remover registros
### DCL (Linguagem de Controle de Dados)
- Usada para gerenciar permissões e controle de acesso
    - **GRANT** – Concede privilégios de acesso.
    - **REVOKE** – Revoga privilégios
### TCL (Linguagem de Controle de Transações)
- Usada para gerenciar transações no banco de dados
    - **COMMIT** – Salva mudanças permanentemente
    - **ROLLBACK** – Desfaz mudanças se ocorrer um erro
    - **SAVEPOINT** – Define um ponto para rollback parcial
## 2.1 DDL - Linguagem de Definição de Dados
- DDL significa Data Definition Language (Linguagem de Definição de Dados).
- Enquanto o DQL é usado para consultar dados e o DML é usado para manipular dados, o DDL é usado para definir a estrutura dos nossos objetos de dados (o "esqueleto" do banco de dados).
## 2.2 Operações Principais de DDL
- O **DDL** permite que você gerencie a **planta estrutural (blueprint)** do seu banco de dados através de três ações principais:
    - **CREATE** - Usado para construir novos objetos (Bancos de Dados ou Tabelas) do zero.
    - **ALTER** - Usado para modificar a estrutura de um objeto existente (ex: adicionar uma nova coluna a uma tabela).
    - **DROP** - Usado para excluir permanentemente um objeto e todos os seus dados.
## 2.3 Criando Objetos (CREATE)
- **CREATE DATABASE Sales**; - Para começar um novo projeto, primeiro criamos um contêiner para nossas tabelas.
- **CREATE TABLE** - Ao criar uma tabela, devemos definir as Colunas e seus Tipos de Dados associados:
    - CREATE TABLE Products (
  ProductID INT,
  ProductName VARCHAR(100),
  Price DECIMAL
);
## 2.4 Modificando Objetos (ALTER)
- Se os requisitos mudarem, usamos o comando **ALTER** para atualizar a estrutura sem excluir a tabela
- Adicionar uma Coluna
    - **ALTER TABLE Products**
    - **ADD Category VARCHAR(50)**;

- Remover uma Coluna
    - **ALTER TABLE Products**
    - **DROP COLUMN Price**;
##2.5 Excluindo Objetos (DROP)
- O comando **DROP** é **destrutivo**. Ele remove toda a estrutura e todos os registros armazenados nela
    - DROP TABLE Products;
## 2.5 Tabela Resumo de DDL

| comando | ação| Objeto afetado|
|---------| ------| ------------|
Create| Construir novo| Banco de dados, tabela, schema|
|Alter| Modificar existente| Colunas, tipos de dados|
DROP| Excluir| Banco de dados, tabela, schema|

## 3 

    

    
    
    