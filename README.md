# MVP-Engenharia-de-Dados


MVP - Sprint: Engenharia de Dados 
Documentação do Projeto Bike Sharing

1. Documentação Detalhada do Processo e dos Resultados

1.1. Contexto e Objetivos do Projeto

O projeto tem como objetivo analisar o comportamento dos aluguéis de bicicletas em um sistema de compartilhamento, com foco em identificar padrões e tendências que possam auxiliar na tomada de decisões estratégicas. Os principais objetivos são:
Entender a sazonalidade: Como as estações do ano afetam o volume de aluguéis.
Avaliar o impacto do clima: Como as condições climáticas influenciam a demanda por bicicletas.
Identificar horários de pico: Quais são os períodos de maior demanda ao longo do dia.
Comparar dias úteis e fins de semana: Como o uso de bicicletas varia entre dias de trabalho e dias de lazer.

1.2. Metodologia

1.2.1. Coleta dos Dados

O dataset Bike Sharing foi selecionado por ser um conjunto de dados aberto, bem documentado e amplamente utilizado em análises de mobilidade urbana.
Os dados foram coletados do diretório /databricks-datasets/bikeSharing/ no Databricks, contendo dois arquivos principais:
day.csv: Dados agregados por dia.
hour.csv: Dados agregados por hora.
Os arquivos foram copiados para um diretório pessoal (/FileStore/tables/aula-databricks/projeto_final/bikeSharing/) para garantir a reprodutibilidade do projeto.

1.2.2. Modelagem dos Dados
Foram criadas duas tabelas no banco de dados SQL:
dados_dia: Contém dados agregados por dia, com 16 atributos.
dados_hora: Contém dados agregados por hora, com 17 atributos (incluindo a hora do dia).
O Catálogo de Dados foi elaborado para documentar os atributos, tipos de dados, descrições e domínios de cada coluna.

1.2.3. Carga dos Dados
Os dados foram carregados nas tabelas SQL utilizando comandos de ETL (Extração, Transformação e Carga).
Exemplo de carga para a tabela dados_dia:

1.2.4. Análise dos Dados

Foram realizadas análises exploratórias para responder às perguntas-chave do projeto:
Sazonalidade: Qual é o total de aluguéis por estação do ano?
Impacto do Clima: Como as condições climáticas afetam o número de aluguéis?
Horários de Pico: Quais são os horários de maior demanda ao longo do dia?
Dias Úteis vs. Fins de Semana: Como o uso de bicicletas varia entre dias de trabalho e dias de lazer?
As análises foram realizadas utilizando SQL para agregações e consultas, e bibliotecas Python (Matplotlib, Seaborn) para visualizações gráficas.

1.2.5. Resultados
Os resultados foram documentados em gráficos e tabelas, destacando:
O total de aluguéis por estação do ano.
A relação entre condições climáticas e volume de aluguéis.
Os horários de pico de demanda.
A comparação entre dias úteis e fins de semana/feriados.

2. Discussão Aprofundada Conectando as Análises aos Objetivos do Projeto

2.1. Sazonalidade: Total de Aluguéis por Estação do Ano

Resultado: O verão registrou o maior volume de aluguéis (35% do total), enquanto o inverno teve o menor volume (15%).
Discussão:
O aumento no verão pode ser atribuído ao clima mais favorável, que incentiva atividades ao ar livre.
No inverno, o clima frio e as condições adversas (neve, chuva) reduzem a demanda por bicicletas.
Implicação Estratégica: A empresa pode desenvolver campanhas promocionais no inverno, como descontos ou pacotes especiais, para estimular a demanda.

2.2. Impacto do Clima nos Aluguéis
Resultado: Dias com clima claro tiveram 40% mais aluguéis do que dias com chuva ou neve.
Discussão:
O clima é um fator crítico para o uso de bicicletas, pois afeta a segurança e o conforto dos usuários.
Implicação Estratégica: A empresa pode monitorar previsões do tempo e ajustar a disponibilidade de bicicletas conforme as condições climáticas, além de investir em infraestrutura para dias chuvosos (e.g., coberturas para bicicletas).

2.3. Horários de Pico de Aluguéis

Resultado: Os horários de pico foram às 8h e 17h-18h em dias úteis, e ao meio-dia em fins de semana.
Discussão: Os picos em dias úteis estão associados ao deslocamento para o trabalho, refletindo o uso de bicicletas como meio de transporte.
No fim de semana, o pico ao meio-dia indica o uso recreativo das bicicletas.
Implicação Estratégica: A empresa pode aumentar a disponibilidade de bicicletas nos horários de pico e oferecer promoções para aluguéis fora desses períodos, otimizando a utilização da frota.

2.4. Comparação entre Dias Úteis e Fins de Semana/Feriados

Resultado: Dias úteis tiveram 60% mais aluguéis do que fins de semana/feriados.
Discussão: O uso de bicicletas para deslocamento ao trabalho é mais consistente e previsível do que o uso recreativo.
Implicação Estratégica: A empresa pode desenvolver estratégias para aumentar o uso recreativo, como parcerias com pontos turísticos, eventos ou promoções para famílias.

2.5. Relação entre Temperatura e Aluguéis
Resultado: Há uma correlação positiva entre temperatura e número de aluguéis (coeficiente de correlação de 0,75).
Discussão: Temperaturas mais altas incentivam o uso de bicicletas, enquanto temperaturas baixas desencorajam.
Implicação Estratégica: A empresa pode ajustar a frota de bicicletas conforme a estação do ano e as previsões de temperatura, além de oferecer incentivos para aluguéis em dias mais frios.

Conclusão Geral e Recomendações:
O projeto alcançou seus objetivos ao identificar padrões e tendências no uso do sistema de compartilhamento de bicicletas. Os resultados fornecem insights valiosos para a empresa, como:
Ajustar a disponibilidade de bicicletas conforme a estação do ano, o clima e os horários de pico.
Desenvolver campanhas promocionais para estimular a demanda em períodos de baixa utilização (inverno, dias chuvosos, horários fora de pico).
Investir em infraestrutura para melhorar a experiência do usuário em condições climáticas adversas.
Fortalecer parcerias com pontos turísticos e eventos para aumentar o uso recreativo das bicicletas.

