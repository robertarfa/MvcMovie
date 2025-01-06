# MvcMovie

## Descrição
MvcMovie é um projeto Blazor que permite gerenciar uma lista de filmes. Ele inclui funcionalidades para listar, criar, editar e excluir filmes.

## Tecnologias Utilizadas
- Blazor
- .NET 8
- Entity Framework Core
- SQL Server

## Instalação
1. Clone o repositório:

   git clone https://github.com/robertarfa/mvcmovie.git

2. Navegue até o diretório do projeto:

   cd mvcmovie

3. Restaure as dependências:

   dotnet restore


## Configuração do Banco de Dados
1. Configure a string de conexão no arquivo `appsettings.json`.
2. Aplique as migrações do Entity Framework:
   
    dotnet ef database update
   

## Estrutura do Projeto
- `Controllers/MoviesController.cs`: Controlador responsável pelas operações CRUD dos filmes.
- `Models/Movie.cs`: Modelo que representa um filme.
- `Data/MvcMovieContext.cs`: Contexto do Entity Framework Core.

## Funcionalidades Principais
- Listar filmes
- Filtrar filmes por gênero e título
- Criar, editar e excluir filmes

## MoviesController.cs
O arquivo `MoviesController.cs` é um controlador que gerencia as operações CRUD (Create, Read, Update, Delete) para os filmes no projeto. Ele utiliza o Entity Framework Core para interagir com o banco de dados e fornece métodos para:

- **Listar Filmes**: O método `Index` permite listar todos os filmes, com a opção de filtrar por gênero e título.
- **Detalhes do Filme**: O método `Details` exibe os detalhes de um filme específico.
- **Criar Filme**: Os métodos `Create` (GET e POST) permitem adicionar um novo filme ao banco de dados.
- **Editar Filme**: Os métodos `Edit` (GET e POST) permitem editar as informações de um filme existente.
- **Excluir Filme**: Os métodos `Delete` (GET e POST) permitem excluir um filme do banco de dados.

### Exemplo de Uso
- **Listar Filmes**: Acesse a URL `/Movies` para ver a lista de filmes.
- **Filtrar Filmes**: Use os campos de busca e filtro na página de listagem de filmes para encontrar filmes específicos.
- **Adicionar Filme**: Acesse a URL `/Movies/Create` para adicionar um novo filme.
- **Editar Filme**: Acesse a URL `/Movies/Edit/{id}` para editar um filme existente.
- **Excluir Filme**: Acesse a URL `/Movies/Delete/{id}` para excluir um filme.
   
   
