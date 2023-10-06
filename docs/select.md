# Select

## Selecionando todos os registros

```swift
SELECT * FROM [TABELA DE PRODUTOS]; 
```


## Selecionando campos

```swift
SELECT [NOME], [ESTADO] FROM [TABELA DE PRODUTOS];
```


## Ordenando os registros

```swift
SELECT * FROM [TABELA DE PRODUTOS] ORDER BY NOME
```

## Como apelidar uma coluna(alias)

```swift
SELECT [NOME] AS [NOME DO CLIENTE], [ESTADO] AS [UF] FROM [TABELA DE CLIENTES]
```
```swift
## Como filtrar sem repetições
SELECT DISTINCT [NOME] AS [NOME DO CLIENTE] FROM [TABELA DE CLIENTES]
```

## Para selecionar registros específicos

```swift
SELECT [NOME] AS [NOME DO CLIENTE], [ESTADO] AS [UF], [PRIMEIRA COMPRA] <br>
FROM [TABELA DE CLIENTES] <br>
WHERE [PRIMEIRA COMPRA] = 1
```

