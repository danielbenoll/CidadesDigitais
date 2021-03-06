# Adonis API application

This is the boilerplate for creating an API server in AdonisJs, it comes pre-configured with.

1. Bodyparser
2. Authentication
3. CORS
4. Lucid ORM
5. Migrations and seeds

## Setup

Use the adonis command to install the blueprint

```bash
adonis new yardstick --api-only
```

or manually clone the repo and then run `npm install`.


### Migrations

Run the following command to run startup migrations.

```js
adonis migration:run
```



1 - Instalar o Git (https://git-scm.com/)
2 - Instalar o NodeJS (https://nodejs.org/en/)
3 - Criar Projeto:
	- Via terminal (prompt de comando) no diretório desejado, digite os seguintes comandos:
		npm i --global @adonisjs/cli
		adonis new escola-api --api-only
4 - Abra o novo projeto criado com a IDE de sua preferência
5 - No terminal na raiz do projeto, digite: 
	adonis serve --dev

Comandos comuns:

Para criação de Arquivos:

// Migration
adonis make:migration curso 

// Controller
adonis make:controller Curso

// Model
adonis make:model Curso

// Tudo Junto
adonis make:model Curso -m -c

// Seeder
adonis make:seed Curso	

// Instalar Mysql
npm i mysql


// Executar Migration
adonis migration:run

// Reiniciar Migration
adonis migration:refresh

// Executar Migration com seeders
adonis migration:run --seed


API REST / RESTful
REpresentational State Transfer

Request
Verbos HTTP

GET - Consultas, pesquisas, recuperar dados
POST - Inserir dados
PUT - Alterar dados
DELETE - Deletar dados



ADONIS JS - Framework NodeJS
Rotas
Requisições HTTP
Controllers
Migration



//Validação
1 - adonis install @adonisjs/validator
2 - '@adonisjs/validator/providers/ValidatorProvider' (start/app.js dentro do providers)
3 - adonis make:validator Aluno
4 - Criar regras no Validator (app\Validators\Aluno.js)
5 - Adicionar o Validator nas rotas
Route.resource('/alunos', 'AlunoController')
     .apiOnly()
     .validator(new Map([
       [['store', 'update'], 'Aluno']
     ]))

//Documentação de validação de campos
indicative-v5.adonisjs.com


//ADONIS SWAGGER
github.com/ahmadarif/adonis-swagger
