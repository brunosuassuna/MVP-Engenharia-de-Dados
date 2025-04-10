# Autoavaliação do Projeto Bike Sharing

## 1. Objetivos e Resultados
O projeto teve como meta principal analisar padrões de demanda no sistema de compartilhamento de bicicletas, com foco em:
- **Padrões temporais**: Variação de aluguéis por horário, dia da semana e estação do ano.
- **Fatores externos:** Impacto de clima, temperatura e umidade na demanda.
- **Segmentação de usuários:** Comparação entre usuários casuais e registrados.
- **Visualização de dados:** Criação de dashboards claros para tomada de decisões.
  ### Resultados Alcançados:
- **Demanda sazonal:** Picos de aluguel em dias úteis (8h e 17h) para usuários registrados e fins de semana para casuais.
- **Influência climática:** Temperaturas acima de 20°C e condições de céu claro aumentam a demanda em até 40%.
- **Visualizações eficazes:** Gráficos de dispersão (temperatura vs. demanda) e heatmaps (uso por horário) destacaram correlações-chave.

## 2. Desafios e Soluções
### 2.1 Limitações dos Dados
- **Problema:** Dados agregados (não individuais) e falta de informações externas (eventos, tráfego).
- **Solução:** Otimização das análises com os dados disponíveis, usando agregações por hora e métricas derivadas (ex.: "sensação térmica").
### 2.2 Dificuldades Técnicas
- **Ferramentas:** Curva de aprendizado no Databricks para manipulação de tabelas e SQL.
- **Visualização:** Desafio na criação de gráficos multivariados no Matplotlib/Seaborn.
- **Ação:** Documentação de códigos e testes iterativos para garantir precisão.
### 2.3 Restrições de Tempo
Escopo inicial priorizado, postergando modelos preditivos para futuras iterações.

## 3. Melhorias Propostas
### 3.1 Aprimoramentos Analíticos
- **Modelos preditivos:** Regressão para prever demanda com base em histórico climático.
- **Análise geoespacial:** Mapeamento de rotas populares com integração a APIs de geolocalização.
- **Dados em tempo real:** Pipeline com Kafka ou AWS Kinesis para monitoramento dinâmico.
## 3.2 Avanços Técnicos
- **Automação:** Pipeline de ETL (Airflow ou Luigi) para atualização diária dos dados.
- **Dashboard interativo:** Implementação com Power BI ou Metabase para visualização em tempo real.
## 3.3 Expansão do Escopo
- **Integração multimodal:** Cruzamento com dados de transporte público (ônibus, metrô).
- **Campanhas de marketing:** Análise de ROI para promoções direcionadas a usuários casuais.

## 4. Conclusão
O projeto consolidou habilidades críticas em engenharia e análise de dados, desde a limpeza de dados até a comunicação de insights. As limitações identificadas reforçam a importância de um planejamento robusto de coleta de dados, enquanto as sugestões de melhoria abrem oportunidades para:
Aplicação de machine learning.
Maior escalabilidade com ferramentas de cloud (AWS/GCP).
Impacto direto na operação do negócio (ex.: reposição estratégica de bicicletas).

