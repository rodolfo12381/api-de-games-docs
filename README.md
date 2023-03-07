# API de Games
Documentação da API de games criada para fins de estudo e usando Node.js 

## Endpoints
### GET /games
Esse endpoint é responsável por retornar a listagem de todos os games cadastrados no banco de dados.
#### Parametros
Nenhum
#### Respostas
##### Ok! 200
Caso essa resposta aconteça você irá receber a listagem de todos os games

Exemplo de resposta:
```
[
        {
            "id": 23,
            "title": "Call of duty MW",
            "year": 2019,
            "price": 60
        },
        {
            "id": 65,
            "title": "Sea of Thieves",
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
##### Falha na autenticação! 401
Caso essa resposta aconteça, isso significa que aconteceu alguma falha durante o processo de autenticação da requisição. Motivos: Token inválido, Token expirado.

Exemplo de resposta:
```
{
    "err": "Token inválido"
}
```

### POST /auth
Esse endpoint é responsável por fazer o processo de login.
#### Parametros
email: email cadastrado
password: senha cadastrada
Exemplo:
```
{
    "email": "email",
    "password": "password"
}
```
#### Respostas
##### Ok! 200
Caso essa resposta aconteça você irá receber a listagem de todos os games

Exemplo de resposta:
```
[
        {
            "id": 23,
            "title": "Call of duty MW",
            "year": 2019,
            "price": 60
        },
        {
            "id": 65,
            "title": "Sea of Thieves",
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
##### Falha na autenticação! 401
Caso essa resposta aconteça, isso significa que aconteceu alguma falha durante o processo de autenticação da requisição. Motivos: Token inválido, Token expirado.

Exemplo de resposta:
```
{
    "err": "Token inválido"
}
```
