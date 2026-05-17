---
title: Unit economics
category: conceito
tags: [financeiro, cac, ltv, margem, payback, saas]
updated: 2024-01-01
sources: []
status: stable
related: [[icp]], [[product-market-fit]]
---

# Unit economics

Métricas que medem a rentabilidade de uma unidade do negócio — tipicamente um cliente. Fundamentais para saber se o modelo de negócio é sustentável antes de escalar.

**Regra de ouro:** Nunca escale antes de entender suas unit economics. Crescer rápido com unit economics negativas é queimar dinheiro mais rápido.

---

## As métricas centrais

### CAC — Custo de Aquisição de Cliente

Quanto você gasta para adquirir um cliente pagante.

```
CAC = Total gasto em vendas e marketing (período)
      ÷ Número de clientes novos adquiridos (mesmo período)
```

**Inclua no numerador:** Salários de time de vendas e marketing, ferramentas, ads, eventos, agências, content, SEO — tudo que vai para aquisição.

**Período:** Use o mesmo período para numerador e denominador. Se há lag entre investimento e conversão (ciclo de vendas longo), ajuste o período.

**CAC por canal:** Calcule separadamente por canal de aquisição. O CAC blended esconde qual canal funciona.

---

### LTV — Lifetime Value

Quanto um cliente gera de receita (ou margem) ao longo de toda a relação com a empresa.

**Versão simples (receita):**
```
LTV = Ticket médio mensal × Tempo médio de retenção (meses)
```

**Versão mais precisa (margem de contribuição):**
```
LTV = Margem bruta mensal por cliente × Tempo médio de retenção
```

Use a versão de margem para comparar com CAC — você quer saber se o cliente gera lucro suficiente para cobrir o custo de aquisição.

**Churn e LTV:** LTV é extremamente sensível ao churn.

| Churn mensal | Tempo médio de retenção |
|---|---|
| 1% | ~8 anos |
| 3% | ~2.8 anos |
| 5% | ~1.7 anos |
| 10% | ~10 meses |

Pequenas reduções de churn têm impacto desproporcional no LTV.

---

### Payback period

Em quantos meses o cliente paga o CAC.

```
Payback = CAC ÷ Margem de contribuição mensal por cliente
```

**Por que importa:** É o prazo em que você precisa de capital antes de um cliente virar lucrativo. Payback longo = mais capital necessário para crescer.

Benchmarks gerais (variam por segmento e modelo):
- Excelente: < 12 meses
- Aceitável: 12–24 meses
- Preocupante: > 24 meses

---

### Margem bruta

Receita menos custos diretos de entrega do produto/serviço (COGS).

```
Margem bruta = (Receita - COGS) ÷ Receita
```

**O que entra no COGS:** Hosting, licenças de terceiros, suporte de clientes (se direto), custos de processamento de pagamento.

**Não entra no COGS:** Vendas, marketing, P&D, G&A.

Benchmarks por modelo (aproximados):
- SaaS puro: 70–85%
- SaaS com serviço embarcado: 50–70%
- Marketplace: 60–80%
- E-commerce: 20–50%
- Hardware: 30–60%

**Por que importa:** Margem bruta define o teto do LTV e a capacidade de investir em crescimento.

---

## A relação LTV:CAC

A métrica mais citada em unit economics.

**Interpretação:**
- LTV:CAC < 1 → você destrói valor adquirindo clientes
- LTV:CAC = 1–3 → você cobre o CAC mas sobra pouco
- LTV:CAC ≈ 3 → benchmark para SaaS saudável (regra do 3x)
- LTV:CAC > 5 → ou você está subinvestindo em crescimento ou o denominador está subestimado

**Cuidado:** LTV:CAC de 3x com payback de 36 meses é muito diferente de LTV:CAC de 3x com payback de 8 meses. Apresente os dois.

---

## Erros comuns

❌ Calcular LTV sem descontar churn corretamente
✅ Use churn mensal real, não estimado otimistamente

❌ Excluir salários do time de vendas do CAC
✅ CAC deve incluir tudo — salário, comissão, ferramentas, overhead do time de vendas

❌ Usar LTV de receita em vez de LTV de margem para comparar com CAC
✅ Compare CAC com o que o cliente gera de **margem**, não de receita bruta

❌ Calcular unit economics blended quando há múltiplos segmentos
✅ Calcule por segmento, por canal, por cohort — o blended esconde o que está funcionando

❌ Projetar LTV assumindo churn zero ou churn que nunca foi medido
✅ Use churn histórico real. Se não tem histórico, use benchmarks do setor como lower bound

❌ Escalar antes de ter payback positivo em pelo menos 1 cohort
✅ Valide unit economics em um segmento antes de replicar

---

## Como interpretar por estágio

**Pré-revenue:** Estime CAC com base em benchmarks do setor. LTV é hipótese.

**Early stage (primeiros 10–20 clientes):** Unit economics são ruidosas — cohorts pequenos, CAC artificialmente alto (founder vende direto), LTV não comprovada. Foque em entender a estrutura, não os números absolutos.

**Crescimento:** Cohorts começam a se estabilizar. Compare cohorts mais recentes com mais antigos — unit economics devem melhorar com aprendizado de canal e produto.

**Scale:** Unit economics devem melhorar com economias de escala no CAC (brand, referral, inbound) e no LTV (redução de churn, expansão de receita por cliente).

---

## Conexões

- [[icp]] — unit economics variam muito por segmento. Calcule por ICP.
- [[product-market-fit]] — churn alto é o principal sinal de falta de PMF e destrói LTV
