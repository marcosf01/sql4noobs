# Alter Table

### Alterando uma tabela

```swift
ALTER TABLE [TABELA DE CLIENTES] ALTER COLUMN [CPF] CHAR (11) NOT NULL;
```

### Colocando uma chave primária num campo

```swift
ALTER TABLE [TABELA DE CLIENTES] ADD CONSTRAINT PK_TABELA_CLIENTE 
PRIMARY KEY CLUSTERED (CPF);
```
