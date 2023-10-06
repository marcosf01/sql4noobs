# SQL4Noobs

<h1 align="center">
  <img src="./images/microsoft-sql-server 1.png" alt="SQL Server Logo" width="150">
</h1>

[Tipos de dados](docs/tipos.md)

<p align="center">Tenha todos os comando em SQL em um só lugar! Copie, cole e edite.</p>

### Criar Banco de Dados
CREATE DATABASE <em>Nome_do_banco</em>

### Excluir Banco de Dados
DROP DATABASE <em>Nome_do_banco</em>

### Criando uma tabela
CREATE TABLE [TABELA DE CLIENTES] ( <br>
CPF CHAR (11),<br>
NOME VARCHAR (150),<br>
RUA VARCHAR (150),<br>
COMPLEMENTO VARCHAR (150),<br>
BAIRRO VARCHAR (150),<br>
ESTADO CHAR (2),<br>
CEP CHAR (8),<br>
[DATA DE NASCIMENTO] DATE,<br>
IDADE SMALLINT,<br>
SEXO CHAR (1),<br>
[LIMITE DE CREDITO] MONEY,<br>
[VOLUME MINIMO] FLOAT,<br>
[PRIMEIRA COMPRA] BIT
)

## Alterando uma tabela

ALTER TABLE [TABELA DE CLIENTES] ALTER COLUMN [CPF] CHAR (11) NOT NULL;

## Colocando uma chave primária num campo

ALTER TABLE [TABELA DE CLIENTES] ADD CONSTRAINT PK_TABELA_CLIENTE 
PRIMARY KEY CLUSTERED (CPF);

## Inserindo dados na tabela

INSERT INTO [TABELA DE PRODUTOS] VALUES (
'104017',
'Light - 350 ml - Melância',
'Lata',
'350 ml',
'Melancia',
4.56
);



