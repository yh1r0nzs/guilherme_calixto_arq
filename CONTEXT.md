# CONTEXT — Estado atual do projeto

> Última atualização: 2026-09-26

## CONTEXTO ATUALIZADO

### Concluído

- Leitura do `briefing.md` e do `AI-GUARDRAIL.md`.
- Análise do site de referência (arquitetojoaogabriel.com): estrutura da Home, página de projeto, tipografia e plataforma (Wix).
- `PLANNING.md` criado: escopo, mapa do site, modelo de conteúdo, direção visual, stack, fases (F0–F7), dependências, decisões em aberto e riscos.
- `PERGUNTAS-CLIENTE.md` criado: 35 perguntas em 8 grupos (A–H), com as essenciais marcadas com ★.
- Recebidas as respostas sobre o projeto de extensão (2026-09-26) e registradas em `RESPOSTAS-CLIENTE.md`.
- Montadas 3 opções de fundo da Home (claro, escuro, alternado), refeitas para seguir a estrutura da referência, para o cliente escolher: https://claude.ai/artifact/ATyxnNcovmBBY1XWuahBp8

### Decisões

- Stack: **Next.js (App Router) + TypeScript**, hospedagem na Vercel (decisão do responsável).
- Conteúdo da v1 em MDX no repositório; CMS só se o cliente quiser publicar sozinho (E4).
- As perguntas ao cliente ficam em `PERGUNTAS-CLIENTE.md`; as respostas, em `RESPOSTAS-CLIENTE.md`.
- Não copiar da referência as seções que dependem de trajetória que o cliente não informou (time, mídia impressa, selos, infoprodutos).
- O projeto de extensão só entra na v1 se o material chegar antes do lançamento.
- D-01: o cliente gostou de toda a estrutura da referência (seções sem material real continuam de fora).
- D-03: sem logo nova; marca = nome em tipografia.
- D-04: assinatura "Guilherme Calixto".
- Seção Time removida da Home: o Guilherme não tem equipe.

### Alterações

- `PLANNING.md`: D-01, D-03 e D-04 fechadas; nova §7.1 (opções de fundo); redesign de logo fora da v1.
- `PLANNING.md` (antes): faculdade (UNIFACIG) no resumo; nova §5.1 com o projeto de extensão; decisões D-12 e D-13; dois riscos novos (material do projeto de extensão, autorização só por mensagem).
- Divergência já registrada: o briefing diz que a referência tem "blog/recursos técnicos", mas ela tem **infoprodutos**, não blog.

### Pendências

- Resposta completa do `PERGUNTAS-CLIENTE.md` (fase F0).
- Projeto de extensão:
  - nome do projeto (não informado);
  - grafia do nome de quem orienta ("Espindula" ou "Espíndula") e forma de crédito;
  - se a casa já foi concluída ou está em andamento;
  - autorização das famílias por escrito e o que ela cobre;
  - material (render, planta, foto do antes) — hoje não existe nenhum.
- Receber os demais materiais: renders, plantas, textos, foto e artigos/TCC.
- Confirmar o registro do domínio `guilhermecalixtoarq.com.br`.
- Decidir entre CSS Modules e Tailwind (interno, na F3).
- Cliente escolher o fundo (A, B ou C) — fecha D-02 junto com A5 (cor de destaque).
- Decidir se a seção Destaques fica na Home sem material (hoje aparece como opcional).
- Tirar a seção Time do canvas de opções de fundo (ainda aparece lá).
- Aprovar a tipografia (Archivo está nas opções só como proposta).
- Decidir D-12 (tipo do projeto de extensão) e D-13 (bloco antes/depois).

### Problemas

- Nenhum bloqueio técnico. A execução depende das respostas do cliente.
- O projeto de extensão ainda não tem material; não dá para contar com ele no lançamento.

### Próximo passo

- Enviar as 3 opções de fundo ao Guilherme e pedir a escolha + resposta da A5 (cor de destaque).
- Mandar ao Guilherme as 4 perguntas que ficaram em aberto sobre o projeto de extensão.
- Continuar a coleta das respostas do questionário. Com elas, fechar D-01 a D-13 no `PLANNING.md` e iniciar a F1 (Identidade).
