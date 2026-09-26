# PLANNING — Website & Portfólio Guilherme Calixto

> Fonte de verdade do projeto (ver `AI-GUARDRAIL.md` §13 e §15).
> Itens marcados **[A CONFIRMAR]** dependem de resposta do cliente e apontam para o ID da pergunta em `PERGUNTAS-CLIENTE.md`.
> Última atualização: 2026-09-26

---

## 1. Resumo do projeto

| Item | Definição |
| --- | --- |
| Cliente | Guilherme Calixto, arquiteto |
| Contato | cgarquitetura27@gmail.com · (32) 98454-2644 |
| Domínio pretendido | `guilhermecalixtoarq.com.br` (consulta/registro no Registro.br) **[A CONFIRMAR — G1]** |
| Prazo | Sem prazo definido no briefing |
| Problema | Ausência de visibilidade e de posicionamento digital |
| Objetivo | Ganhar visibilidade, reconhecimento e autoridade técnica/conceitual |
| Público | Estudantes de arquitetura, arquitetos, engenheiros e clientes finais de interiores |
| Tipo de solução | Portfólio digital híbrido: projetos + hub acadêmico (artigos/TCC) |
| Faculdade | UNIFACIG (resposta de 2026-09-26) |

**Dois públicos, duas intenções:**
- **Profissionais/estudantes** → querem ler, aprender, reconhecer autoridade (artigos, TCC, projetos acadêmicos).
- **Clientes finais de interiores** → querem ver projetos e entrar em contato.

A navegação e os CTAs precisam atender aos dois sem misturar as mensagens. A prioridade entre eles é a pergunta **F1**.

---

## 2. Análise da referência — arquitetojoaogabriel.com

### 2.1 O que foi observado

- **Plataforma:** Wix.
- **Tipografia:** títulos em caixa-alta, sem serifa geométrica e bold (Lulo Clean); apoio em Montserrat; corpo em Avenir Light. A marca é basicamente o nome em tipografia forte.
- **Estrutura da Home (ordem):**
  1. Nome em caixa-alta + tagline curta (“projetos | cursos | infoprodutos | publicidade”) + ícones sociais.
  2. Dois cards grandes com foto e CTA de serviço (“solicite uma proposta”).
  3. Linha de 5 cards pequenos de infoprodutos/mentoria (links de venda).
  4. Foto grande do arquiteto.
  5. “Destaques impressos” (mídia/publicações).
  6. “Sobre” com credenciais em negrito + retrato.
  7. “Time” do escritório.
  8. Grade de projetos (6 projetos).
  9. Contato: e-mail, WhatsApp, Instagram.
- **Página de projeto:** botão “voltar ao início”, título grande, subtítulo (ambientes + cidade), foto hero, faixa de miniaturas e texto narrativo curto (conceito → desafio técnico → materiais). A paleta da página acompanha o projeto.

### 2.2 Adotar / Adaptar / Não copiar

| Decisão | Elemento | Motivo |
| --- | --- | --- |
| **Adotar** | Nome em tipografia forte como marca | Alinhado ao briefing (§3: “tipografia minimalista para o nome”) |
| **Adotar** | Home em blocos modulares, grade de projetos, contato direto no rodapé | Pedido do briefing (§4) |
| **Adotar** | Página de projeto: hero + galeria + texto narrativo | Estrutura clara e já validada no mercado |
| **Adaptar** | Linha de “infoprodutos” → **destaques de artigos/TCC** | Guilherme não vende infoprodutos; o conteúdo dele é acadêmico **[A CONFIRMAR — E1, F2]** |
| **Adaptar** | Página de projeto → incluir **plantas/esquemas e ficha técnica** | Pedido do briefing (§5) e relevante para público técnico |
| **Adaptar** | Paleta: referência usa cinzas/cores por projeto → base P&B clean | Briefing pede clean/minimalista **[A CONFIRMAR — A4, A5]** |
| **Não copiar** | “Time” | O Guilherme não tem equipe (confirmado em 2026-09-26) |
| **Adaptar** | “Destaques impressos”, selos (Forbes, Casa Vogue) → “Destaques” | Só entra com material real **[A CONFIRMAR — C6]** |
| **Não copiar** | Blog | **A referência não tem blog.** O hub de artigos será desenho próprio |

> **Divergência com o briefing:** o briefing descreve a referência como tendo “blog/recursos técnicos”. Na verdade, a área de conteúdo dela é de infoprodutos (links de venda). A seção de artigos/TCC do Guilherme **não tem modelo direto na referência**.

---

## 3. Escopo

