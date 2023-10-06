# SQL4Noobs

<a ref="docs/tipos.md">Tipo de dados</a>

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

