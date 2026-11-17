# Matheus Cardoso Rodrigues

**Desenvolvedor Python & Dados · Saúde Pública**

Construo painéis de vigilância epidemiológica sobre as bases do SUS (SINAN, SIM, IBGE) no **Cenários / NESP-UnB**, o Núcleo de Estudos em Saúde Pública da Universidade de Brasília. Os painéis abaixo estão no ar e são usados por secretarias de saúde e equipes de pesquisa.

Curso Análise e Desenvolvimento de Sistemas na **UDF** e venho da infraestrutura de TI. Por isso cuido do que acontece depois do `git push`: build reprodutível, dependências travadas, CI e documentação.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mcardosor)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:matheuscardoso21@gmail.com)

---

### 📊 Painéis em produção

O código está na organização [**Dev-Cenarios**](https://github.com/Dev-Cenarios), aberto, sob licença MIT. Cada repositório traz a metodologia de cada número, o contrato de dados e o botão "Cite this repository".

| Painel | O que mostra | Stack | |
|---|---|---|---|
| [**Tuberculose · Brasil**](https://github.com/Dev-Cenarios/painel-tuberculose-brasil) | Incidência, mortalidade e cura nos 5.570 municípios, com mapa por estado e por município, na régua oficial do Ministério da Saúde. | Streamlit · DuckDB · deck.gl · ECharts · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/tbbrasil/) |
| [**Tuberculose · Pernambuco**](https://github.com/Dev-Cenarios/painel-tuberculose-pernambuco) | Vigilância da TB nos 185 municípios de PE desde 2010, por região e macrorregião de saúde: incidência, cura, abandono, óbito e coinfecção HIV, com mapa clicável e canal endêmico. | Streamlit · DuckDB · deck.gl · ECharts · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/tbpe/) |
| [**Tuberculose · Recife**](https://github.com/Dev-Cenarios/painel-tuberculose-recife) | Os oito indicadores do Boletim Epidemiológico do MS por bairro e Distrito Sanitário. Entregue também como imagem Docker com os dados dentro, sem nenhum identificador. | Streamlit · DuckDB · deck.gl · ECharts · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/tbrecife/) |
| [**Tuberculose · Distrito Federal**](https://github.com/Dev-Cenarios/painel-tuberculose-df) | Mapa por Região Administrativa, a partir de uma fonte nominal da qual os identificadores são descartados na extração; números contados como no Boletim da SES-DF. | Streamlit · DuckDB · deck.gl · ECharts · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/dftb/) |
| [**Hanseníase · Brasil**](https://github.com/Dev-Cenarios/painel-hanseniase-brasil) | Do Brasil ao município: detecção geral e em menores de 15 anos, grau II, cura e contatos nas coortes, com os parâmetros do Boletim do MS. | Streamlit · DuckDB · deck.gl · ECharts · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/hansebr/) |
| [**Hanseníase · Pernambuco**](https://github.com/Dev-Cenarios/painel-hanseniase-pernambuco) | Detecção, grau II e qualidade do programa por município, região e macrorregião, conferidos município a município contra o boletim estadual. | Streamlit · DuckDB · deck.gl · ECharts · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/hansepe/) |
| [**Hanseníase · Distrito Federal**](https://github.com/Dev-Cenarios/painel-hanseniase-df) | Detecção, grau II, cura e contatos, com mapa por Região Administrativa e os parâmetros do boletim da SES-DF. | Streamlit · DuckDB · deck.gl · ECharts · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/hansedf/) |
| [**Envelhecimento · Brasil**](https://github.com/Dev-Cenarios/painel-envelhecimento-brasil) | Pessoas com 60+ por estado a partir das Projeções do IBGE (rev. 2024): estimativas de 2000 a 2022 e projeções até 2070, separadas na tela. | Streamlit · Pandas · Plotly · pydeck · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/demografico-longevidade/) |
| [**Demográfico · Brasil**](https://github.com/Dev-Cenarios/painel-demografico-brasil) | A população por estado e município (2010–2025): pirâmide etária comparando anos, crescimento, densidade, nascimentos e fecundidade (SINASC) e esperança de vida, com mapa clicável até o município. | Streamlit · DuckDB · deck.gl · ECharts · Docker | [ao vivo](https://painel.cenarios.unb.br/cenarios/demografico/) |

**Como os painéis são mantidos**

- 📐 Documentação de metodologia: de onde vem cada número e como cada indicador é calculado
- 🔒 `requirements.txt` (intenção) separado de `requirements.lock.txt` (o que roda), resolvido dentro da imagem de produção
- ⚙️ CI no GitHub Actions a cada push: `ruff`, testes com `pytest`, build da imagem Docker e conferência do lock contra o container
- 🐳 Deploy em container, com as mesmas versões no build e em produção
- 🧪 Paridade testada: os números são conferidos contra os boletins oficiais, e toda divergência fica registrada com o motivo

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
