<h1 align="center" style="font-weight: bold;">API para cadastro de pessoas</h1>

<p align="center">
 <a href="#tech">Tecnologias</a> • 
 <a href="#started">Getting Started</a> • 
  <a href="#routes">API Endpoints</a> •
 <a href="#colab">Collaborators</a> •
 <a href="#contribute">Contribute</a>
</p>

<p align="center">
    <b>O sistema se trata de uma simples API rest criada com intuito de fazer cadastro de pessoas. Essa foi a minha solução para uma das atividades durante meu tempo como traine da InfoJR, uma empresa júnior de informática da UFBA.</b>
</p>

[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)

<h2 id="technologies">💻 Technologies</h2>

![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![Nodemon](https://img.shields.io/badge/NODEMON-%23323330.svg?style=for-the-badge&logo=nodemon&logoColor=%BBDEAD)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white)


<h2 id="started">🚀 Vamos conhecer a aplicação!</h2>

<h3>Prerequisitos</h3>

- [NodeJS](https://github.com/)
- [Git 2](https://github.com)

<h3>Clonando</h3>

```bash
git clone https://github.com/Jaedsonn/APIrest-de-cadastro.git
```

<h3>Rodando o projeto</h3>


```bash
cd APIrest-de-cadastro
npm i
npm run dev
```

<h2 id="routes">📍 API Endpoints</h2>

Rotas da API.
​
| route               | description                                          
|----------------------|-----------------------------------------------------
| <kbd>POST /usuario/cadastro</kbd>     | rota para cadastro de uma nova pessoa [request details](#post-details)
| <kbd>GET /usuario/id/:id</kbd>     | rota para encontrar uma pessoa pelo id [request details](#get-id-details)
| <kbd>GET /usuario/email/:email</kbd>     | rota para encontrar uma pessoa pelo email [request details](#get-email-details)
| <kbd>GET /usuario/nome/:nome</kbd>     | rota para encontrar uma pessoa pelo nome [request details](#get-nome-details)
| <kbd>DELETE /usuario/deletar/:id</kbd>     | rota para deletar uma pessoa pelo id de cadastro[request details](#delete-user-id)
| <kbd>PUT /usuario/atualizar/:id</kbd>     | rota para atualizar uma pessoa pelo id de cadastro [request details](#put-user-id)

<h3 id="post-details">POST /usuario/cadastro</h3>

**REQUEST**
```json
{
"nome":"Keila",
 "idade":19,
 "email":"keila@gmail.com",
 "senha":"jaja123",
 "estado":"bahia",
 "cidade":"Serrolândia"
}
```

**RESPONSE**
```json
{
    "msg": "Usuário cadastrado!",
    "user": {
        "id": 14,
        "nome": "Keila",
        "email": "keila@gmail.com",
        "senha": "jaja123",
        "idade": 19,
        "estado": "bahia",
        "cidade": "Serrolândia"
    }
}
```


<h3 id="get-id-details">GET /usuario/id/:id</h3>

**RESPONSE**
```json
{
 {
    "msg": "Usuários encontrados!",
    "user": {
        "id": 11,
        "nome": "Fernanda Silva Santos Jesus",
        "email": "fermam@gmail.com",
        "senha": "jaja123",
        "idade": 19,
        "estado": "bahia",
        "cidade": "Serrolândia"
    }
}
}
```


<h3 id="get-email-details">GET /usuario/email/:email</h3>

**RESPONSE**
```json
{
 {
    "msg": "Usuários encontrados!",
    "user": {
        "id": 11,
        "nome": "Fernanda Silva Santos Jesus",
        "email": "fermam@gmail.com",
        "senha": "jaja123",
        "idade": 19,
        "estado": "bahia",
        "cidade": "Serrolândia"
    }
}
}
```


<h3 id="get-nome-details">GET /usuario/nome/:nome</h3>

**RESPONSE**
```json
{
 {
    "msg": "Usuários encontrados!",
    "user": {
        "id": 11,
        "nome": "Fernanda Silva Santos Jesus",
        "email": "fermam@gmail.com",
        "senha": "jaja123",
        "idade": 19,
        "estado": "bahia",
        "cidade": "Serrolândia"
    }
}
}
```


<h3 id="delete-user-id">DELETE /usuario/deletar/:id</h3>

**RESPONSE**
```json
{
    "msg": "Usuário deletado!",
    "user": {
        "id": 11,
        "nome": "Fernanda Silva Santos Jesus",
        "email": "fermam@gmail.com",
        "senha": "jaja123",
        "idade": 19,
        "estado": "bahia",
        "cidade": "Serrolândia"
    }
}
```


<h3 id="put-user-id">PUT /usuario/atualizar/:id</h3>

**REQUEST**
```json
{
 "nome":"Fernanda Silva Santos Jesus",
 "idade":19,
 "email":"Fernandona@gmail.com",
 "senha":"jaja123",
 "estado":"bahia",
 "cidade":"Serrolândia"
}
```

**RESPONSE**
```json
{
    "msg": "Usuário Atualizado!",
    "user": {
        "id": 12,
        "nome": "Fernanda Silva Santos Jesus",
        "email": "Fernandona@gmail.com",
        "senha": "jaja123",
        "idade": 19,
        "estado": "bahia",
        "cidade": "Serrolândia"
    }
}
```

<h2 id="contribute">📫 Contribute</h2>

Se você quiser contribuir com o meu projeto basta seguir os comandos abaixo☺️

1. `git clone https://github.com/Jaedsonn/APIrest-de-cadastro.git`
2. `git checkout -b feature/NAME`
3. Abra um Pull Request explicando o problema resolvido ou o recurso criado, se houver, anexe uma captura de tela das modificações visuais e aguarde a revisão!

<h3>Documentos que podem ajudar</h3>

[📝 How to create a Pull Request](https://www.atlassian.com/br/git/tutorials/making-a-pull-request)
