<h1 align ="center"> Majestic Exportadora </h1>

Este projeto foi elaborado como parte do curso "Master DAX - Power BI orientado a projetos", ministrado por Felipe Mafra. O curso tem como principal objetivo proporcionar uma experiência prática ao longo de todo o processo, permitindo construir um projeto do zero. Durante o curso, são exploradas as funções mais comuns em DAX, assim como os cálculos típicos realizados por um analista de dados no dia a dia.

Para desenvolver este projeto, foram utilizados dados fictícios de uma empresa exportadora de materiais escolares. Através desta iniciativa, foi possível analisar diversos aspectos do negócio, incluindo seu faturamento, custos, margem de lucro, receita líquida e ticket médio. Além disso, foram explorados indicadores de crescimento ao longo do tempo, tanto a nível de país quanto de continente. O projeto também possibilitou a identificação de padrões, variações e a realização de simulações para prever possíveis impactos e embasar decisões futuras em contexto dinâmico.

Para visualização em web: https://shorturl.at/cvW15 

<h3> Destaco abaixo alguns dos aprendizados e informações importantes: </h3>

<h3>Layout</h3>

- Destaco a utilização de Tooltip (dica de ferramenta do Power BI) no gráfico de "Venda Bruta por Categoria" na página de Análise Geral, com o intuito de detalhar algumas informações gráficas. Sendo bastante útil para economizar espaço, principalmente quando não é possível colocar maiores detalhamentos em um único gráfico ou sua representação não ficaria visualmente agradável e legível. 
- Foram importados os seguintes visuais para uso em layout por meio do Power BI Visuals: Sparkline by OKViz, Image Grid, Advance Card, Simple Image, Brick Chart by MAQ Software e radarChart. Importar visuais são interessantes para experimentar em estudos e criar narrativas diferentes, porém não recomendo utilizar em contextos profissionais. A manutenção desses visuais acabam sendo complexas para o desenvolvedor, além de existir a possibilidade de ficarem indisponíveis para importação na loja, gerando uma quebra na visualização de alguns dados. Por isso, em um projeto real, recomendo utilizar visuais padrões do PBI.
- Alguns nomes de tabela e títulos das páginas foram criadas em DAX a fim de tornar a manutenção mais rápida e prática. Recurso útil para nomes de tabela que se repetem, nomes de KPIs, avisos padronizados, etc. Uma vez a legenda / texto alterado por dax, todas as páginas que utilizam essa medida serão afetadas. Nesse sentido economizaria tempo, podendo ser reaproveitados ganhando maior de agilidade para manutenção.
- Utilização de URL para importar imagens para os meus visuais, como imagens de países no gráfico "Receita por País" na página de Análise Geral. É importante deixar essas imagens em ambiente seguro e que não será alterado, para que não haja quebra de visualização caso aquela url não exista.

<h3>DAX</h3>

- Uso de variáveis dentro de medidas utilizando convenções a fim de padronização, além de possibilitar maior otimização e redução de linhas de código. 
- Tabelas virtuais para análise de cross sell. As tabelas virtuais são úteis para agilizar cálculos e economizar espaço. 
- Utilização da função SWITCH() para classificações qualitativas de produto a partir do cálculo de receita líquida.
- Função CALCULATE() para cálculos dentro de contextos específicos, como margem de lucro (%) para o país top 1 da América do Sul.
- Função USERELATIONSHIP() para criar relacionamento entre tabelas que inicialmente não tinham um relacionamento no modelo de dados, a fim de criar novos insights.
- Função SAMEPERIODLASTYEAR() para buscar indicador relativo ao mesmo período do ano anterior.Além do uso de DATEADD() para também buscar vendas do ano anterior de forma dinâmica.
