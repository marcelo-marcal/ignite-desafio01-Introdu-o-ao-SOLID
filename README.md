# Ignite Node.JS 
## Chapter II desafio 01 Introdu o ao SOLID



Criar uma aplicação de listagem e cadastro de usuários. Para que a listagem de usuários funcione, o usuário que solicita a listagem deve ser um admin, utilizando os conceitos de SOLID.

### Requisitos: Rotas da aplicação.

POST /users
PATCH /users/:user_id/admin
GET /users/:user_id
GET /users/:user_id

## Específicação dos testes

### Teste do model:
Para rodar os teste: yarn test

- Should be able to create an user with all props
 
img 01

### Testes do repositório

- Should be able to create new users
- Should be able to list all users
- Should be able to find user by ID
- Should be able to find user by e-mail address
- Should be able to turn an user as admin

img 02

### Testes de useCases

- Should be able to create new users
- Should not be able to create new users when email is already taken
- Should be able to turn an user as admin
- Should not be able to turn a non existing user as admin

- Should be able to get user profile by ID
- Should not be able to show profile of a non existing user
img 03

- Should be able to list all users
- Should not be able to a non admin user get list of all users
- Should not be able to a non existing user get list of all users
img 04


### Testes das rotas

- **Rota - [POST] /users**
- **Rota - [PATCH] /users/:user_id/admin**
- **Rota - [GET] /users/:user_id**
- **Rota - [GET] /users**
img 06

img Fim