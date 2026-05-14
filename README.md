# SaúdeBR — Painel de Inteligência da Saúde Pública Brasileira

[![Power BI](https://img.shields.io/badge/Visualização-Power%20BI-yellow)](https://app.powerbi.com/view?r=eyJrIjoiN2E0OGUzOTYtZTc4Mi00ZGIyLTg1NmUtOTBmNzU2MTk0YWVlIiwidCI6ImY5OTZjZmRiLTQyYWMtNGVhZC1iYzQzLThmZmY3Njc0Zjg4NiIsImMiOjR9)
[![PostgreSQL](https://img.shields.io/badge/Banco-PostgreSQL%20(Neon)-blue)](https://neon.tech/)
[![Python](https://img.shields.io/badge/ETL-Python-green)](https://www.python.org/)

## 📌 Sobre o Projeto
O **SaúdeBR** é uma solução completa de dados que transforma os microdados complexos do **DATASUS** em inteligência estratégica. O projeto abrange desde a extração e limpeza de dados públicos até a modelagem em banco de dados e visualização analítica.

> **Acesse o Painel Interativo aqui:** [Link do Relatório Power BI](https://app.powerbi.com/view?r=eyJrIjoiN2E0OGUzOTYtZTc4Mi00ZGIyLTg1NmUtOTBmNzU2MTk0YWVlIiwidCI6ImY5OTZjZmRiLTQyYWMtNGVhZC1iYzQzLThmZmY3Njc0Zjg4NiIsImMiOjR9)

## 📸 Visualização do Painel

### 1. Panorama de Internações (SIH/SUS)
Análise de volume de internações com visão temporal e distribuição geográfica por UF.
![Dashboard Página 1]("C:\Users\joaop\Downloads\Captura de tela 2026-05-14 161601.png")

### 2. Análise de Mortalidade (SIM)
Monitoramento epidemiológico de óbitos por local de residência e evolução anual.
![Dashboard Página 2]("C:\Users\joaop\Downloads\Captura de tela 2026-05-14 161638.png")

### 3. Capacidade Hospitalar (CNES)
Visão crítica de oferta de leitos SUS vs Privados, identificando municípios abaixo da meta recomendada.
![Dashboard Página 3]("C:\Users\joaop\Downloads\Captura de tela 2026-05-14 161653.png")

## 🛠️ Tecnologias e Arquitetura
*   **Extração & ETL:** Python (Pandas, SQLAlchemy) para consumo de dados do DATASUS e limpeza de inconsistências geográficas.
*   **Banco de Dados:** PostgreSQL hospedado na nuvem (**Neon**) utilizando modelagem **Star Schema**.
*   **Business Intelligence:** Power BI Desktop com medidas em **DAX** para taxas epidemiológicas e mapas coropléticos.

## 🚀 Como Executar o Pipeline
1. Configure as variáveis de ambiente com sua connection string do PostgreSQL.
2. Execute o script `etl_unificado.py` na pasta `/carga` para processar os dados brutos.
3. Abra o arquivo `.pbix` e atualize a fonte de dados para o seu banco.

---
*Projeto desenvolvido para demonstrar competências em Engenharia de Dados e Business Intelligence aplicados ao setor público.*
