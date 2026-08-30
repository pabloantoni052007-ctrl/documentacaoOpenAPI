# Documentação OpenAPI - Sistema de Controle de Estoque de Pastilhas Industriais

Este repositório contém a documentação da API desenvolvida para o Projeto Integrador do SENAI/SC - Florianópolis.

O projeto tem como tema o desenvolvimento de um sistema para controle de estoque de pastilhas industriais utilizado pela DDA Usinagem Industrial Ltda.

## Objetivo do projeto

A proposta do sistema é substituir o controle manual realizado por planilhas por uma solução capaz de gerenciar o estoque de pastilhas industriais de forma mais segura, organizada e eficiente.

A aplicação deverá permitir o acompanhamento das quantidades disponíveis em estoque, registrar entradas e saídas de materiais, controlar níveis mínimos e disponibilizar informações para apoiar o planejamento de compras e evitar interrupções na produção.

## Objetivo da documentação

Esta documentação foi desenvolvida utilizando a especificação OpenAPI, seguindo a abordagem API First.

O objetivo é definir previamente o contrato da API que posteriormente será implementada utilizando Spring Boot.

O arquivo principal da documentação é:

`openapi.yaml`

## Funcionalidades previstas

A API contempla funcionalidades relacionadas a:

- Autenticação de usuários;
- Cadastro e gerenciamento de usuários;
- Cadastro de pastilhas industriais;
- Cadastro de fabricantes;
- Cadastro de fornecedores;
- Registro de entradas de estoque;
- Registro de saídas de estoque;
- Consulta das quantidades disponíveis;
- Histórico de movimentações;
- Controle de estoque mínimo;
- Alertas de estoque crítico;
- Consulta de indicadores e resumo do estoque.

## Principais recursos da API

### Autenticação

Responsável pelo acesso dos usuários ao sistema.

Exemplo:

`POST /auth/login`

### Usuários

Gerenciamento dos usuários que terão acesso ao sistema.

Exemplos:

`GET /usuarios`

`POST /usuarios`

`GET /usuarios/{id}`

`PUT /usuarios/{id}`

`DELETE /usuarios/{id}`

### Pastilhas

Gerenciamento dos diferentes modelos de pastilhas industriais.

Exemplos:

`GET /pastilhas`

`POST /pastilhas`

`GET /pastilhas/{id}`

`PUT /pastilhas/{id}`

`DELETE /pastilhas/{id}`

### Fabricantes

Gerenciamento dos fabricantes das pastilhas industriais.

### Fornecedores

Gerenciamento dos fornecedores responsáveis pelo fornecimento dos materiais.

### Movimentações

Responsável pelo registro das entradas e saídas do estoque.

Exemplos:

`GET /movimentacoes`

`POST /movimentacoes`

### Estoque

Permite consultar a situação atual dos materiais.

Exemplos:

`GET /estoque`

`GET /estoque/alertas`

`GET /estoque/resumo`

## Tecnologias e padrões utilizados

A documentação foi desenvolvida utilizando:

- OpenAPI 3.0.3;
- YAML;
- API REST;
- JSON;
- Métodos HTTP;
- Autenticação Bearer Token / JWT.

A API será posteriormente implementada utilizando:

- Java;
- Spring Boot.

## Métodos HTTP utilizados

| Método | Utilização |
|---|---|
| GET | Consulta de informações |
| POST | Cadastro ou registro de informações |
| PUT | Atualização de registros |
| DELETE | Exclusão de registros |

## Códigos HTTP utilizados

| Código | Significado |
|---|---|
| 200 | Operação realizada com sucesso |
| 201 | Recurso criado com sucesso |
| 204 | Operação realizada sem conteúdo de retorno |
| 400 | Requisição inválida |
| 401 | Usuário não autenticado |
| 404 | Recurso não encontrado |
| 409 | Conflito com informações existentes |
| 422 | Regra de negócio não atendida |

## Como visualizar a documentação

A documentação pode ser visualizada através do Swagger Editor.

1. Acesse o Swagger Editor;
2. Abra o arquivo `openapi.yaml`;
3. Copie o conteúdo do arquivo;
4. Cole no editor;
5. A documentação será gerada automaticamente.

Swagger Editor:

https://editor.swagger.io/

## Estrutura do repositório

documentacaoOpenAPI/
├── openapi.yaml
└── README.md

## Projeto Integrador

**Projeto:** Sistema para Controle de Estoque de Pastilhas Industriais

**Empresa:** DDA Usinagem Industrial Ltda.

**Instituição:** SENAI/SC - Florianópolis

**Área:** Tecnologia da Informação

## Autor

Pablo

Projeto acadêmico desenvolvido para o Projeto Integrador do SENAI/SC.