# 🏋️ Exercícios de Preparação para Prova Django

## Task 1: MTV Básico (Livros) 📚
### Model
#### Livro:

| Campo | Tipo | 
| -------- | ----- | 
|titulo | CharField -> max_length=50 |
|autor  | CharField -> max_length=30 |
|paginas  | IntegerField |

### Tarefas
- Criar view listar_livros que renderiza template
- Template livros.html mostrando lista em <ul>
- URL /livros/ mapeada para a view
- Registrar model no admin

## Task 2: API Simples (@api_view) 🖥️
### Model (mesmo Livro da Task 1)
#### Endpoints
- GET /api/livros/ - Lista todos (JSON)
- POST /api/livros/ - Adiciona novo livro

#### Requisitos
- Usar @api_view(['GET', 'POST'])
- Serializer básico
- Retornar status codes apropriados

## Task 3: Autenticação Básica (JWT) 🔑
### Custom User - Campos adicionais

| Campo | Tipo | 
| -------- | ----- | 
|telefone  | CharField -> max_length=15 |

### Endpoints
- POST /auth/registro/ - Cria usuário
- POST /auth/login/ - Retorna tokens JWT