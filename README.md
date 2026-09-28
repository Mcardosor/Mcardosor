# Matheus Cardoso Rodrigues

**Desenvolvedor Python & Dados · Saúde Pública**

Construo painéis de vigilância epidemiológica sobre as bases do SUS (SINAN, SIM, IBGE) no **Cenários / NESP-UnB**, o Núcleo de Estudos em Saúde Pública da Universidade de Brasília. Os painéis abaixo estão no ar e são usados por secretarias de saúde e equipes de pesquisa.

Curso Análise e Desenvolvimento de Sistemas na **UDF** e venho da infraestrutura de TI. Por isso cuido do que acontece depois do `git push`: build reprodutível, dependências travadas, CI e documentação.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/matheus-cardoso-637a1b145)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:matheuscardoso21@gmail.com)

---

### 📊 Painéis em produção

| Painel | O que mostra | Stack | |
|---|---|---|---|
| [**Tuberculose · Pernambuco**](https://github.com/Mcardosor/Tuberculose_Pernambuco) | Vigilância da TB nos 185 municípios de PE desde 2010, com recorte por região e macrorregião de saúde: incidência, cura, abandono, óbito e coinfecção HIV, com mapa clicável e canal endêmico. | Streamlit · DuckDB · deck.gl · ECharts · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/tbpe/) |
| [**Longevidade · Brasil**](https://github.com/Mcardosor/dashboard-demografico-longevidade) | Envelhecimento da população por UF a partir das Projeções do IBGE (rev. 2024): estimativas de 2000 a 2022 e projeções até 2070, separadas na tela. | Streamlit · Pandas · Plotly · Parquet · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/demografico-longevidade) |
| [**Demográfico · Brasil**](https://github.com/Mcardosor/dashboard-demografico) | Distribuição etária por estado (2010–2025): mapa coroplético, pirâmide etária, ranking e KPIs com comparativo anual. | Streamlit · Pandas · Plotly · Parquet · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/demografico) |

**Também no ar, com código em repositório privado:** [Hanseníase · Pernambuco](https://painel.cenarios.unb.br/cenarios/hansepe) · [Tuberculose · Recife](https://painel.cenarios.unb.br/cenarios/tbrecife)

**Como os painéis são mantidos**

- 📐 Documentação de metodologia: de onde vem cada número e como cada indicador é calculado
- 🔒 `requirements.txt` (intenção) separado de `requirements.lock.txt` (o que roda), resolvido dentro da imagem de produção
- ⚙️ CI no GitHub Actions a cada push: `ruff`, build da imagem Docker e conferência do lock contra o container
- 🐳 Deploy em container, com as mesmas versões no build e em produção

---

### 🛠️ Stack

**Dados**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Parquet](https://img.shields.io/badge/Parquet-50ABF1?style=flat-square&logo=apacheparquet&logoColor=white)

**Visualização**
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![ECharts](https://img.shields.io/badge/ECharts-AA344D?style=flat-square&logo=apacheecharts&logoColor=white)
![deck.gl](https://img.shields.io/badge/deck.gl-1C1C1C?style=flat-square&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)

**Infra & Entrega**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Ruff](https://img.shields.io/badge/Ruff-D7FF64?style=flat-square&logo=ruff&logoColor=black)

Também trabalho com Power BI, SQL Server, MySQL, n8n e Google Cloud.

---

### 🩺 Dados com que trabalho

**SINAN** (notificação de agravos) · **SIM** (mortalidade) · **IBGE** (projeções populacionais): limpeza, vinculação entre bases, geocodificação e cálculo de indicadores epidemiológicos, sempre conferidos contra os números oficiais do Ministério da Saúde.

---

📍 Brasília, DF · Aberto a colaborações acadêmicas e projetos de dados