### 3.1 Dentro da v1 (MVP)
- Site institucional/portfólio responsivo em Next.js.
- Páginas: Home, Projetos (lista), Projeto (detalhe), Artigos (lista), Artigo (detalhe), Sobre, Contato *(mapa final pendente — ver §4)*.
- Poucos projetos na v1, misturando acadêmicos e de interiores (briefing §4) **[A CONFIRMAR — D1]**.
- Projeto de extensão da UNIFACIG (1 casa) como candidato a projeto da v1 — ver §5.1.
- Estrutura pronta para artigos e TCC, mesmo com pouco conteúdo no lançamento **[A CONFIRMAR — E2]**.
- CTA principal de contato **[A CONFIRMAR — F1]**.
- SEO básico, Open Graph, sitemap, performance e acessibilidade.
- Publicação na Vercel com domínio próprio.

### 3.2 Fora da v1 (proposta → aprovação antes de incluir)
- Redesign de marca/logo: **fora da v1** (decidido em 2026-09-26, B1).
- CMS para o cliente publicar sozinho **[A CONFIRMAR — E4]**.
- Versão em inglês **[A CONFIRMAR — H1]**.
- Depoimentos, newsletter, área de downloads pagos, infoprodutos **[A CONFIRMAR — H2, H3]**.
- E-mail profissional no domínio **[A CONFIRMAR — G2]**.

---

## 4. Mapa do site (proposta — pendente de validação)

```text
/                     Home
/projetos             Lista de projetos (filtro: Acadêmico | Interiores)
/projetos/[slug]      Detalhe do projeto
/artigos              Lista de artigos/TCC (filtro por tema)       [A CONFIRMAR — E1]
/artigos/[slug]       Detalhe do artigo
/sobre                Sobre o arquiteto
/contato              Contato (ou só seção no rodapé)              [A CONFIRMAR — F1]
```

### 4.1 Home — ordem dos blocos (espelha a referência, D-01)

Revisado em 2026-09-26: o cliente quer **toda a estrutura** da referência. A Home segue a mesma ordem e composição:

1. **Abertura** (sem menu no topo): nome em caixa-alta + frase curta **[C1]** + redes **[F4]**; **2 cards grandes** com foto e chamada **[F1, F2]**; **linha de 5 cards pequenos** → artigos/TCC **[E1, E2]**; **foto grande do Guilherme recortada à direita** **[C5]**.
2. **Projetos:** grade de 3 colunas × 2 linhas, card com imagem e legenda **[D1]**.
3. **Destaques** (na referência, "Destaques impressos"): **opcional** — só entra com material real **[C6]**.
4. **Sobre:** texto com pontos em negrito à esquerda + retrato à direita **[C1, C2, C5]**.
5. **Contato:** e-mail, WhatsApp e Instagram **[F3, F4]**.

**Time: removido** (2026-09-26) — o Guilherme não tem equipe. É a única seção da referência que fica de fora.

Cada seção tem um fundo próprio na referência (cinza, grafite, preto, cinza-claro, cinza-médio).

---

## 5. Estrutura da página de projeto

1. Voltar para projetos.
2. Título + subtítulo (ambientes/tipo + cidade).
3. Selo de tipo: **Acadêmico** ou **Interiores** (e real/conceitual) **[D2]**.
4. Imagem hero (render principal).
5. Ficha técnica: ano, local, área (se houver), tipo, disciplina/professor (acadêmicos, se desejado) **[D2]**.
6. Conceito: texto narrativo.
7. Galeria de renders (grade + visualização ampliada).
8. Plantas baixas / esquemas / diagramas.
9. Navegação para o próximo/anterior projeto + CTA.

### 5.1 Projeto de extensão — o que já se sabe (2026-09-26)

Fonte: `RESPOSTAS-CLIENTE.md`.

| Item | Situação |
| --- | --- |
| Instituição | UNIFACIG |
| Nome do projeto de extensão | **[A CONFIRMAR]** — não informado |
| Orientação (crédito) | Lidiane Espindula — **grafia e forma de crédito [A CONFIRMAR]** |
| Casas | 1 |
| Material disponível | Nenhum ainda (sem render, planta ou foto do antes) |
| Autorização das famílias | Sim, por mensagem — **registro por escrito [A CONFIRMAR]** |

**Consequências para o planejamento:**
- O projeto **só entra na v1 se o material chegar antes do lançamento**. Sem material, a página não é criada (não usar imagem genérica no lugar).
- A ficha técnica (§5, item 5) precisa de um campo para **instituição e orientação**. Isso já estava previsto para acadêmicos ("disciplina/professor").
- O modelo atual (`type: academico | interiores`) não tem uma categoria para extensão. **Decisão em aberto (D-12):** tratar como `academico` + `status: real`, ou criar um tipo `extensao`.
- A pergunta sobre "foto do antes" indica um possível bloco **antes/depois**. Não está no escopo atual; entra só com aprovação (D-13).

