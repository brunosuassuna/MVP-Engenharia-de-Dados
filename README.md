📊 Projeto de Análise de Dados: Sistema de Bike Sharing
GitHub: https://github.com/brunosuassuna/MVP-Engenharia-de-Dados

📖 Descrição do Projeto

Este projeto tem como objetivo analisar o comportamento dos aluguéis de bicicletas em um sistema de compartilhamento, identificando padrões e tendências para apoiar a tomada de decisões estratégicas.

🎯 Objetivos

Este projeto analisou padrões de demanda em um sistema de compartilhamento de bicicletas para apoiar decisões estratégicas, com foco em:

Sazonalidade: Impacto das estações do ano no volume de aluguéis.

Clima: Influência de condições meteorológicas (temperatura, umidade, clima).

Comportamento dos usuários: Diferenças entre usuários casuais e registrados.

Horários de pico: Variação da demanda ao longo do dia e da semana.

📂 1. Metodologia

📥 1.1. Coleta dos Dados

Os dados foram obtidos do diretório /databricks-datasets/bikeSharing/ no Databricks.

Conjunto de dados utilizado:

day.csv: Dados agregados por dia.

hour.csv: Dados agregados por hora.

Os arquivos foram copiados para /FileStore/tables/aula-databricks/projeto_final/bikeSharing/ para reprodutibilidade.

📑 1.2. Modelagem dos Dados Foram criadas duas tabelas no banco de dados SQL:

dados_dia: Dados agregados por dia (16 atributos).

dados_hora: Dados agregados por hora (17 atributos, incluindo a hora do dia).

Um Catálogo de Dados foi elaborado para documentar os atributos, tipos de dados e descrições de cada coluna.

🔄 1.3. Carga dos Dados

Utilização de ETL (Extração, Transformação e Carga) para inserir os dados nas tabelas SQL.

Exemplo de comando de carga:

CREATE TABLE dados_dia AS

SELECT * FROM bikeSharing.day;

🔍 1.4. Análise dos Dados Foram conduzidas análises exploratórias para responder às perguntas-chave do projeto:

✔ Sazonalidade: Distribuição de aluguéis por estação do ano.

✔ Impacto do clima: Influência das condições climáticas na demanda.

✔ Horários de pico: Padrões de uso ao longo do dia.

✔ Dias úteis vs. fins de semana: Diferença no comportamento dos usuários.

Ferramentas utilizadas:

SQL para agregações e consultas.

Python (Matplotlib, Seaborn) para visualizações gráficas.

📊 2. Resultados e Discussões

🍂 2.1. Sazonalidade - Total de Aluguéis por Estação

Verão: Maior volume (35% do total).

Inverno: Menor volume (15%). 📌 Implicação: Desenvolver campanhas promocionais no inverno para estimular a demanda.

☁️ 2.2. Impacto do Clima nos Aluguéis

Dias claros tiveram 40% mais aluguéis que dias chuvosos ou com neve.

📌 Implicação: Ajustar a frota com base nas previsões meteorológicas.

⏰ 2.3. Horários de Pico

Dias úteis: 8h e 17h-18h (horários de deslocamento para o trabalho).

Fins de semana: 12h (uso recreativo).

📌 Implicação: Aumentar a disponibilidade de bicicletas nos horários de pico.

📅 2.4. Dias Úteis vs. Finais de Semana

Dias úteis tiveram 60% mais aluguéis que os fins de semana.

📌 Implicação: Criar incentivos para aumentar o uso recreativo (parcerias com pontos turísticos).

🌡️ 2.5. Relação entre Temperatura e Aluguéis

Correlação positiva (coeficiente de 0,75) entre temperatura e número de aluguéis.

📌 Implicação: Ajustar a frota conforme a estação do ano.

✅ 3. Conclusão e Recomendações

✔️ Ajustar a frota de bicicletas conforme estação do ano, clima e horários de pico.

✔️ Criar campanhas promocionais para períodos de baixa demanda (inverno, dias chuvosos).

✔️ Investir em infraestrutura para melhorar a experiência do usuário em condições climáticas adversas.

✔️ Estabelecer parcerias estratégicas para incentivar o uso recreativo das bicicletas.

🛠 4. Tecnologias Utilizadas

Tecnologia Uso

Databricks Plataforma de análise de dados

SQL Modelagem e consultas

Python Análises e visualizações

Matplotlib/Seaborn Gráficos e insights visuais

📌 5. Como Reproduzir o Projeto

Clone este repositório:

git clone https://github.com/brunosuassuna/MVP-Engenharia-de-Dados

Acesse o Databricks e copie os arquivos do diretório:

/FileStore/tables/aula-databricks/projeto_final/bikeSharing/

Importe os arquivos .csv para um banco de dados SQL.

Execute os scripts de ETL e análise disponíveis no repositório.
