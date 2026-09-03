# 🛒 E-Commerce Analytics & Performance Dashboard

## 📌 Objetivos de Negócio
Análise de desempenho de vendas para uma plataforma de e-commerce com foco em identificar alavancas de crescimento de receita, eficiência de mídia geográfica, comportamento de categorias e governança na base de clientes.

## 📐 Metodologia & Governança de Dados
- **Qualidade de Dados:** Identificou-se uma divergência cadastral em que 19,3% das transações brutas (71 registros) pertenciam a IDs não cadastrados na base mestre do CRM.
- **Modelagem SQL:** Utilizou-se `INNER JOIN` para garantir a integridade dos dados demográficos na consolidação executiva, mantendo 296 transações validadas e R$ 22.025,02 em receita.
- **Processamento:** Tratamento de valores decimais em SQL e Python (`REPLACE(',', '.')`), deduplicação e análise distributiva.

## 📊 Principais Insights de Performance
1. **Concentração Geográfica:** CA, TX e DC concentram **29,0% da receita total**.
2. **Liderança por Categoria:** A categoria **Beauty** é o carro-chefe em faturamento (R$ 1.773,61), enquanto **Clothing** tem o maior Ticket Médio (R$ 100,91).
3. **Curva de Pareto:** Os top 20% clientes geram 35,8% da receita. A base apresenta baixa dependência de contas individuais, com frequência média de 1,74 compras por cliente.

## 🚀 Recomendações Práticas
- **Otimização de ROAS:** Redirecionar verba de campanhas de tráfego pago com geotargeting para os estados CA e TX.
- **Aumento de Ticket Médio:** Implementar réguas de *Cross-selling* sugerindo itens da categoria *Clothing* durante o checkout de produtos de *Beauty*.
- **Correção no Funil de Vendas:** Ajustar a validação do checkout do site para impedir a conclusão de compras sem cadastro ativo no CRM.

## 🛠️ Tecnologias Utilizadas
- **SQL:** Consultas analíticas, agregações e junções.
- **Python (Pandas, Seaborn):** EDA, sanity check de dados e gráficos.
- **Power BI / Looker Studio:** Dashboard interativo de página única.