---

## 6. Modelo de conteúdo (MDX no repositório — v1)

### Projeto — `content/projetos/<slug>.mdx`
```yaml
title: string
subtitle: string            # ex.: "Cozinha e banheiro · Cidade, UF"
type: academico | interiores
status: real | conceitual
year: number
location: string
area: string?               # opcional
cover: string               # caminho da imagem hero
gallery: string[]           # renders
drawings: string[]          # plantas/esquemas
featured: boolean           # aparece na Home
order: number
```
Corpo MDX = texto de conceito.

### Artigo — `content/artigos/<slug>.mdx`
```yaml
title: string
excerpt: string
date: YYYY-MM-DD
category: urbanismo | extensao | paisagismo | ...   # [A CONFIRMAR — E5]
cover: string?
pdf: string?                # ex.: TCC completo para download [A CONFIRMAR — E3]
featured: boolean
```

> Se o cliente quiser publicar sozinho (E4), migrar para um CMS headless mantendo este mesmo modelo de campos.

---

## 7. Direção visual

- **Estilo:** clean, moderno, minimalista e com tipografia forte (briefing §3).
- **Marca:** o nome **"Guilherme Calixto"** em tipografia, sem logo (D-03 e D-04, 2026-09-26). A logo atual (1º período) **não** será usada. O redesign de logo sai da proposta da v1.
- **Cores:** base preto/branco/cinzas; cor de destaque a definir **[A4, A5]**.
- **Tipografia:** uma display forte (caixa-alta, geométrica) + uma de texto legível para artigos longos. Escolha final na F1, sem copiar as fontes da referência.
- **Imagens:** renders são o conteúdo principal, então a interface deve ficar em segundo plano.
- **Estrutura:** o cliente gostou de **toda a estrutura** da referência (D-01). Segue valendo a regra da §2.2: as seções que dependem de material que ele não tem (time, destaques impressos, selos, infoprodutos) só entram com material real.
- **Evitar (AI-GUARDRAIL §6):** excesso de cards, gradientes decorativos, animações sem função, textos placeholder apresentados como finais.

### 7.1 Opções de fundo (D-02) — 2026-09-26

Três versões da Home, todas com a estrutura da referência (§4.1) e o mesmo conteúdo provisório, para o cliente escolher:

| Opção | Descrição |
| --- | --- |
| A — Claro | Todas as seções em tons claros (off-white e bege-acinzentado) |
| B — Escuro | Todas as seções em tons de preto e grafite |
| C — Alternado | Um fundo por seção, como na referência: cinza, grafite, preto, cinza-claro |

- Tipografia usada nas opções (**provisória**, ainda não aprovada): Archivo, peso 800, caixa-alta nos títulos.
- A primeira versão (2026-09-26) tinha menu no topo e nome gigante; foi descartada por não seguir a estrutura da referência.
- Nenhuma cor de destaque foi usada; A5 segue aberta.
- Todo o conteúdo entre colchetes é provisório e aponta para a pergunta que o preenche.
- Link das opções: https://claude.ai/artifact/ATyxnNcovmBBY1XWuahBp8

---

## 8. Stack e arquitetura técnica

| Camada | Decisão |
| --- | --- |
| Framework | **Next.js (App Router) + TypeScript** — decidido |
| Estilo | CSS Modules ou Tailwind *(decidir na F3)* |
| Conteúdo | MDX no repositório (v1); CMS headless opcional (E4) |
| Imagens | `next/image` (otimização, lazy-load, AVIF/WebP) — renders são pesados |
| Hospedagem | Vercel |
| Domínio/DNS | Registro.br → Vercel |
| SEO | Metadata API, Open Graph por página, `sitemap.xml`, `robots.txt`, dados estruturados (Person/Article) |
| Analytics | Vercel Analytics ou GA4 **[A CONFIRMAR — G4]** |
| Formulário (se houver) | Server Action + serviço de e-mail **[A CONFIRMAR — F1]** |

### Estrutura de pastas (proposta)
```text
app/
  layout.tsx
  page.tsx                  # Home
  projetos/page.tsx
  projetos/[slug]/page.tsx
  artigos/page.tsx
  artigos/[slug]/page.tsx
  sobre/page.tsx
  contato/page.tsx
components/
content/
  projetos/
  artigos/
lib/                        # leitura/parse do conteúdo MDX
public/images/
```

---

