# Rafael Gomide

Estudante de Ciência de Dados na UVV (ES) — 4º período.
Foco em análise exploratória, modelagem estatística e visualização de dados.
Interesse de pesquisa em análise de sobrevivência e métodos estatísticos aplicados.

## Stack

**Análise & Dados**
`Python` `pandas` `polars` `numpy` `SQL`

**Estatística & Machine Learning**
`statsmodels` `scikit-learn` `XGBoost` `scipy` `lifelines`

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

### 🧰 [DS Toolkit](https://github.com/RafaelGomide/DS_toolkit)

Módulo Python único com 66 funções cobrindo o ciclo inteiro de um projeto de dados: ingestão, ETL, EDA, gráficos, machine learning, estatística aplicada e análise de sobrevivência. Nasceu da camada repetitiva que eu reescrevia em todo projeto novo — arquivo com encoding errado, `"R$ 1.234,56"` virando número, escolha do teste estatístico, a mesma matriz de confusão.

**Decisão de projeto:** as funções não escondem a estatística, elas a explicitam. `comparar_grupos()` escolhe entre t de Welch, Mann-Whitney, ANOVA e Kruskal-Wallis conforme normalidade e número de grupos, e sempre reporta tamanho de efeito junto do p-valor. O merge avisa quando um `left join` multiplicou linhas silenciosamente; o Cox alerta quando há menos de 10 eventos por covariável; o teste A/B distingue "não significativo" de "amostra pequena demais para concluir".

- 7 seções, ~3.980 linhas · pré-processamento encapsulado em `ColumnTransformer` para eliminar vazamento de dados, inclusive dentro de cada fold
- Seção de sobrevivência: Kaplan-Meier, Nelson-Aalen, Cox PH com checagem de riscos proporcionais, Cox-LASSO para p >> n e previsão individual de S(t)
- Dados brasileiros por padrão: datas `dd/mm/aaaa`, vírgula decimal, encoding `latin-1` de sistema legado
- Docstring completa em cada função — incluindo *quando não usar* aquela abordagem

`Python` `pandas` `numpy` `scipy` `scikit-learn` `lifelines` `matplotlib` `seaborn`

## Formação

- 🎓 Bacharelado em Ciência de Dados — UVV (cursando)
- 📍 Espírito Santo, Brasil

## Contato

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rafael-gomide-ds/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:provisoria.rafa@gmail.com)
