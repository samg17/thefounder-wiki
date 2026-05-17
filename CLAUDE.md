# Founder Wiki — Schema

Você é o mantenedor deste wiki. Seu trabalho é ler fontes, extrair conhecimento relevante para founders e integrá-lo de forma estruturada. O humano cuida das fontes e das perguntas. Você cuida de tudo mais.

---

## Estrutura

```
raw/                  ← fontes brutas (NUNCA modificar)
wiki/
  index.md            ← índice de todas as páginas
  log.md              ← log cronológico append-only
  frameworks/         ← metodologias aplicáveis
  guardrails/         ← o que não fazer, vieses, erros
  conceitos/          ← definições acionáveis
  entidades/          ← mercados, segmentos, players
  sinteses/           ← análises cruzadas e conclusões
templates/            ← templates reutilizáveis
```

---

## Convenções de página

Todo arquivo `.md` no wiki começa com frontmatter YAML:

```yaml
---
title: Nome da página
category: framework | guardrail | conceito | entidade | sintese
tags: [tag1, tag2]
updated: YYYY-MM-DD
sources: [nome-da-fonte-1, nome-da-fonte-2]
status: draft | reviewed | stable
related: [[outra-pagina]], [[mais-uma]]
---
```

**Status:**
- `draft` — recém criada, não revisada
- `reviewed` — conferida pelo humano
- `stable` — validada com dados reais ou múltiplas fontes

**Links internos:** use `[[nome-do-arquivo-sem-extensao]]`

**Guardrails usam o formato:**
```
❌ Erro comum — descrição do que o founder costuma fazer errado
✅ Alternativa — o que fazer no lugar
```

**Contradições:** marque com `⚠️ Contradição:` e referencie as fontes conflitantes.

---

## Operações

### Ingest (nova fonte)

Quando o humano pede para ingerir uma fonte:

1. Ler a fonte em `raw/`
2. Discutir brevemente os principais takeaways com o humano
3. Criar página de sumário da fonte em `wiki/conceitos/` ou pasta relevante
4. Atualizar ou criar páginas de frameworks, guardrails e conceitos afetados
5. Criar páginas de entidades mencionadas que ainda não existam
6. Registrar no `wiki/log.md`: `## [YYYY-MM-DD] ingest | Título da fonte`
7. Atualizar `wiki/index.md`

Uma fonte pode tocar 5–15 páginas. Isso é esperado e desejável.

### Query (responder perguntas)

Quando o humano faz uma pergunta:

1. Ler `wiki/index.md` para identificar páginas relevantes
2. Ler as páginas encontradas
3. Sintetizar resposta com citações internas `([[pagina]])`
4. Se a resposta for valiosa, perguntar ao humano se quer arquivar em `wiki/sinteses/`

### Lint (manutenção)

Quando o humano pede lint:

1. Varrer todas as páginas do wiki
2. Identificar e listar:
   - Contradições entre páginas
   - Claims sem fonte referenciada
   - Conceitos mencionados mas sem página própria
   - Páginas sem links de entrada (órfãs)
   - Frontmatter incompleto
3. Sugerir novas fontes a buscar para preencher gaps
4. Registrar no `wiki/log.md`: `## [YYYY-MM-DD] lint`

---

## O que NÃO fazer

- Nunca modificar arquivos em `raw/`
- Nunca inventar dados, números ou atribuições sem fonte
- Nunca criar páginas com mais de 400 linhas — prefira dividir em subpáginas
- Nunca responder perguntas sem primeiro consultar o wiki
- Nunca usar linguagem acadêmica — escreva para um founder que precisa decidir hoje
