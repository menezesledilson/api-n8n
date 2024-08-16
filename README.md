# API de Tarefas com Integração Slack

Este projeto é uma API simples para gerenciar tarefas com dois endpoints: um para listar tarefas (`GET`) e outro para criar novas tarefas (`POST`). Cada nova tarefa criada gera um alerta em um canal do Slack utilizando o N8N para enviar mensagens personalizadas. Os dados das tarefas são armazenados em um banco de dados PostgreSQL.

## Tecnologias Utilizadas

- **Backend:**
  - Java
  - Spring Boot
  - Spring Web
  - Lombok
  - PostgreSQL
  - JPA

- **Integração e Automação:**
  - [N8N](https://n8n.io)
    - Webhook:Configurado para receber notificações de novas tarefas.
    - Nó HTTP Request:Utilizado para enviar mensagens personalizadas para o Slack.

## Executando o N8N Localmente

Para rodar o N8N localmente, utilize o comando:
http://localhost:5678/signin
```bash
n8n start
