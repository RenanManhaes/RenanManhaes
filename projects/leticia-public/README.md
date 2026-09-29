# Leticia

> Portfólio público de um projeto com código-fonte privado.

**Leticia** é uma assistente pessoal em aplicativo desktop, criada para ir além de um chatbot e funcionar como uma interface contínua de apoio, voz, contexto, tarefas e execução auditável.

## Objetivo

Criar uma assistente que consiga manter contexto real do usuário, armazenar dados localmente, trabalhar com voz e evoluir para execução controlada de ações no computador.

## Funcionalidades implementadas

- interface desktop em Electron;
- orbe/HUD com estados visuais;
- entrada por voz;
- transcrição de fala;
- síntese de voz;
- conversa por texto;
- persistência local;
- gestão de projetos e tarefas;
- preferências persistidas;
- métricas do sistema;
- histórico auditável de ações;
- anexos em tarefas;
- backups automáticos.

## Arquitetura

O projeto usa **Electron + TypeScript** com persistência local em **SQLite**.

A aplicação foi desenhada com atenção especial a segurança de desktop:

- sandbox;
- Content Security Policy;
- IPC restrito;
- instância única;
- proteção de chave de API usando criptografia do sistema operacional.

## Stack

- Electron
- TypeScript
- React
- SQLite
- Vitest
- Playwright
- STT
- TTS

## Qualidade

O projeto inclui:

- testes unitários;
- validação de entrada;
- smoke test end-to-end do aplicativo empacotado;
- documentação de arquitetura;
- ADRs para decisões técnicas;
- separação explícita entre recursos implementados e planejados.

## Visão de produto

A arquitetura foi pensada para evoluir por domínios:

- identidade e memória;
- contexto;
- planejamento;
- execução;
- integrações;
- permissões;
- observabilidade;
- personalidade e experiência.

## Código-fonte

O código-fonte permanece privado porque o projeto é um assistente pessoal, com integrações locais, configurações específicas do usuário e dados que não devem ser publicados.

Este case apresenta somente a arquitetura e as capacidades que podem ser compartilhadas com segurança.
