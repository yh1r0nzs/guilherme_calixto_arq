# REVIEW — Estado do Projeto & Próximas Ações
> **Data:** 2026-09-28  
> **Repositório:** [yh1r0nzs/guilherme_calixto_arq](https://github.com/yh1r0nzs/guilherme_calixto_arq)  
> **Status Geral:** ✅ **Planejamento Concluído | ⏳ Aguardando Cliente (F0)**

---

## 1. Resumo Executivo

### O que foi entregue ✅

| Entregável | Status | Local |
|------------|--------|-------|
| Análise do briefing & referência | ✓ | PLANNING.md §1–2 |
| Plano de projeto completo (7 fases) | ✓ | PLANNING.md §9 |
| Questionário para o cliente (35 perguntas) | ✓ | PERGUNTAS-CLIENTE.md |
| Modelo de conteúdo (MDX) | ✓ | PLANNING.md §6 |
| Stack técnico definido | ✓ | PLANNING.md §8 |
| Documentação de guardrails & contexto | ✓ | AI-GUARDRAIL.md, CONTEXT.md |
| Repositório GitHub público | ✓ | github.com/yh1r0nzs/guilherme_calixto_arq |

**Resultado:** Projeto bem estruturado, documentado e pronto para avançar assim que o cliente responder.

---

## 2. Status Atual da Fase F0 (Descoberta)

### ✅ Completo
- [x] Briefing analisado e entendido
- [x] Referência (arquitetojoaogabriel.com) estudada
- [x] Planejamento detalhado criado
- [x] Questionário estruturado para cliente
- [x] Documentação de projeto criada
- [x] Repositório GitHub criado e populado

### ⏳ Bloqueado (aguardando cliente)
- [ ] **Respostas às perguntas** (★ = críticas)
  - A1: O que agradou na referência?
  - B2: Como assinar o site? (nome/logo)
  - C1: Frase de posicionamento?
  - D1: Quais projetos na v1?
  - D2: Detalhes de cada projeto (tipo, ano, conceito, renders)?
  - D5: Autorização para publicar imagens?
  - E1: Onde colocar artigos (página ou destaque)?
  - E2: Quantos artigos prontos?
  - E4: Quer publicar sozinho?
  - F1: **CTA principal** (WhatsApp / formulário / artigos)?
  - G1: Domínio já registrado?
  
- [ ] **Materiais de conteúdo**
  - Renders (alta resolução, mín. 1920px)
  - Plantas baixas / esquemas / diagramas
  - Textos de conceito (ou tópicos para redação)
  - Foto profissional

- [ ] **Confirmações administrativas**
  - Status do domínio `guilhermecalixtoarq.com.br`
  - Autorização para publicar projetos de clientes
  - Definição do público prioritário (profissionais vs. clientes finais)

---

## 3. Checklist de Tarefas Sequenciais

### **Fase Atual: Comunicação com Cliente**

```
[ ] Task 1: Preparar e enviar o questionário
    ├─ [ ] Formatar PERGUNTAS-CLIENTE.md em PDF
    ├─ [ ] Escrever e-mail de acompanhamento explicando o projeto
    ├─ [ ] Enviar para: cgarquitetura27@gmail.com
    ├─ [ ] Prazo sugerido: 5–7 dias para resposta
    └─ [ ] Registrar data de envio em CONTEXT.md

[ ] Task 2: Receber materiais da v1
    ├─ [ ] Criar Google Drive compartilhado (ou WeTransfer)
    ├─ [ ] Solicitar renders em alta resolução (.jpg/.png, mín. 1920px)
    ├─ [ ] Solicitar plantas e esquemas (.pdf/.png)
    ├─ [ ] Solicitar textos de conceito (ou tópicos)
    ├─ [ ] Solicitar foto profissional
    └─ [ ] Organizar em pasta `/content/projetos/` do repositório

[ ] Task 3: Confirmar pré-requisitos técnicos
    ├─ [ ] Verificar se domínio foi registrado no Registro.br
    ├─ [ ] Confirmar posse (CPF do cliente)
    ├─ [ ] Se não registrado: orientar processo no Registro.br
    └─ [ ] Documentar em PLANNING.md §1 (Resumo do projeto)

[ ] Task 4: Make go/no-go decision
    ├─ [ ] Todas as respostas ★ recebidas?
    ├─ [ ] Materiais da v1 na pasta?
    ├─ [ ] Domínio confirmado?
    └─ [ ] SE sim → avançar para F1 (Identidade)
          SE não → fazer follow-up focado nas críticas
```

---

### **Próxima Fase: F1 (Identidade Visual)** — depende de respostas

```
Será acionada QUANDO:
✓ Respostas ao questionário recebidas
✓ Materiais de conteúdo organizados
✓ Domínio confirmado

O que será feito:
□ Definir tipografia (display + corpo)
□ Refinar paleta de cores
□ Criar wireframes (Home, Projeto, Artigo)
□ Entregar para aprovação do cliente

Duração estimada: 3–5 dias úteis
```

---

### **Fase F3 (Setup Técnico)** — depende de F1 aprovada

```
O que será feito:
□ Criar projeto Next.js (App Router + TypeScript)
□ Adicionar Tailwind CSS
□ Estruturar pastas (app/, components/, content/, lib/)
□ Deploy na Vercel (preview URL)
□ Configurar variáveis de ambiente

Duração estimada: 2–3 dias úteis
Entregável: URL de preview (ex.: main.guilherme-site.vercel.app)
```

---

## 4. Decisões Críticas em Aberto

| # | Decisão | Impacto | Quem | Status |
|---|---------|--------|------|--------|
| **D-01** | O que agradou na referência? | Direção visual | Cliente (A1) | ⏳ Aguardando |
| **D-02** | Cores de destaque? | Design | Cliente (A4, A5) | ⏳ Aguardando |
| **D-03** | Redesign de logo? | Escopo + orçamento | Cliente (B1) | ⏳ Aguardando |
| **D-04** | Assinatura do site? | Branding | Cliente (B2) | ⏳ Aguardando |
| **D-05** | Quais projetos na v1? | Conteúdo | Cliente (D1) | ⏳ Aguardando |
| **D-06** | Artigos: página ou destaque? | Navegação | Cliente (E1) | ⏳ Aguardando |
| **D-07** | CTA principal? | Conversão | Cliente (F1) | ⏳ Aguardando |
| **D-08** | Domínio registrado? | Lançamento | Cliente (G1) | ⏳ Aguardando |
| **D-09** | CSS: Tailwind ou Modules? | Dev speed | Interno | **✓ Tailwind** |
| **D-10** | Analytics + LGPD? | Conformidade | Cliente (G4) | ⏳ Aguardando |

---

## 5. Riscos Monitorados

| Risco | Probabilidade | Impacto | Mitigação | Status |
|-------|---------------|--------|-----------|--------|
| Cliente não responde | Média | Alto | Follow-up em 1 semana; oferecer chamada | 🟡 Monitorar |
| Poucos projetos na v1 | Média | Médio | Páginas ricas + plantas | 🟢 Planejado |
| Renders muito pesados | Média | Médio | `next/image` + compressão | 🟢 Planejado |
| Domínio indisponível | Baixa | Alto | Ter alternativas prontas | 🟡 Verificar |
| Sem autorização para publicar | Baixa | Alto | Confirmar D5 | 🟢 Planejado |

---

## 6. Recomendações Imediatas

### 🎯 Esta semana (até 2026-10-04)

1. **Enviar o questionário ao cliente**
   ```
   Para: cgarquitetura27@gmail.com
   CC: —
   Assunto: Seu site de portfólio — Questionário para começar
   
   Mensagem:
   "Oi Guilherme,
   
   Para montar o seu site do jeito certo, criei um questionário com 35 perguntas.
   As marcadas com ★ são as mais importantes.
   
   Pode responder por texto, áudio ou vídeo — como for mais confortável.
   Se não souber alguma coisa, é só dizer e decidimos junto.
   
   Arquivo em anexo: PERGUNTAS-CLIENTE.md
   Repositório do projeto: https://github.com/yh1r0nzs/guilherme_calixto_arq
   
   Prazo sugerido: Uma semana (até XX de outubro).
   Próximo passo: Assim que receber as respostas, faço a primeira proposta visual.
   
   Abraços,
   Arthur"
   ```

2. **Criar Google Drive para materiais** (compartilhado com cliente)
   - Pasta: "Guilherme Calixto Arq — Materiais v1"
   - Subpastas: Renders | Plantas | Textos | Foto

3. **Registrar data de envio em CONTEXT.md**
   ```markdown
   ### Data de envio do questionário
   - **Enviado em:** 2026-09-28
   - **Para:** cgarquitetura27@gmail.com
   - **Prazo esperado de resposta:** 2026-10-05
   - **Responsável:** Arthur
   ```

### 📅 Próximas 2 semanas

4. **Preparar o repositório Next.js** (em paralelo, sem bloquear cliente)
   - Criar branch `setup/next-js`
   - Executar: `npx create-next-app@latest`
   - Estruturar pastas conforme PLANNING.md §8
   - Não fazer commit para `main` até F1 aprovada

5. **Fazer follow-up se não houver resposta em 7 dias**
   - WhatsApp: "(32) 98454-2644"
   - Oferecer chamada de 30 min para responder ao vivo

---

## 7. Matriz de Comunicação

### Contato do cliente
| Canal | Valor | Status |
|-------|-------|--------|
| **E-mail** | cgarquitetura27@gmail.com | ✓ Primário para docs |
| **WhatsApp** | (32) 98454-2644 | ✓ Para follow-up |
| **GitHub** | @yh1r0nzs (Arthur) | ✓ Para atualizar |

### Frequência sugerida
- **Envio inicial:** Agora (2026-09-28)
- **Follow-up 1:** +7 dias (2026-10-05)
- **Follow-up 2:** +3 dias (2026-10-08)
- **Depois:** Semanal até conclusão

---

## 8. Artefatos Criados & Localização

### No repositório GitHub
```
yh1r0nzs/guilherme_calixto_arq/
├─ PLANNING.md              # Plano completo do projeto
├─ PERGUNTAS-CLIENTE.md     # Questionário (35 perguntas)
├─ CONTEXT.md               # Estado atual & decisões
├─ EXECUTION-LOG.md         # Histórico de trabalho
├─ briefing.md              # Dados do cliente & objetivos
├─ AI-GUARDRAIL.md          # Regras & guardrails do projeto
├─ PREFERENCES.md           # Preferências de cliente
└─ README.md (a criar)      # Instruções para começar
```

### Local (sincronizado com GitHub)
```
C:\Users\arthu\OneDrive\Documentos\CLIENTES\GUILHERME\
├─ [arquivos listados acima, sincronizados]
└─ .claude/worktrees/       # Exemplo de projeto anterior
```

---

## 9. Timeline Realista

| Fase | Duração | Início | Critério de conclusão |
|------|---------|--------|----------------------|
| **F0** | ~2 sem. | 2026-09-28 | Respostas + materiais recebidos |
| **F1** | 3–5 dias | Após F0 | Wireframes aprovados |
| **F2** | Incluído em F1 | — | — |
| **F3** | 2–3 dias | Após F1 | Preview no ar |
| **F4** | 5–7 dias | Após F3 | Páginas funcionais |
| **F5** | Variável | Paralelo | Conteúdo real |
| **F6** | 2 dias | Após F5 | Testes passando |
| **F7** | 1 dia | Final | Lançamento |
| **TOTAL** | **4–5 semanas** | 2026-09-28 | MVP em produção |

---

## 10. Próximo Encontro/Review

**Recomendação:** Agendar review após receber respostas do cliente (aprox. 2026-10-05).

**Agenda:**
- [ ] Análise das respostas
- [ ] Atualizar PLANNING.md com decisões (D-01 a D-10)
- [ ] Validar modelo de conteúdo vs. materiais recebidos
- [ ] Kickoff de F1 (Identidade)
- [ ] Definir ferramentas de design (Figma vs. protótipo HTML)

---

## 11. Checklist Final (Esta sessão)

- [x] Repositório GitHub criado e público
- [x] Documentação completa versionada
- [x] Planejamento detalhado (7 fases)
- [x] Questionário estruturado para cliente
- [x] Riscos identificados e mitigados
- [x] Timeline realista estimada
- [x] Próximos passos claros
- [ ] **Enviar questionário ao cliente** ← AÇÃO IMEDIATA
- [ ] **Criar Google Drive de materiais** ← AÇÃO IMEDIATA
- [ ] **Registrar data de envio em CONTEXT.md** ← AÇÃO IMEDIATA

---

**Status de conclusão desta etapa:** ✅ **100%**  
**Bloqueador para avançar:** ⏳ Respostas do cliente + materiais

**Próximo passo:** Enviar PERGUNTAS-CLIENTE.md ao Guilherme com mensagem de acompanhamento.

