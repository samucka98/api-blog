## API-Blog com .NET C#

Este foi um projeto que desenvolvi uma API Rest de um blog durante o treinamento da carreira .net pelo Balta.io, e nele tive a oportunidade de aprender conceitos e ferramentas do ecossistema .net sempre levando em consideração a performance nos cenários apropriados, outras ferramentas como o Docker, revisar fundamentos importantes como logica de programação e programação orientada a objetos usando C#, banco de dados relacionais e etc.

---

#### Requisitos do sistema
* [Docker instalado em sua maquina](https://balta.io/blog/docker-instalacao-configuracao-e-primeiros-passos)
* [SQL Server no Docker](https://balta.io/blog/sql-server-docker)
* [.NET na versão 6](https://dotnet.microsoft.com/en-us/download/dotnet/6.0)

---

### Instalação de dependências do projeto
**Microsoft Entity Framework Core**: Para instalar execute os dois comandos listados abaixo.

    dotnet add package Microsoft.EntityFrameworkCore.SqlServer

    dotnet add package Microsoft.EntityFrameworkCore.Design

    dotnet tool install --global dotnet-ef
---
### Rotas disponíveis na API

| Método | Recurso | Descrição |
|--|--|--|
| `POST` | v1/accounts/ | Cadastro de novo usuário |
| `POST` |  v1/accounts/login |  Login do usuário
| `POST` |  v1/accounts/upload-image | Adicionar uma imagem ao perfil de usuário
| `GET` |  v1/categories | Listar todas as categorias de posts
| `GET` |  v1/categories/{id:int} | Listar uma categoria de post 
| `POST` |  v1/categories | Cadastrar nova categoria de post
| `PUT` |  v1/categories/{id:int} |  Editar categoria de post
| `DELETE` |  v1/categories/{id:int} | Excluir uma categoria de post
| `GET` |  v1/posts |  Listar todos os posts
| `GET` |  v1/posts/{id:int} | Listar um post
| `GET` |  v1/posts/category/{category} | Listar os posts de determinada categoria
