# Abadon

> Portfólio público de um projeto com código-fonte privado.

**Abadon** é uma base de conhecimento própria criada para substituir uma estrutura de notas isoladas por um sistema com **RAG, busca semântica, memória, biblioteca de documentos e grafo de conceitos**.

O projeto combina engenharia de dados, segurança de acesso, recuperação semântica e interface própria para transformar conhecimento disperso em contexto utilizável por uma IA.

## Problema

Bases de conhecimento pessoais normalmente têm três limitações:

- armazenam conteúdo, mas não recuperam contexto de forma inteligente;
- não separam corretamente informação compartilhada de informação privada;
- dificultam visualizar relações entre documentos, conceitos e conversas.

## Solução

O Abadon reúne:

- biblioteca de documentos;
- controle de versões;
- conceitos e relações;
- grafo visual;
- autenticação;
- conversas privadas por usuário;
- RAG semântico;
- embeddings;
- fila de processamento;
- memória contextual;
- interface web própria.

## Arquitetura

A base usa **Supabase/PostgreSQL** como núcleo de dados, com **pgvector** para armazenamento vetorial.

A segurança é feita com **Row Level Security**, separando:

- conteúdo compartilhado;
- dados privados por usuário;
- autoria e permissões de edição.

O pipeline de RAG:

1. recebe a pergunta;
2. gera embedding;
3. busca chunks semanticamente relevantes;
4. monta o contexto;
5. envia o contexto ao modelo;
6. persiste a resposta e o histórico.

## Dados processados

Na implantação inicial, o importador idempotente carregou:

- 98 documentos;
- 19 conceitos;
- 455 relações.

## Stack

- PostgreSQL
- Supabase
- pgvector
- JavaScript
- RAG
- embeddings
- Cloudflare Workers
- Cloudflare Workers AI
- bge-m3
- Row Level Security

## Diferenciais técnicos

- importação idempotente;
- migrations versionadas;
- RLS para isolamento de dados;
- grafo de conceitos em canvas;
- recuperação semântica;
- fila de jobs;
- arquitetura separando dados, recuperação e interface.

## Código-fonte

O código não está disponível publicamente porque o projeto trabalha com uma base de conhecimento privada, documentos pessoais, regras de acesso e integrações sensíveis.

O objetivo deste case é demonstrar a arquitetura e as decisões técnicas sem expor conteúdo, credenciais ou informações privadas.
