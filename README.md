# Projeto Django API
Este projeto implementa uma API RESTful utilizando Django e Django REST Framework para gerenciar usuários.

### A API possui as seguintes funcionalidades principais:

### Obter Usuários
- Endpoint: /get_users/
- Método: GET
  ### Descrição:
  - Retorna uma lista de todos os usuários registrados no banco de dados.
### Obter e Atualizar Usuário por Nickname
- Endpoint: /get_by_nick/<nick>/
- Métodos: GET, PUT
  ### Descrição:
  - GET: Retorna os dados de um usuário específico, identificado pelo nickname.
  - PUT: Atualiza os dados de um usuário específico, identificado pelo nickname.
  
### Gerenciar Usuário (CRUD)

- Endpoint: /user_manager/
- Métodos: GET, POST, PUT, DELETE
  ### Descrição:
  - GET: Retorna os dados de um usuário específico com base no parâmetro user fornecido na URL.
  - POST: Cria um novo usuário com base nos dados fornecidos no corpo da requisição.
  - PUT: Atualiza os dados de um usuário específico com base nos dados fornecidos no corpo da requisição.
  - DELETE: Deleta um usuário específico com base no user_nickname fornecido no corpo da requisição.
    
### Estrutura do Projeto

O projeto é composto pelos seguintes arquivos e diretórios principais:

- views.py: Contém as funções de view para lidar com as requisições HTTP e interações com os modelos de dados.
- models.py: Define os modelos de dados utilizados no projeto.
- serializers.py: Define os serializers usados para converter os objetos do modelo em JSON e vice-versa.

### Dependências
- Django
- Django REST Framework
