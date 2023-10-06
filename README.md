<h1 align="center"> SQL4Noobs</h1>

<img src="./images/Frame 5.svg" alt="SQL Server Logo">

<p align="center">Aprenda os comandos em SQL e reaproveite os códigos para copiar, colar e editar!</p>

[Tipos de dados](docs/tipos.md)

# Tipos de dados

| Tipo | Descrição |
| --- | --- |
| CHAR | Quantidade determinada de caracteres |
| VARCHAR | Quantidade indeterminada de caracteres |
| DATE | Padrao americano para data |
| SMALLINT | Numérico do tipo Int. Usado para economizar espaço no banco |
| FLOAT | Numérico para casa decimal |
| MONEY | Para valores monetários |
| SMALLMONEY | Para valores monetários. Usado para economizar espaço no banco |
| BIT | Para valores binários(0/1) |

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

Como fazer para inserir quando os valores estão em posições diferentes? <br>
INSERT INTO FILMES ([Nome], [Genero], [Lancamento], [Duracao], [Id_filme] ) <br>
VALUES <br>
( "Toy Story"              , "Aventura", '1995-12-22' , 81   , 1), <br>
( "O Silêncio dos Inocentes" , "Suspense" , '1991-05-17' , 118  , 2), <br>
( "Coringa"                  , "Drama"    , '2019-10-03' , 122  , 3); 

## Selecionando todos os registros

SELECT * FROM [TABELA DE PRODUTOS];

## Selecionando campos

SELECT [NOME], [ESTADO] FROM [TABELA DE PRODUTOS];

## Ordenando os registros

SELECT * FROM [TABELA DE PRODUTOS] ORDER BY NOME

## Como apelidar uma coluna(alias)
SELECT [NOME] AS [NOME DO CLIENTE], [ESTADO] AS [UF] FROM [TABELA DE CLIENTES]

## Como filtrar sem repetições
SELECT DISTINCT [NOME] AS [NOME DO CLIENTE] FROM [TABELA DE CLIENTES]

## Para selecionar registros específicos

SELECT [NOME] AS [NOME DO CLIENTE], [ESTADO] AS [UF], [PRIMEIRA COMPRA] <br>
FROM [TABELA DE CLIENTES] <br>
WHERE [PRIMEIRA COMPRA] = 1

