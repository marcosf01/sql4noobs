# Create

### Criar e excluir Banco de Dados

```swift
CREATE DATABASE Nome_do_banco
DROP DATABASE Nome_do_banco
```

### Criando uma tabela

```swift
CREATE TABLE [TABELA DE CLIENTES] ( 
    CPF CHAR (11),
    NOME VARCHAR (150),
    RUA VARCHAR (150),
    COMPLEMENTO VARCHAR (150),
    BAIRRO VARCHAR (150),
    ESTADO CHAR (2),
    CEP CHAR (8),
    [DATA DE NASCIMENTO] DATE,
    IDADE SMALLINT,
    SEXO CHAR (1),
    [LIMITE DE CREDITO] MONEY,
    [VOLUME MINIMO] FLOAT,
    [PRIMEIRA COMPRA] BIT
)
```