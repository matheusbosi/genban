# Requirements

[MVP](#mvp)  
[NICE TO HAVE](#nice-to-have)  
[MOLDE BANCO DE DADOS](#modelo-banco)  
[FOOTNOTES](#footnotes)

---

## MVP

- Usuario pode
  - cadastro
  - fazer login
  - criar projeto
- Projeto
  - pode ter varios usuarios
  - projeto vai ser composto por listas
  - fazer pesquisa
- Lista
  - composto por cards
- Cards
  - descrição
  - anexar arquivos
  - usuarios podem comentar
  - mencionar outros usuarios

---

## Nice to have

- projeto
  - personalizar fundo
  - notificação
- card
  - ter data
  - label
  - associar com usuario
  - ter automatização
  - formatar markdown
  - ter um TODO
- usuario
  - recuperar senha
  - marcar outros usuarios em comentarios

---

## Modelo banco

- users
  - name
  - email
  - password
- projects
  - name
  - created_by
- projects_users
  - project_id
  - user_id
  - role
- lists ? [^1]
- cards
  - project_id
  - name
  - description
  - files_url
  - active
- comments
  - user_id
  - card_id
  - comment

---

## FOOTNOTES

[^1]: Não sei se é uma boa gerenciar o estado da lista pelo banco de dados.
