# Testes automatizados

## Tipos de testes

- Unitários: unidade da sua aplicação
- Integração: comunicação entre duas ou mais unidades
- e2e - ponta a ponta: simulam um usuário operando na nossa aplicação
  - front-end: abre a página de login, digite o texto exemple@tests.com no campo com ID email, clique no botão
  - back-end: chamadas HTTP, WebSockets

## Pirâmide de testes: E2E (não dependem de nenhuma tecnologia, não dependem de arquitetura)

- 2000 testes -> Testes E2E => 16min, são os testes mais pesados, por isso o projeto existe vários testes Unitários e de Integração, sendo eles a base da pirâmide e os testes e2e são a ponta desta pirâmide.
