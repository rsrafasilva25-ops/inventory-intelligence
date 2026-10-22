# Inventory Intelligence | SQL & Analytics Engineering

## Visão geral

O **Inventory Intelligence** é um projeto de portfólio desenvolvido em PostgreSQL para análise de estoque, vendas e reposições, com foco em qualidade de dados, indicadores operacionais e apoio à tomada de decisão.

O projeto demonstra como estruturar dados relacionais, calcular indicadores, aplicar regras de negócio e identificar situações que exigem acompanhamento operacional.

**Contexto:** estudo analítico com dados simulados. Os resultados representam o cenário construído para demonstração, não uma operação comercial real.

## Objetivos do projeto

- Estruturar e relacionar dados de produtos, vendas, movimentações de estoque e reposições.
- Comparar quantidades vendidas com as saídas de estoque registradas.
- Calcular saldo de estoque e cobertura estimada em dias.
- Comparar os saldos com os níveis mínimos definidos.
- Identificar reposições pendentes e pedidos com previsão vencida.
- Aplicar testes de qualidade para identificar inconsistências nos dados.

## Tecnologias e recursos SQL

- PostgreSQL
- SQL
- CTEs (`WITH`)
- Agregações (`SUM`, `COUNT`)
- Junções (`JOIN`, `LEFT JOIN`)
- Regras condicionais (`CASE`)
- Tratamento de valores nulos (`COALESCE`, `NULLIF`)
- Agrupamentos e filtros
- Validação de regras de negócio

## Modelo de dados

O projeto utiliza quatro tabelas principais:

| Tabela | Finalidade |
|---|---|
| `inventory.produtos` | Cadastro de produtos, categorias, custos e estoque mínimo |
| `inventory.movimentacoes_estoque` | Registro de entradas e saídas de produtos |
| `inventory.vendas` | Quantidades vendidas, datas e preços unitários |
| `inventory.reposicoes` | Pedidos de