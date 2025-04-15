# 🚴 Análise de Dados: Sistema de Bike Sharing

## 📌 Visão Geral do Projeto
Este projeto de análise de dados explora padrões de demanda em um sistema de compartilhamento de bicicletas, fornecendo insights valiosos para tomada de decisão estratégica. Através de técnicas de ETL, modelagem de dados e análise exploratória, identificamos fatores-chave que influenciam o comportamento dos usuários.

## 🎯 Objetivos Principais
- Analisar o impacto da sazonalidade no volume de aluguéis
- Investigar a influência das condições meteorológicas na demanda
- Comparar padrões de uso entre usuários casuais e registrados
- Identificar horários de pico e variações diárias/semanais
- Fornecer recomendações acionáveis baseadas em dados

## 📊 Principais Insights
**🌦️ Impacto do Clima**

- Dias claros: 40% mais aluguéis que dias chuvosos/nevados
- Neblina: reduz demanda em 25% comparado a dias claros

**📅 Sazonalidade**

- **Verão:** 35% do total de aluguéis (pico de demanda)
- **Inverno:** 15% do total (menor demanda)
## ⏰ Padrões Temporais

- **Dias úteis:** Picos às 8h e 17h-18h (deslocamento)
- **Fins de semana:** Pico ao meio-dia (uso recreativo)
## 🌡️ Fatores Ambientais

- Correlação de 0.75 entre temperatura e número de aluguéis
## 🛠️ Tecnologias Utilizadas
- **Plataforma:**	Databricks
- **Linguagens:**	SQL, Python
- **Visualização:**	Matplotlib, Seaborn,
Processamento	ETL, Modelagem de Dados,
Versionamento	Git e GitHub
## 📂 Estrutura do Projeto
**Base de Dados**
- **Origem:** /databricks-datasets/bikeSharing/
- **Arquivos principais:** day.csv e hour.csv

**Modelagem de Dados**

**Tabelas SQL criadas:**

- dados_dia (16 atributos)

- dados_hora (17 atributos)

**Catálogo de dados documentado**
- **Processamento (ETL)**

- **Criação da tabela diária:**

CREATE TABLE dados_dia AS

SELECT * FROM bikeSharing.day;

- **Criação da tabela horária:**

CREATE TABLE dados_hora AS

SELECT *, HOUR(dteday) as hora FROM bikeSharing.hour;

**Análise Exploratória**

- Consultas SQL para agregações
- Visualizações com Python
- Identificação de padrões e tendências

## 📈 Principais Resultados
**Recomendações Operacionais**

- Ajustar frota conforme previsão do tempo e estações
- Campanhas promocionais no inverno/dias chuvosos
- Aumentar disponibilidade nos horários de pico
- Estratégias de Marketing
- Incentivos para uso recreativo nos fins de semana
- Parcerias com pontos turísticos e empresas locais
- Melhorias de Infraestrutura
- Proteção contra condições climáticas adversas
- Otimização da distribuição das estações

## 🚀 Como Reproduzir o Projeto

**Clone o repositório:**

git clone https://github.com/brunosuassuna/MVP-Engenharia-de-Dados

**Acesse o Databricks e importe os datasets:**

/FileStore/tables/aula-databricks/projeto_final/bikeSharing/

- Execute os scripts de ETL e análise disponíveis

- Explore as visualizações e relatórios gerados

## 💡 Habilidades Demonstradas
✅ Engenharia de Dados (ETL, modelagem)

✅ Análise Exploratória (SQL, Python)

✅ Visualização de Dados e Storytelling

✅ Solução de Problemas Baseada em Dados

✅ Documentação Técnica

## 📬 Contato

- **Email:** brunosuassuna.dev@gmail.com

- **LinkedIn:** www.linkedin.com/in/bruno-suassuna-698aa7235

**Licença:** [MIT](https://opensource.org/license/MIT)
