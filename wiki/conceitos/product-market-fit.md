---
title: Product-Market Fit (PMF)
category: conceito
tags: [pmf, validacao, retencao, crescimento]
updated: 2024-01-01
sources: []
status: stable
related: [[icp]], [[unit-economics]], [[guardrails-pesquisa-mercado]]
---

# Product-Market Fit (PMF)

O momento em que um produto satisfaz uma demanda de mercado forte o suficiente para gerar crescimento orgânico sustentável. Conceito central para decidir quando escalar.

**Definição de Marc Andreessen:** PMF significa estar em um bom mercado com um produto que consegue satisfazer esse mercado.

**Definição prática:** Clientes adoram o produto, usam com frequência, recomendam espontaneamente, e você tem dificuldade de atender a demanda.

---

## PMF não é binário

PMF é um espectro, não um interruptor. Você pode ter PMF fraco (suficiente para sobreviver, não para escalar), PMF moderado (crescimento possível com esforço), ou PMF forte (crescimento acontece quase sozinho).

A maioria das startups que falham tentam escalar com PMF fraco ou inexistente.

---

## Como medir PMF

### Método Sean Ellis (survey)

Pergunte aos usuários ativos: "Como você se sentiria se não pudesse mais usar [produto]?"

- Muito desapontado
- Um pouco desapontado
- Não desapontado (não é realmente necessário)
- Não se aplica, já deixei de usar

**Benchmark:** Se ≥40% responderem "muito desapontado", há sinal forte de PMF.

**Limitação:** Funciona melhor para produtos de consumo com muitos usuários. Em B2B com poucos clientes, a amostra pode ser pequena demais.

### Retenção por cohort

O gráfico de retenção mais importante: % de usuários/clientes ativos ao longo do tempo, por cohort de aquisição.

**Sinal de PMF:** A curva de retenção estabiliza (flattens) — há um núcleo de clientes que continua usando indefinidamente.

**Sinal de falta de PMF:** A curva continua caindo e tende a zero — clientes chegam, experimentam e saem.

### Net Promoter Score (NPS)

Pergunta: "Em uma escala de 0–10, qual a probabilidade de recomendar [produto] para um amigo ou colega?"

```
NPS = % Promotores (9–10) - % Detratores (0–6)
```

Benchmarks aproximados:
- NPS > 50: excelente, sinal forte de PMF
- NPS 30–50: bom, há PMF em desenvolvimento
- NPS < 30: sinal de alerta

**Limitação:** NPS mede satisfação declarada, não comportamento real. Combine com retenção.

### Crescimento orgânico

Qual % dos novos clientes vem de referência, boca a boca ou busca orgânica (sem paid)?

- > 30% orgânico: sinal positivo de PMF
- Crescimento só com paid, que para quando o investimento para: sinal de alerta

---

## Sinais qualitativos de PMF

**Sinais positivos:**
- Clientes ficam frustrados quando o produto cai ou tem bugs
- Clientes constroem workflows críticos em cima do produto
- Vendas fica mais fácil com o tempo (menos objeções, ciclos menores)
- Recebem pedidos de clientes que você não prospectou
- Clientes pedem features de expansão, não features básicas

**Sinais de ausência de PMF:**
- Churn alto nos primeiros 60–90 dias
- Clientes "gostam mas não usam com frequência"
- Vendas é sempre difícil, exige muito esforço de educação
- Clientes pedem descontos frequentemente
- NPS neutro — ninguém odeia, ninguém ama

---

## PMF é sempre relativo a um segmento

Um produto pode ter PMF forte com um ICP e nenhum PMF com outro. "Não temos PMF" muitas vezes significa "não temos PMF com o segmento que estamos perseguindo".

Antes de concluir que o produto não tem PMF, verifique:
- Há subgrupo de clientes com retenção muito melhor que a média?
- O que os clientes que ficam têm em comum?
- Você está medindo PMF no segmento certo?

Ver [[icp]].

---

## Erros comuns

❌ Escalar antes de ter PMF claro
✅ PMF primeiro, escala depois. Crescer com PMF fraco queima capital e cria problemas de retenção que ficam mais difíceis de resolver com escala

❌ Confundir interesse inicial com PMF ("todos adoraram a demo")
✅ PMF se mede no uso contínuo, não na primeira impressão

❌ Medir PMF só com métricas de aquisição (quantos se cadastraram)
✅ PMF é sobre retenção — o que importa é quem ficou, não quem chegou

❌ Acreditar que PMF é permanente
✅ Mercado e concorrência mudam. PMF precisa ser re-validado periodicamente

---

## O que fazer sem PMF

1. Voltar para pesquisa com clientes — [[guardrails-pesquisa-mercado]]
2. Identificar o subgrupo com melhor retenção e concentrar nele
3. Revisar o ICP — talvez o problema seja o segmento, não o produto
4. Pivotar com base em aprendizado real, não em especulação
5. Não contratar time de vendas e marketing agressivamente — isso amplifica os problemas, não os resolve

---

## Conexões

- [[icp]] — PMF é sempre relativo a um ICP específico
- [[unit-economics]] — sem PMF, LTV é baixo e churn é alto — unit economics não fecham
- [[guardrails-pesquisa-mercado]] — como pesquisar para encontrar onde o PMF existe
