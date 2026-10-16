# Analise de explicabilidade para classificacao de risco fiscal

Projeto de Trabalho de Conclusao de Curso sobre explicabilidade de modelos de
classificacao de risco fiscal. O repositorio contem dados sinteticos, notebooks
de geracao, treinamento e avaliacao dos modelos, analises de explicabilidade,
experimentos de fidelidade e estabilidade, alem dos resultados produzidos.

## Estrutura

- `dados/`: conjunto fiscal sintetico completo, particoes de treino e teste e
  metadados das variaveis.
- `notebooks/`: notebooks numerados que documentam o fluxo experimental.
- `resultados/`: metricas, tabelas, graficos e modelos treinados.
- `requirements.txt`: dependencias Python do projeto.

## Como executar

No Windows, abra um terminal na pasta do projeto e execute:

```powershell
py -m venv env_tcc
.\env_tcc\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

Abra a pasta no VS Code ou inicie o Jupyter e execute os notebooks em ordem,
de `01_geracao_dados.ipynb` a `05_estabilidade.ipynb`. Se necessario, selecione
`env_tcc` como kernel Python. Os notebooks registram as etapas e os resultados
de cada experimento.

## Dados

Os dados deste repositorio sao sinteticos. As sete variaveis informativas, as
tres variaveis de ruido e o alvo `risco_fiscal` estao descritos em
`dados/metadados.json`; nao sao dados reais de contribuintes.
