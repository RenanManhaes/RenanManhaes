# Trader Harness

> Case público de um projeto experimental privado.

**Trader Harness** é um experimento de engenharia multiagente para estudar coordenação, risco, execução simulada, reconciliação e auditoria em operações de cripto Spot.

O projeto **não executa ordens reais** e foi desenhado para trabalhar exclusivamente com paper trading durante a fase experimental.

## Objetivo técnico

O foco do projeto não é prever mercado. O objetivo é estudar como agentes especializados podem colaborar dentro de uma arquitetura com:

- papéis bem definidos;
- autoridade limitada;
- contratos estruturados;
- validação independente;
- rastreabilidade;
- tratamento de falhas;
- gates de segurança.

## Arquitetura de agentes

O sistema separa responsabilidades entre agentes dedicados a:

- comando de sessão;
- validação de dados;
- estratégia;
- risco;
- execução simulada;
- reconciliação;
- incidentes;
- avaliação de performance.

Nenhum agente controla sozinho o ciclo completo.

## Conceitos de engenharia demonstrados

- arquitetura multiagente;
- segregação de responsabilidades;
- handoffs estruturados;
- schemas de comunicação;
- state machines;
- idempotência;
- reconciliação;
- rastreabilidade;
- fail-safe;
- experimentação controlada.

## Segurança

O projeto foi desenhado com limites explícitos:

- somente paper trading;
- sem alavancagem;
- sem futuros;
- sem saques;
- sem operação autônoma com dinheiro real;
- decisões de risco independentes da estratégia.

## Código-fonte

O repositório principal permanece privado porque o projeto ainda está em desenvolvimento experimental.

Este case existe para demonstrar a arquitetura e os princípios de engenharia, sem apresentar o projeto como sistema financeiro de produção.
