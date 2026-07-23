# Rafael Gomide

Estudante de Ciência de Dados na UVV (ES) — 4º período.
Foco em análise exploratória, modelagem estatística e visualização de dados.
Interesse de pesquisa em análise de sobrevivência e métodos estatísticos aplicados.

## Stack

**Análise & Dados**
`Python` `pandas` `polars` `numpy` `SQL`

**Estatística & Machine Learning**
`statsmodels` `scikit-learn` `XGBoost`

**Geoespacial**
`geopandas` `Leaflet`

**Coleta & Pipelines**
`BeautifulSoup` `requests` `ETL` `ThreadPoolExecutor`

**Backend & Deploy**
`FastAPI` `Gradio` `Render` `Hugging Face Spaces`

**Visualização**
`matplotlib` `seaborn` `plotly`

**Ferramentas**
`Git` `Jupyter` `Google Colab`

## Projetos em destaque

### 🌊 [Análise do Mercado Imobiliário de Vila Velha](https://github.com/RafaelGomide/Capstone-Imoveis-Vila-Velha)

Aplicação full-stack de análise de preços de imóveis, do scraping ao deploy. Coleta anúncios de quatro portais, testa hipóteses sobre o que forma o preço, treina modelos de valor justo e de zonas de valorização, e serve tudo num mapa interativo com API.

**Achado central:** controlando área, tipo e número de cômodos, cada quilômetro de distância da orla se associa a uma queda de ~17% no preço (IC 95%: −20,8% a −13,6%). Três métodos independentes — correlação, regressão hedônica e clustering — convergem para o mesmo resultado.

- Regressão hedônica log-linear (`statsmodels`) para inferência · Gradient Boosting (`scikit-learn`) para predição
- KMeans (k=3) para zonas de valorização · 1.371 imóveis em 58 bairros
- Arquitetura em três camadas: ETL → modelagem → serviço (`FastAPI` + `Leaflet`)
- Limitações de amostragem documentadas explicitamente no README

`Python` `polars` `geopandas` `statsmodels` `scikit-learn` `FastAPI` `Leaflet`
🔗 [Aplicação no ar](https://imoveis-vila-velha.onrender.com) *(tier gratuito — a primeira carga pode levar ~50s)*

## Formação

- 🎓 Bacharelado em Ciência de Dados — UVV (cursando)
- 📍 Espírito Santo, Brasil

## Contato

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rafael-gomide-ds/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:provisoria.rafa@gmail.com)
