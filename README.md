# Rest API

# RF (Requisitos funcionais)

- [x] O usuário deve poder criar uma nova transação;
- [x] O usuário deve poder obter um resumo da sua conta;
- [x] O usuário deve poder listar todas transações que já ocorreram;
- [x] O usuário deve poder visualizar uma transação única;

# RN (Regras de Negócios)

- [x] A transação pode ser fo tipo crédito que somará ao valor total, ou débito subtrairá;
- [ ] Deve ser possível identificarmos o usuário entre as requisições;
- [ ] O usuário só pode visualizar transações o qual ele criou;

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
