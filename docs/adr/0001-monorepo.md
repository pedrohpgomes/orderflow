# ADR 0001 - Monorepo

## Status

Accepted

## Context

O projeto OrderFlow será composto por múltiplos microsserviços
(Order API, Inventory Service e Payment Service),
além de componentes de infraestrutura compartilhados
(PostgreSQL, RabbitMQ, Redis, Prometheus e Grafana).

Precisamos decidir entre utilizar um monorepo
ou múltiplos repositórios.

## Decision

Optamos por um monorepo.

## Consequences

### Positivas

- Configuração simplificada.
- Um único docker-compose.
- Facilita o aprendizado.
- Facilita a demonstração em entrevistas.

### Negativas

- Em equipes muito grandes pode dificultar o versionamento independente.