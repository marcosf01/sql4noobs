## Inserindo dados na tabela

INSERT INTO [TABELA DE PRODUTOS] VALUES (
'104017',
'Light - 350 ml - Melância',
'Lata',
'350 ml',
'Melancia',
4.56
);

<br>

<em>Como fazer para inserir quando os valores estão em posições diferentes?</em> <br><br>
INSERT INTO FILMES ([Nome], [Genero], [Lancamento], [Duracao], [Id_filme] ) <br>
VALUES <br>
( "Toy Story"              , "Aventura", '1995-12-22' , 81   , 1), <br>
( "O Silêncio dos Inocentes" , "Suspense" , '1991-05-17' , 118  , 2), <br>
( "Coringa"                  , "Drama"    , '2019-10-03' , 122  , 3); 
