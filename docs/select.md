## Selecionando todos os registros

SELECT * FROM [TABELA DE PRODUTOS];

#

## Selecionando campos

SELECT [NOME], [ESTADO] FROM [TABELA DE PRODUTOS];

#

## Ordenando os registros

SELECT * FROM [TABELA DE PRODUTOS] ORDER BY NOME

#

## Como apelidar uma coluna(alias)
SELECT [NOME] AS [NOME DO CLIENTE], [ESTADO] AS [UF] FROM [TABELA DE CLIENTES]

#

## Como filtrar sem repetições
SELECT DISTINCT [NOME] AS [NOME DO CLIENTE] FROM [TABELA DE CLIENTES]

#

## Para selecionar registros específicos

SELECT [NOME] AS [NOME DO CLIENTE], [ESTADO] AS [UF], [PRIMEIRA COMPRA] <br>
FROM [TABELA DE CLIENTES] <br>
WHERE [PRIMEIRA COMPRA] = 1
