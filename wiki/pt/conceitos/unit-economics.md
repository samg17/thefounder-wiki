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

**Regra de ouro:** Nunca escale antes de entender suas unit economics.

---

## CAC — Custo de Aquisição de Cliente

```
CAC = Total gasto em vendas e marketing (período)
      ÷ Número de clientes novos adquiridos (mesmo período)
```

Inclua no numerador: salários, ferramentas, ads, eventos, agências — tudo que vai para aquisição.

---

## LTV — Lifetime Value

**Versão simples:**
```
LTV = Ticket médio mensal × Tempo médio de retenção (meses)
```

**Versão mais precisa:**
```
LTV = Margem bruta mensal por cliente × Tempo médio de retenção
```

| Churn mensal | Tempo médio de retenção |
|---|---|
| 1% | ~8 anos |
| 3% | ~2.8 anos |
| 5% | ~1.7 anos |
| 10% | ~10 meses |

---

## Payback period

```
Payback = CAC ÷ Margem de contribuição mensal por cliente
```

Benchmarks: < 12 meses (excelente) · 12–24 meses (aceitável) · > 24 meses (preocupante)

---

## A relação LTV:CAC

- LTV:CAC < 1 → você destrói valor adquirindo clientes
- LTV:CAC ≈ 3 → benchmark para SaaS saudável
- LTV:CAC > 5 → ou você está subinvestindo em crescimento ou o denominador está subestimado

---

## Erros comuns

❌ Excluir salários do time de vendas do CAC
✅ CAC deve incluir tudo — salário, comissão, ferramentas, overhead

❌ Usar LTV de receita em vez de LTV de margem para comparar com CAC
✅ Compare CAC com o que o cliente gera de **margem**, não de receita bruta

❌ Escalar antes de ter payback positivo em pelo menos 1 cohort
✅ Valide unit economics em um segmento antes de replicar
