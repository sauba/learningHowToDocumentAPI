# learning HowTo Document an API
###### PT-BR ## API de Games do Curso Formação Nodejs na Udemy.
###### EN
In this repository, i will be doing what i am learning at udemy course named Formação Nodejs

#### Endpoints

##### GET /games

###### PT-BR
Esse endpoint é responsável por retornar a listagem de todos os games no banco de dados.

###### EN
this endpoint is responsible  to return the game´s list from database

###### Parametros | Params
Nenhum | None

###### Respostas | Awnsers
##### OK ! 200
###### PT-BR
Caso essa resposta aconteça você receberá a listagem de games do banco de dados
###### EN
In case you got this awnser you will receive a game´s list from the database

```
Exemplo | Example

[
    {
        "id": 23,
        "title": "Call of duty MW",
        "year": 2019,
        "price": 60
    },
    {
        "id": 65,
        "title": "Sea of thieves",
        "year": 2018,
        "price": 40
    },
    {
        "id": 2,
        "title": "Minecraft",
        "year": 2012,
        "price": 20
    }
]

```



##### Falha de Autenticação | Authentication Failure - Error 401

```
{
    "err": "Token inválido!" 
}

``` 
###### PT-BR
Caso essa resposta aconteça, isso significa que houve alguma falha durante o processo de autenticação da requisição. Motivos: Token Inválido ou Expirado.
###### EN
In case you got this awnser it means that you are having some problem at the requirement of authentication process. Possibles Reasons: Token is probabily Invalid or Expired





###### PT-BR

###### EN


##### POST /auth

###### PT-BR
Esse endpoint é responsável por autenticar o usuario 

###### EN
this endpoint is responsible  to authenticate user

###### Parametros | Params
email e password cadastrados no sistema. | email and password of the user

```
Exemplo | Example

{
    "email": "user@test.com!",
    "password": "123456789"
}

```
###### Respostas | Awnsers
##### OK ! 200
###### PT-BR
Caso essa resposta aconteça você receberá a listagem de games do banco de dados
###### EN
In case you got this awnser you will receive a game´s list from the database

```
Exemplo | Example

[
    {
        "id": 23,
        "title": "Call of duty MW",
        "year": 2019,
        "price": 60
    },
    {
        "id": 65,
        "title": "Sea of thieves",
        "year": 2018,
        "price": 40
    },
    {
        "id": 2,
        "title": "Minecraft",
        "year": 2012,
        "price": 20
    }
]

```



##### Falha de Autenticação | Authentication Failure - Error 401

###### PT-BR
Caso essa resposta aconteça, isso significa que houve alguma falha durante o processo de autenticação da requisição. Motivos: e-mail ou senha incorretos.
###### EN
In case you got this awnser it means that you are having some problem at the requirement of authentication process. Possibles Reasons: e-mail or password or both are incorrects.

```
{
    "err": "Token inválido!" 
}

``` 
