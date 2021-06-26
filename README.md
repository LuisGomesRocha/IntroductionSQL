# Introdução ao SQL com MySQL

<h1 align="center">
    <a href="https://cursos.alura.com.br/formacao-oracle-mysql/">🔗 Introdução ao SQL com MySQL: Manipule e consulte dados </a>
</h1>

<p align="justify"> :robot: Somos muitos alunos e alunas aqui no Bootcamp. Em função de todas as avaliações respondidas, muitos dados são gerados. E agora temos alguns desafios para você :robot: </p>

<p align="justify"> :robot: Dado que todo(a) aluno(a) tem um email(máximo de 30 caracteres),nome(máximo de 30 caracteres) e idade(entre 1 e 100) :robot: </p>

### Features

- [x] O que você faria para representar essa estrutura no banco? 
- [x] O que você precisa fazer agora para inserir novos(as) alunos(as) nessa tabela?
- [x] E para apagar um registro pelo email?
- [x] Agora você precisa buscar todos os(as) alunos(as) que tem Zup no email. Como você faria?
- [x] E para fechar é necessário que alunos e alunas sejam listados pela sua idade em ordem crescente

<h3 align="justify">
   O que você faria para representar essa estrutura no banco? 
</h3>

 ``` 
CREATE DATABASE CADASTRO
USE CADASTRO
CREATE TABLE ALUNOS (
ID INT PRIMARY KEY NOT NULL,
NOME VARCHAR (30),
EMAIL VARCHAR (30),
IDADE INT  (3)
)
GO

``` 

<h3 align="justify">
   O que você precisa fazer agora para inserir novos(as) alunos(as) nessa tabela? 
</h3>

   ``` 
 INSERT INTO ALUNOS (NOME, EMAIL, IDADE) VALUES ('Luis Gomes', 'luisgomes@gmail.com', '36');
	
  ``` 


<h3 align="justify">
   E para apagar um registro pelo email?
</h3>

   ``` 
DELETE FROM ALUNOS WHERE EMAIL =  'luisgomes@gmail.com'
	
  ``` 


<h3 align="justify">
   Agora você precisa buscar todos os(as) alunos(as) que tem Zup no email. Como você faria?
</h3>

   ``` 
   SELECT * FROM ALUNOS WHERE email LIKE '%@zup.com.br%';

  ``` 

<h3 align="justify">
   E para fechar é necessário que alunos e alunas sejam listados pela sua idade em ordem crescente
</h3>
 
   ``` 
SELECT * FROM ALUNOS
WHERE  idade
ORDER BY  ASC;
	
  ``` 
