# AtividadeWEb2-3pN
API RESTful desenvolvida com Node.js e Express para gerenciar tarefas. Suporte a CRUD completo, validações com Joi, filtros, banco de dados em memória, tratamento de erros e logs. Projeto acadêmico com testes via Postman.

API RESTful - Gerenciador de Tarefas
Este projeto é uma API RESTful criada com Node.js e Express para o gerenciamento de tarefas. Desenvolvido como parte da Atividade Prática Avançada II do curso de Desenvolvimento Web.

Funcionalidades
Criar, listar, atualizar e deletar tarefas

Marcar tarefa como concluída

Filtros por query e path parameters

Validação de dados com Joi

Banco de dados simulado em memória (fakeDb.js)

Estrutura em camadas: Controller, Service, Middleware, etc.

Logs de ações importantes no sistema

Tratamento de erros com mensagens padronizadas

Tecnologias utilizadas
Node.js

Express

Joi

UUID

Morgan (opcional)

Instalação
Clone este repositório:

bash
Copiar
Editar
git clone https://github.com/seu-usuario/seu-repositorio.git
Acesse a pasta do projeto:

bash
Copiar
Editar
cd api-tarefas
Instale as dependências:

nginx
Copiar
Editar
npm install
Inicie a aplicação:

bash
Copiar
Editar
node src/app.js
Endpoints disponíveis

Método	Rota	Descrição
GET	/tarefas	Lista todas as tarefas
GET	/tarefas?concluida=true	Lista apenas as tarefas concluídas
GET	/tarefas/:id	Busca uma tarefa pelo ID
POST	/tarefas	Cria uma nova tarefa
PUT	/tarefas/:id	Atualiza todos os campos da tarefa
PATCH	/tarefas/:id/concluir	Marca uma tarefa como concluída
DELETE	/tarefas/:id	Deleta uma tarefa
Testes
Os testes foram realizados com o Postman. Para cada rota:

Envie os dados obrigatórios no corpo (JSON)

Verifique os status de resposta (200, 201, 204, 400, 404)

Teste com dados inválidos para verificar as validações

Estrutura de Pastas
