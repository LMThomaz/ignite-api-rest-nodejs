# Rest API

## Variáveis de ambientes

- DATABASE_URL - URL do banco de dados

## Comandos Knex

- Criar uma migration
  Note que o nome da migration é relacionado ao o que ela irá realizar, neste caso ela irá adicionar um campo chamado _session-id_ na tabela _transactions_

```bash
npm run knex -- migrate:make add-session-id-to-transactions
```

- Executar as migrations

```bash
npm run knex -- migrate:latest
```

- Voltar a execução da migrations

```bash
npm run knex -- migrate:rollback
```