## 9. Fases e entregáveis

Sem datas: o briefing não define prazo. As fases são sequenciais e cada uma só fecha com o critério de conclusão atendido.

| Fase | Entregáveis | Critério de conclusão |
| --- | --- | --- |
| **F0 — Descoberta** | Questionário respondido; materiais recebidos (renders, plantas, textos, foto) | Todas as perguntas essenciais (★) respondidas; materiais da v1 recebidos |
| **F1 — Identidade** | Tipografia, paleta e assinatura do nome (ou logo, se contratada) | Aprovação explícita do cliente |
| **F2 — Wireframes** | Wireframes de Home, Projeto, Artigo (desktop + mobile) | Aprovação explícita do cliente |
| **F3 — Setup técnico** | Repositório, projeto Next.js, deploy de preview na Vercel | Preview acessível por URL |
| **F4 — Implementação** | Layout base → Home → Projetos → Artigos → Sobre/Contato | Páginas funcionais com conteúdo de teste identificado como teste |
| **F5 — Conteúdo** | Projetos e textos reais inseridos | Nenhum placeholder restante |
| **F6 — QA** | Testes responsivos, Lighthouse, acessibilidade, SEO, links | Lighthouse ≥ 90 em Performance/SEO/Acessibilidade; sem links quebrados |
| **F7 — Lançamento** | Domínio apontado, HTTPS, Search Console, analytics | Site no ar em `guilhermecalixtoarq.com.br` |

---

## 10. Dependências do cliente

- [ ] Respostas do `PERGUNTAS-CLIENTE.md`.
- [ ] Renders e plantas dos projetos da v1 (em alta resolução).
- [ ] Textos de conceito de cada projeto, ou tópicos para redação.
- [ ] Foto profissional e texto/dados para o “Sobre”.
- [ ] Artigos e TCC (arquivos) para o lançamento.
- [ ] Registro do domínio (titularidade em CPF/CNPJ do cliente).
- [ ] Aprovações nas fases F1, F2 e antes do lançamento.

---

## 11. Decisões em aberto

| # | Decisão | Pergunta |
| --- | --- | --- |
| D-01 | O que agradou na referência | A1, A2 — **Fechada (2026-09-26): toda a estrutura.** A2 segue aberta |
| D-02 | Paleta e cor de destaque | A4, A5 — **Em andamento:** 3 opções de fundo montadas para o cliente escolher (§7.1). A5 aberta |
| D-03 | Redesign de logo na proposta | B1 — **Fechada (2026-09-26): não.** Só o nome em tipografia |
| D-04 | Assinatura/nome da marca | B2 — **Fechada (2026-09-26): "Guilherme Calixto"** |
| D-05 | Artigos: página própria ou destaque na Home | E1 |
| D-06 | Formato do TCC (PDF completo / resumo) | E3 |
| D-07 | CMS (cliente publica sozinho?) | E4 |
| D-08 | CTA principal (WhatsApp / formulário / artigos) | F1 |
| D-09 | Domínio registrado e titular | G1 |
| D-10 | Analytics + aviso de cookies (LGPD) | G4 |
| D-11 | Estilização: CSS Modules ou Tailwind | Interna (F3) |
| D-12 | Projeto de extensão: tipo `academico` (real) ou tipo novo `extensao` | Interna + cliente |
| D-13 | Incluir bloco antes/depois na página de projeto | Cliente (depende de existir foto do antes) |

---

## 12. Riscos

| Risco | Impacto | Mitigação |
| --- | --- | --- |
| Poucos projetos na v1 | Portfólio parece vazio | Páginas de projeto mais ricas (processo, plantas, conceito); grade pensada para poucos itens |
| Artigos sem conteúdo no lançamento | Seção vazia prejudica autoridade | Lançar só com o que existir (ex.: TCC); ocultar a seção se não houver nada **[E2]** |
| Renders muito pesados | Site lento, SEO ruim | `next/image`, compressão, tamanhos responsivos |
| Imitar a referência sem ter a mesma trajetória | Soa genérico/forçado | Usar só as seções que tenham material real (§2.2) |
| Projetos de clientes sem autorização | Problema ético/legal | Confirmar permissão **[D5]** |
| Projeto de extensão sem material no lançamento | Projeto anunciado mas sem página | Só publicar quando houver render/planta/foto; não depender dele para lançar |
| Autorização das famílias só verbal | Exposição de moradia de famílias atendidas (LGPD/imagem) | Pedir autorização por escrito; não mostrar endereço nem rostos sem permissão explícita |
| Domínio indisponível | Atraso no lançamento | Checar no Registro.br e ter alternativas **[G1]** |
