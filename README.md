# 📊 Análise de Vendas – Desafio **Alura Store**

**Autor:** Bruno – Especialização em Data Science  
**Data:** 18 de maio de 2025  

---

## 1 ▪ Contexto

O Sr. João é proprietário de quatro lojas que compõem o e-commerce **Alura Store**.  
**Objetivo:** identificar a unidade de pior desempenho para ser vendida, liberando capital para um novo negócio.

Métricas analisadas ⬇️  

| Métrica | Descrição |
|---------|-----------|
| **Faturamento total** | Receita bruta por loja |
| **Categoria mais popular** | Classe de produtos com maior volume de vendas |
| **Avaliação média** | Satisfação (1–5 estrelas) dos clientes |
| **Produtos mais / menos vendidos** | Itens com maior e menor demanda |
| **Frete médio** | Custo logístico médio por pedido |

As métricas foram normalizadas e combinadas em um **Score global** (0 = pior, 1 = melhor).

---

## 2 ▪ Painel Consolidado

| Loja | Faturamento (R$) | Avaliação&nbsp;Média | Frete&nbsp;Médio (R$) | Score Global |
|:---:|---------------:|:-----------------:|---------------:|-----------:|
| **1** | 1 534 509,12 | 3,98 | 34,69 | **0,33 ⬇️** |
| 4 | 1 384 497,58 | 4,00 | 31,28 | 0,42 |
| 2 | 1 488 459,06 | 4,04 | 33,62 | 0,62 |
| 3 | 1 464 025,03 | 4,05 | 33,07 | 0,67 |

> **Insight-chave:** apesar do maior faturamento, **Loja 1** tem o pior Score devido a frete elevado e menor satisfação dos clientes.

---

## 3 ▪ Análises Pontuais

### 3.1 Faturamento
* Loja 1 lidera em receita bruta, mas margens são impactadas por custos logísticos.

### 3.2 Categoria Mais Popular
* Todas as lojas têm **móveis** como categoria líder – não há vantagem competitiva diferenciada.

### 3.3 Avaliação Média
* Loja 1 possui **3,98/5**, ≈ 1,7 % abaixo da média das demais (4,03).

### 3.4 Produtos Destaque

| Loja | Mais Vendido (unid.) | Menos Vendido (unid.) |
|------|----------------------|-----------------------|
| 1 | Micro-ondas (60) | Headset (33) |
| 2 | Iniciando em programação (65) | Jogo de tabuleiro (32) |
| 3 | Kit banquetas (57) | Blocos de montar (35) |
| 4 | Cama box (62) | Guitarra (33) |

A campeã de vendas da Loja 1 vende 8 % menos que a da Loja 2.

### 3.5 Frete Médio
* Loja 1 pratica o frete mais alto (**R$ 34,69**), reduzindo competitividade.

---

## 4 ▪ Conclusão & Recomendação

Recomenda-se **vender a Loja 1**, pois concentra os pontos fracos:

1. **Frete elevado** → impacto direto na conversão.  
2. **Menor satisfação** → risco de churn e má reputação.  
3. **Mix de produtos** menos eficiente – best-sellers com menor tração.

Mesmo com maior faturamento, o conjunto de indicadores demonstra **desempenho operacional inferior**, refletido no Score 0,33.

---

## 5 ▪ Próximos Passos

| Ação | Responsável | Prazo |
|------|-------------|------:|
| Due-diligence contábil & jurídica (Loja 1) | Financeiro / Jurídico | 30 dias |
| Definir valuation & faixa de preço | CFO | 45 dias |
| Prospeção de compradores | Comercial | 60 dias |
| Plano de reinvestimento do capital | Diretoria | 75 dias |

---

### 🚀 Como reproduzir

```bash
# Clonar repositório
git clone https://github.com/brunopintonascimento/analisedevendas.git
cd analisedevendas

# Abrir o notebook no Google Colab
# (ou Jupyter, se preferir)
