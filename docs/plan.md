# Plano Técnico (Plan) - TaskEasy

## 1. Stack Tecnológica

A stack tecnológica ainda não está especificada nos documentos do projeto TaskEasy. A linguagem, o framework, o banco de dados e a infraestrutura deverão ser definidos pela equipe antes da implementação. Não se considera Python, Flask ou Docker como decisões já tomadas.

## 2. Design Arquitetural

A solução deverá contemplar, no mínimo, os seguintes conceitos funcionais:

- **Usuário:** cadastro e autenticação por e-mail e senha.
- **Tarefa:** título obrigatório, descrição, data de vencimento opcional e situação (pendente ou concluída).
- **Associação:** cada tarefa deverá pertencer ao usuário que a cadastrou.
- **Operações:** criar, consultar, editar, excluir e concluir tarefas.
- **Consulta:** filtrar por situação, ordenar por vencimento e apresentar contadores.

A definição de classes, rotas, endpoints, banco de dados e infraestrutura permanece pendente de decisão técnica da equipe.
