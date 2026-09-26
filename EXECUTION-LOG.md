# EXECUTION LOG

> Formato definido em `AI-GUARDRAIL.md` §18.

---

## 2026-09-24 — Planejamento — v1

**IA/Agente:** Claude (Claude Code)  
**Modelo:** Opus 5.5 (`claude-opus-5-5`)  
**Etapa executada:** Planejamento inicial + questionário do cliente

**Arquivos alterados:**

- `PLANNING.md` (criado o conteúdo)
- `PERGUNTAS-CLIENTE.md` (novo)
- `CONTEXT.md` (criado o conteúdo)
- `EXECUTION-LOG.md` (primeira entrada)

**O que foi feito:**

- Lidos todos os `.md` do projeto. O `readme.md` dentro de `.claude/worktrees` é de outro projeto e foi ignorado.
- Analisado o site de referência arquitetojoaogabriel.com (Home e página de projeto "Casa de Gal").
- Montado o planejamento completo e o questionário para o cliente.

**Data/hora:** 2026-09-24

### Decisão relacionada

- Stack Next.js definida pelo responsável; perguntas em arquivo separado.

### Validação

- Cada pendência do `briefing.md` §5 tem uma pergunta correspondente (A1, B1, E1, D2, F1, G1).
- Cada decisão em aberto do `PLANNING.md` §11 aponta para um ID de pergunta.
- Os itens não confirmados estão marcados como **[A CONFIRMAR]**.

### Pendências

- Respostas do cliente (fase F0).

---

## 2026-09-26 — Registro de respostas do cliente (projeto de extensão)

**IA/Agente:** Claude (Claude Code)  
**Modelo:** Opus 5.5 (`claude-opus-5-5`)  
**Etapa executada:** F0 — Descoberta (respostas parciais)

**Arquivos alterados:**

- `RESPOSTAS-CLIENTE.md` (novo)
- `PLANNING.md`
- `CONTEXT.md`
- `EXECUTION-LOG.md`

**O que foi feito:**

- Transcritas as respostas do Guilherme (WhatsApp, 2026-09-26): UNIFACIG, orientação de Lidiane Espindula, 1 casa, nenhum material ainda, famílias autorizaram.
- Incluída no `PLANNING.md` a §5.1 com o que se sabe do projeto de extensão, as decisões D-12 e D-13 e dois riscos novos.

**Data/hora:** 2026-09-26

### Decisão relacionada

- Projeto de extensão só entra na v1 com material real (regra de não usar placeholder, `AI-GUARDRAIL.md` §6).

### Validação

- Nada foi inventado: o nome do projeto de extensão, que não veio na resposta, ficou como **[A CONFIRMAR]**.
- Nenhum item de escopo foi adicionado; o bloco antes/depois ficou como decisão em aberto (D-13).

### Pendências

- Nome do projeto de extensão, grafia do nome de quem orienta, situação da casa, autorização por escrito e material.
