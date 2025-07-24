# Valuation Mult3

Esse repositório concentra os modelos e artefatos que eu utilizados para fazer o valuation da MULT3. Estou usando como base o [[https://ri.multiplan.com.br/ferramentas-de-analise/como-montar-o-modelo-da-multiplan/]guia da companhia] que lista as principais ferramentas para criar um modelo desse negócio. 

## MULT3

A Multiplan é uma empresa imobiliária full-service, que executa o planejamento, desenvolvimento, e administração, com foco em shoppings centers no Brasil. Até junho de 2019 a empresa detinha 19 shopping centers e dois conjuntos de torres comerciais. A Área Bruta Locável (ABL) total administrada é de quase 1 milhão de metros quadrados.

Os shopping centers da Multiplan possuem, somados, mais de 5.400 operações, que geram um tráfego anual estimado em 180 milhões de visitas.

A companhia também executa projetos multiuso, construindo, nas proximidades de seus shoppings, edifícios comerciais, prédios residenciais e hotéis. A estratégia busca gerar sinergias e fluxo de consumidores para os shoppings, ao mesmo tempo em que valoriza as regiões.

(source: [[https://www.infomoney.com.br/cotacoes/b3/acao/multiplan-mult3/] informoney])

## Artefatos 

### Avaliação de receitas

**Modelo IGP-DI**: A principal receita da empresa é a de locação de lojas, e o principal indexador da variação é o IGP-DI, usando dados abertos e séries temporais podemos criar um modelo de previsão dessa variação para os próximos 7 anos. Os contratos são, em geral de 5 anos, com revisão anual baseada no índice.

**Modelo IGP-M** similar ao anterior mas com um output diferente. O IGP-M é utilizado no alguuel de torres comerciais. Contratos em Geral tem 5 anos de duração, com a previsão de 7 anos

- Para ABL e taxa de ocupação usamos dados existentes visto que esses projetos são multianos.

### Despesas

Os custos também tem variação relativa à inflação e utilizam os mesmos modelos. A maioria das despesas também utiliza inflação e série temporal a exceçào de **provisão para Provisão para créditos de liquidação duvidosa que usa dados do BACEN para avaliar a série.

