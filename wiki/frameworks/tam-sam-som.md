---
title: TAM / SAM / SOM
category: framework
tags: [mercado, tamanho, tam, sam, som, validacao]
updated: 2024-01-01
sources: []
status: stable
related: [[porter-5-forcas]], [[icp]], [[guardrails-pesquisa-mercado]]
---

# TAM / SAM / SOM

Framework para estimar e comunicar tamanho de mercado. Mais importante do que o número em si é a **metodologia** usada para chegar nele.

---

## Definições

| Sigla | Nome | Definição |
|---|---|---|
| TAM | Total Addressable Market | Todo o mercado se você tivesse 100% de share |
| SAM | Serviceable Addressable Market | Parcela do TAM que você pode servir com seu modelo atual |
| SOM | Serviceable Obtainable Market | Parcela do SAM que você pode capturar realisticamente em 3–5 anos |

**Analogia:** TAM = todo mundo que tem fome no mundo. SAM = todo mundo que quer pizza na sua cidade. SOM = quem você consegue alcançar com sua capacidade de entrega atual.

---

## Por que isso importa

**Para você:** Saber se o mercado é grande o suficiente para o negócio que você quer construir. Um negócio de R$10M em um mercado de R$50M pode ser ótimo. Em um mercado de R$100M pode ser difícil de financiar como venture.

**Para investidores:** Validar se há espaço para um negócio grande. Investidores de venture tipicamente buscam TAM de no mínimo US$1–10bi para justificar o modelo de retorno deles.

**Cuidado:** TAM impressiona investidores, SOM é o que você precisa defender com dados.

---

## Como calcular — duas abordagens

### Abordagem top-down

Pega o mercado total de uma categoria e afunila.

```
Mercado global de CRM: US$60bi (fonte: relatório Gartner 2023)
→ Brasil representa ~2% do PIB mundial: US$1.2bi
→ Segmento PME (seu foco): 30% do mercado: US$360M
= TAM: US$360M
```

**Problema:** Depende de relatórios de mercado que muitas vezes são imprecisos, desatualizados ou usam definições de mercado diferentes da sua.

**Quando usar:** Para comunicação inicial com investidores, para dar ordem de grandeza.

### Abordagem bottom-up

Constrói o número de baixo para cima a partir de dados reais.

```
Número de potenciais clientes no segmento: 50.000 empresas (fonte: IBGE/Receita Federal)
× Ticket médio anual estimado: R$6.000/ano
= TAM: R$300M
```

**Vantagem:** Mais defensável, baseado em dados verificáveis.
**Problema:** Exige dados de mercado que nem sempre existem.

**Quando usar:** Para validar e refinar a estimativa top-down. Se os dois métodos chegam em números parecidos, mais confiança. Se divergem muito, entender por quê.

### Abordagem por analogia

Usa um mercado similar (outro país, segmento adjacente) como referência.

```
EUA: mercado de X tem penetração de 15% com ticket de US$500/empresa/ano
Brasil tem 1/6 do PIB dos EUA → ajuste para paridade de poder de compra
= TAM estimado: US$X
```

**Quando usar:** Em mercados novos onde não há dados diretos. Sempre declare a analogia explicitamente e suas limitações.

---

## Do TAM ao SAM ao SOM

**TAM → SAM:** Aplique filtros do seu modelo de negócio
- Geográficos (você só opera em SP hoje)
- Segmento (você só serve empresas com 10–200 funcionários)
- Canal (você só vende direto, não via distribuidor)
- Capacidade de suporte (você ainda não tem equipe para enterprise)

**SAM → SOM:** Baseie em capacidade de execução
- Quantos clientes sua equipe consegue adquirir e atender nos próximos 3 anos?
- Qual sua conversão estimada do pipeline?
- Qual a capacidade do seu canal de distribuição?

O SOM é a ponte entre mercado e plano de negócio. Se seu SOM de 3 anos implica uma taxa de crescimento impossível, revise o modelo.

---

## Erros comuns

❌ Apresentar TAM como se fosse seu mercado real
✅ Sempre apresente os três números e como chegou em cada um

❌ Usar TAM genérico sem relevância para o seu segmento ("o mercado de software no Brasil")
✅ Defina o mercado pelo job que você resolve, não pela categoria tecnológica

❌ Não questionar a fonte do TAM ("segundo relatório da consultoria X")
✅ Verifique: quando foi publicado? Como foi calculado? A definição de mercado bate com a sua?

❌ SOM otimista sem base em capacidade de execução
✅ O SOM deve ser derivável do seu plano: headcount × produtividade × conversão

❌ Ignorar a dinâmica do mercado (crescimento, sazonalidade, regulação)
✅ Um TAM de R$1bi crescendo 30% ao ano é muito mais interessante do que um TAM de R$5bi estagnado

---

## Template de apresentação

Para investidores, estruture assim:

> "O TAM é de R$X, calculado a partir de [metodologia]. O SAM para nosso segmento [definição] é de R$Y. Nossa meta de SOM para os próximos 3 anos é de R$Z, o que representa [%] do SAM — consistente com [referência/benchmark]."

---

## Conexões

- [[icp]] — a definição do ICP é o que transforma TAM em SAM
- [[porter-5-forcas]] — a estrutura do mercado afeta o quanto do SAM você consegue capturar
- [[guardrails-pesquisa-mercado]] — como validar premissas do TAM com dados primários
