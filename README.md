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
##### Falha na autenticação! 401
Caso essa resposta aconteça, isso significa que aconteceu alguma falha durante o processo de autenticação da requisição. Motivos: Token inválido, Token expirado.
