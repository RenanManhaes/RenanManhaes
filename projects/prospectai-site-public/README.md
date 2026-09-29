# ProspectAI

> Portfólio público de um projeto com código-fonte privado.

A **ProspectAI** é uma plataforma SaaS de prospecção B2B criada para organizar campanhas de outreach, personalização de mensagens, acompanhamento de leads e handoff comercial em um único fluxo.

O objetivo do projeto é transformar uma operação de prospecção que normalmente fica espalhada entre planilhas, CRM, mensagens e tarefas manuais em um sistema rastreável e orientado a processo.

## Problema

Operações comerciais de prospecção costumam sofrer com:

- informações fragmentadas entre ferramentas;
- dificuldade para acompanhar o histórico de cada lead;
- falta de aprovação e governança sobre mensagens;
- processos manuais entre marketing, operação e vendas;
- pouca visibilidade do andamento das campanhas.

## Solução

A plataforma reúne em um único produto:

- autenticação e gestão de contas;
- portal do cliente;
- dashboard;
- campanhas;
- CRM de leads;
- histórico de conversas;
- aprovação de mensagens;
- painel administrativo;
- integrações preparadas para CRM externo;
- APIs internas e webhooks.

## Arquitetura

A aplicação foi estruturada em **Next.js com App Router**, usando **React e TypeScript** no frontend e **Supabase/PostgreSQL** como camada de dados e autenticação.

O isolamento entre clientes é feito com **Row Level Security (RLS)** diretamente no banco, evitando depender apenas de filtros da aplicação.

A arquitetura também separa:

- superfícies públicas;
- portal do cliente;
- área administrativa;
- rotas de API;
- integrações externas;
- migrações versionadas e rollbacks.

## Stack

- Next.js
- React
- TypeScript
- Supabase
- PostgreSQL
- Row Level Security
- Vercel
- Vitest
- Playwright
- GitHub Actions

## Qualidade e engenharia

O projeto possui verificações para:

- lint;
- type checking;
- testes unitários;
- testes de integração;
- testes end-to-end;
- validação de layout em diferentes larguras;
- proteção contra execução acidental de testes no banco de produção.

## Status

Em desenvolvimento ativo.

Demo pública: https://prospectai-brasil.vercel.app

## Código-fonte

O código-fonte principal **não é disponibilizado publicamente** porque o projeto contém arquitetura de produto, integrações, configurações operacionais e dados que não devem ser expostos.

Este repositório/case existe apenas para apresentar, de forma segura, o problema resolvido, a arquitetura e as decisões de engenharia do projeto.
