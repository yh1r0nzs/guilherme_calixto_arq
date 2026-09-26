# PLANNING — Website & Portfólio Guilherme Calixto

> Fonte de verdade do projeto (ver `AI-GUARDRAIL.md` §13 e §15).
> Itens marcados **[A CONFIRMAR]** dependem de resposta do cliente e apontam para o ID da pergunta em `PERGUNTAS-CLIENTE.md`.
> Última atualização: 2026-09-26 (respostas das rodadas 1 e 2 em `RESPOSTAS-CLIENTE.md`)

---

## 1. Resumo do projeto

| Item | Definição |
| --- | --- |
| Cliente | Guilherme Calixto, estudante de arquitetura (ainda sem registro no CAU) |
| Contato | cgarquitetura27@gmail.com · (32) 98454-2644 |
| Domínio pretendido | `guilhermecalixtoarq.com.br` (consulta/registro no Registro.br) **[A CONFIRMAR — G1]** |
| Prazo | Sem prazo definido no briefing |
| Problema | Ausência de visibilidade e de posicionamento digital |
| Objetivo | Ganhar visibilidade, reconhecimento e autoridade técnica/conceitual |
| Público | Estudantes de arquitetura, arquitetos, engenheiros e clientes finais de interiores |
| Tipo de solução | Portfólio pessoal: quem é o Guilherme + projetos autorais + renders para terceiros. Artigos só se houver material **[E2]**; TCC fora da v1 |

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
| **Não copiar** | “Time”, “Destaques impressos”, selos (Forbes, Casa Vogue) | Dependem de trajetória que não está no briefing; só entram com material real **[A CONFIRMAR — C6]** |
| **Não copiar** | Blog | **A referência não tem blog.** O hub de artigos será desenho próprio |

> **Divergência com o briefing:** o briefing descreve a referência como tendo “blog/recursos técnicos”. Na verdade, a área de conteúdo dela é de infoprodutos (links de venda). A seção de artigos/TCC do Guilherme **não tem modelo direto na referência**.

---

## 3. Escopo

### 3.1 Dentro da v1 (MVP)
- Site institucional/portfólio responsivo em Next.js.
- Páginas: Home, Projetos (lista), Projeto (detalhe), Artigos (lista), Artigo (detalhe), Sobre, Contato *(mapa final pendente — ver §4)*.
- Poucos projetos na v1, misturando acadêmicos e de interiores (briefing §4) **[A CONFIRMAR — D1]**.
- Artigos: só entram na v1 se já houver material **[A CONFIRMAR — E2]**. **TCC fora da v1**: ainda não começou (rodada 2).
- CTA principal de contato **[A CONFIRMAR — F1]**.
- SEO básico, Open Graph, sitemap, performance e acessibilidade.
- Publicação na Vercel com domínio próprio.

### 3.2 Fora da v1 (proposta → aprovação antes de incluir)
- Redesign de marca/logo: **provavelmente fora**. O cliente prefere usar a logo que já tem (C + A dourado). Confirmar se é a logo do 1º período e receber o arquivo **[A CONFIRMAR — B1]**.
- CMS para o cliente publicar sozinho **[A CONFIRMAR — E4]**.
- Versão em inglês **[A CONFIRMAR — H1]**.
- Depoimentos, newsletter, área de downloads pagos, infoprodutos **[A CONFIRMAR — H2, H3]**.
- E-mail profissional no domínio **[A CONFIRMAR — G2]**.

---

## 4. Mapa do site (proposta — pendente de validação)

```text
/                     Home
/projetos             Projetos autorais do GC (plantas, renders, esquemas)
/projetos/[slug]      Detalhe do projeto autoral
/renders              Visualização 3D para terceiros ("Projeto: X · Render: Guilherme Calixto")
/renders/[slug]       Detalhe do render (galeria + créditos)
/artigos              Só se houver artigos no lançamento            [A CONFIRMAR — E2]
/sobre                Quem é, o que faz, onde atua (página central — F1)
/contato              Seção no rodapé: Instagram, WhatsApp, e-mail, LinkedIn (talvez)
```

### 4.1 Home — ordem proposta dos blocos
1. **Abertura:** logo + "Guilherme Calixto" + descritor (ex.: projetista · visualização 3D) **[B2]** + redes sociais.
2. **Sobre:** quem é, o que faz, onde atua + foto + link para /sobre **[C1–C5]**. É a ação principal do site (F1, rodada 2).
3. **Projetos autorais:** 2 a 3 em blocos grandes **[D3]**.
4. **Renders (visualização 3D):** blocos com crédito do autor de cada projeto.
5. **Contato:** Instagram, WhatsApp, e-mail e, talvez, LinkedIn **[F4]**.

