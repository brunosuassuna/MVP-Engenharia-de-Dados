📊 Projeto de Análise de Dados: Sistema de Bike Sharing
GitHub: https://github.com/brunosuassuna/MVP-Engenharia-de-Dados

🎯 Objetivos
Este projeto analisou padrões de demanda em um sistema de compartilhamento de bicicletas para apoiar decisões estratégicas, com foco em:

Sazonalidade: Impacto das estações do ano no volume de aluguéis.

Clima: Influência de condições meteorológicas (temperatura, umidade, clima).

Comportamento dos usuários: Diferenças entre usuários casuais e registrados.

Horários de pico: Variação da demanda ao longo do dia e da semana.

📂 Metodologia
🔍 Coleta e Modelagem dos Dados
Fontes: Datasets day.csv e hour.csv do diretório /databricks-datasets/bikeSharing/ no Databricks.

Modelagem: Criação de tabelas SQL (dados_dia e dados_hora) com documentação detalhada (Catálogo de Dados).

ETL: Processo de carga via queries (ex.: CREATE TABLE dados_dia AS SELECT * FROM bikeSharing.day).

📊 Análise Exploratória
Ferramentas: SQL (agregações), Python (Matplotlib/Seaborn) para visualizações.

Abordagem:

Correlação entre temperatura e demanda.

Distribuição de aluguéis por estação, dia da semana e horário.

Comparação entre usuários casuais e registrados.

📌 Resultados Principais
Análise	Insights	Recomendações
Sazonalidade	Verão: 35% do total de aluguéis; Inverno: 15%.	Campanhas promocionais no inverno para equilibrar demanda.
Clima	Dias claros tiveram 40% mais aluguéis que dias chuvosos.	Ajustar frota com base em previsões meteorológicas.
Horários de Pico	Dias úteis: 8h e 17h (deslocamento); Fins de semana: 12h (lazer).	Aumentar disponibilidade nos horários críticos.
Temperatura vs. Demanda	Correlação positiva (0.75): maior demanda em temperaturas amenas (20-25°C).	Expandir frota em estações quentes.
Usuários Casuais x Registrados	Registrados predominam em dias úteis; casuais em fins de semana.	Parcerias com atrações turísticas para incentivar uso recreativo.
🛠 Tecnologias Utilizadas
Plataforma: Databricks (processamento e análise).

Linguagens: SQL (modelagem), Python (análise).

Visualização: Matplotlib, Seaborn (gráficos de dispersão, heatmaps, barras).

✅ Conclusões e Trabalhos Futuros
Conclusões:

Demanda é altamente influenciada por clima e fatores temporais.

Oportunidades para otimizar frota e campanhas de marketing.

Melhorias Propostas:

Modelos Preditivos: Prever demanda com machine learning.

Dashboard Interativo: Power BI/Tableau para monitoramento em tempo real.

Dados Externos: Integrar eventos locais ou dados de tráfego.

📥 Reprodução do Projeto
Clone o repositório:

git clone https://github.com/brunosuassuna/MVP-Engenharia-de-Dados

Acesse o Databricks e importe os datasets:

/FileStore/tables/aula-databricks/projeto_final/bikeSharing/

Execute os scripts de ETL e análise (disponíveis no repo).

🔎 Autoavaliação e Desafios
1. Limitações na Granularidade dos Dados

Problema: Dados apenas em nível agregado (diário/horário) limitavam análises mais profundas de padrões individuais.

Solução: Criei métricas derivadas como:

"Demanda Relativa" (aluguéis/hora ÷ média histórica)

"Sensação Térmica Efetiva" (combinação de temperatura + umidade)

Segmentação por faixas de uso (leve/moderado/intenso)

2. Complexidade na Visualização de Dados Multidimensionais

Desafio: Representar simultaneamente clima, temperatura e demanda temporal.

Inovações:

Gráficos de calor 3D (hora × dia × demanda)

Mapas de correlação interativos com Plotly

FacetGrids no Seaborn para comparação entre grupos

3. Adaptação ao Ecossistema Databricks

Dificuldades:

Gerenciamento de sessões Spark

Otimização de queries SQL em grandes datasets

Conquistas:

Redução de 40% no tempo de processamento após ajuste de partições

Documentação de boilerplates para operações recorrentes

📈 Evolução de Habilidades
Competências Desenvolvidas
✔ Engenharia de Dados:

Projeto de modelagem dimensional para dados temporais

Técnicas de qualidade de dados (validação de faixas, tratamento de outliers)

✔ Análise

Cálculo avançado de métricas (elasticidade demanda-clima)

Análise de sazonalidade com decomposição temporal

✔ Visualização

Princípios de design para dashboards (hierarquia visual, teoria das cores)

Storytelling com dados para diferentes stakeholders

🚀 Lições Aprendidas
Valor da Documentação

Mantive um log detalhado de todas as decisões de análise

Criei um dicionário de dados com metadados enriquecidos

Pensamento Crítico em Análise

Aprendi a diferenciar correlação de causalidade

Implementei testes de hipóteses para validar insights

Gestão de Trade-offs

Balanceamento entre profundidade analítica e prazos

Priorização de features com maior impacto nos resultados
