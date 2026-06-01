# 📊 Projeto de Dashboard - Sistema de Empréstimos

## 🔗 Acesso ao Dashboard

[Visualizar no Looker Studio](https://datastudio.google.com/reporting/0e7f1508-2ba0-482d-aad5-b4c07ae7d9d7)

---

## 🎯 Objetivo

Este projeto foi desenvolvido para oferecer **autonomia analítica às áreas de negócio**, permitindo acompanhamento interativo da carteira de empréstimos e análise de inadimplência com base em dados tratados e validados.

---

## 🖥️ Funcionalidades do Dashboard

- [Visão geral da carteira](ca://s?q=Explique_visao_geral_da_carteira)
- [Volume de empréstimos](ca://s?q=Detalhe_volume_de_emprestimos)
- [Ticket médio](ca://s?q=Explique_ticket_medio)
- [Taxa geral de inadimplência](ca://s?q=Explique_taxa_de_inadimplencia)
- [Análise de risco por grade (A–E)](ca://s?q=Explique_analise_de_risco_por_grade)
- [Inadimplência por finalidade](ca://s?q=Explique_inadimplencia_por_finalidade)
- [Evolução temporal](ca://s?q=Explique_evolucao_temporal)
- **Filtros interativos**: Grade, Faixa de renda, Finalidade, Período

---

## 🐍 Análise Estatística com Python

### 1. [Análise exploratória](ca://s?q=Explique_analise_exploratoria)

- Tratamento e padronização de dados (numéricos, percentuais, datas)
- Criação de variável binária de inadimplência
- Segmentação por risco (grade, renda, DTI)

### 2. [Teste de hipótese](ca://s?q=Explique_teste_de_hipotese)

Hipótese do negócio: _“A inadimplência aumentou por causa das grades D e E”_

- Teste aplicado: **Z-test para proporções**
- H0: inadimplência D/E ≤ média da carteira
- H1: inadimplência D/E > média da carteira
- Resultado: **p-valor < 0.05 → Rejeitamos H0**
- Conclusão: Grades D/E possuem inadimplência estatisticamente maior

### 3. [Recomendações](ca://s?q=Explique_recomendacoes)

- Revisar critérios de aprovação para grades D/E
- Monitorar concentração da carteira em B/C
- Incorporar variáveis adicionais: renda e DTI (endividamento)

---

## ✅ Conclusão Geral

O trabalho entregou:

- **Dashboard self-service** para autonomia analítica
- **Diagnóstico estatístico** sobre inadimplência
- **Governança de dados/IA**, reduzindo riscos de decisões baseadas em informações incorretas

---

## 🚀 Próximos Passos

- Expandir variáveis para enriquecer a análise (ex.: histórico de crédito, perfil demográfico)
- Criar alertas automáticos de risco no dashboard
- Integrar com sistemas internos para atualização em tempo real