> Artigos entram como bloco entre 4 e 5 só se houver material no lançamento **[E2]**.

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
section: autoral | render   # autoral → /projetos; render → /renders (rodada 2)
projectAuthor: string?      # obrigatório quando section = render ("Projeto autoral de: X")
# render sempre creditado como "Render: Guilherme Calixto"
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
- **Marca:** o cliente quer usar a logo que já tem: monograma **C + A dourado** (resposta B1, 2026-09-26). Avaliar o arquivo junto com a tipografia do nome. Se for a logo do 1º período, apontar ao cliente o que precisa de ajuste antes de usar **[B1, B2]**.
- **Cores:** base preto/branco/cinzas; o **dourado da logo** é o candidato natural a cor de destaque, com uso pontual **[A4, A5]**.
- **Tipografia:** uma display forte (caixa-alta, geométrica) + uma de texto legível para artigos longos. Escolha final na F1, sem copiar as fontes da referência.
- **Imagens:** renders são o conteúdo principal, então a interface deve ficar em segundo plano.
- **Evitar (AI-GUARDRAIL §6):** excesso de cards, gradientes decorativos, animações sem função, textos placeholder apresentados como finais.

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
- [ ] Artigos (se houver) para o lançamento. TCC fora da v1.
- [ ] Autorização de cada autor dos projetos renderizados.
- [ ] Links de Instagram e LinkedIn.
- [ ] Registro do domínio (titularidade em CPF/CNPJ do cliente).
- [ ] Aprovações nas fases F1, F2 e antes do lançamento.

---

## 11. Decisões em aberto

| # | Decisão | Pergunta |
| --- | --- | --- |
| D-01 | O que agradou na referência — **parcial:** gostou da estrutura geral (item 4) | A1, A2 |
| D-02 | Paleta e cor de destaque — dourado da logo como candidato | A4, A5 |
| D-03 | Redesign de logo — **cliente prefere a logo C + A que já tem**; falta o arquivo e confirmar se é a do 1º período | B1 |
| D-04 | Assinatura/nome da marca | B2 |
| D-05 | Artigos: página própria ou destaque na Home — **depende de haver artigos prontos** | E1, E2 |
| D-06 | ~~Formato do TCC~~ — **fechada:** TCC fora da v1 (ainda não começou) | E3 |
| D-07 | CMS (cliente publica sozinho?) | E4 |
| D-08 | ~~CTA principal~~ — **fechada:** conhecer o Guilherme (Sobre em destaque); contato por Instagram, WhatsApp, e-mail | F1 |
| D-09 | Domínio registrado e titular | G1 |
| D-10 | Analytics + aviso de cookies (LGPD) | G4 |
| D-11 | Estilização: CSS Modules ou Tailwind | Interna (F3) |
| D-12 | Renders para terceiros — **formato fechado** (seção própria, "Projeto: X · Render: GC"); falta a autorização de cada autor | D5 |
| D-13 | Descritor da assinatura ("projetista", "visualização 3D"…) sem usar "arquiteto" | B2 |

---

## 12. Riscos

| Risco | Impacto | Mitigação |
| --- | --- | --- |
| Poucos projetos na v1 | Portfólio parece vazio | Páginas de projeto mais ricas (processo, plantas, conceito); grade pensada para poucos itens |
| Artigos sem conteúdo no lançamento | Seção vazia prejudica autoridade | Lançar só com o que existir (ex.: TCC); ocultar a seção se não houver nada **[E2]** |
| Renders muito pesados | Site lento, SEO ruim | `next/image`, compressão, tamanhos responsivos |
| Imitar a referência sem ter a mesma trajetória | Soa genérico/forçado | Usar só as seções que tenham material real (§2.2) |
| Projetos de clientes sem autorização | Problema ético/legal | Confirmar permissão **[D5]** |
| Renders de projetos de terceiros sem crédito | Parecer que o projeto é do Guilherme; problema ético/legal | Seção separada + campo `projectAuthor` obrigatório + autorização do autor **[D-12, D5]** |
| Uso de "arquiteto"/"arquitetura" sem registro no CAU | Exercício ilegal da profissão (Lei 12.378/2010); problema com o CAU | Assinatura sem "arquiteto"; revisar o "arq" do domínio e o "A" da logo com o cliente **[B2, G1]** |
| Domínio indisponível | Atraso no lançamento | Checar no Registro.br e ter alternativas **[G1]** |
