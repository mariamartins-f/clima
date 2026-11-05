# Análise Exploratória de Dados (EDA) do Clima

Análise exploratória de um dataset de observações meteorológicas horárias, feita em Python com pandas. O projeto reúne exercícios de inspeção, filtragem, agregação e estatística descritiva.

## Dados

- Arquivo: `clima.csv`
- Tamanho: 8784 linhas e 8 colunas, sem valores nulos
- Período: observações horárias a partir de 01/01/2012
- Colunas:
  - `Date/Time`: data e hora da observação
  - `Temp_C`: temperatura (°C)
  - `Dew Point Temp_C`: ponto de orvalho (°C)
  - `Rel Hum_%`: umidade relativa (%)
  - `Wind Speed_km/h`: velocidade do vento (km/h)
  - `Visibility_km`: visibilidade (km)
  - `Press_kPa`: pressão atmosférica (kPa)
  - `Weather`: condição do tempo (50 categorias, como Fog e Clear)

## Estrutura

- `clima.ipynb`: notebook com a análise
- `clima.csv`: dataset
- `README.md`: documentação

## O que é feito no notebook

Inspeção inicial do dataset:

- `head`, `shape`, `index`, `columns`, `dtypes` e `info`
- `unique`, `nunique`, `count` e `value_counts`

Perguntas respondidas:

1. Valores únicos de velocidade do vento (34 valores distintos).
2. Quantas vezes o tempo foi exatamente "Clear" (1326 registros).
3. Quantas vezes a velocidade do vento foi exatamente 4 km/h (474 registros).
4. Identificação de valores nulos com `isnull` e `notnull`.
5. Renomear a coluna `Weather` para `Weather Condition`.
6. Visibilidade média (27.66 km).
7. Desvio padrão da pressão (0.84 kPa).
8. Variância da umidade relativa (286.25).
9. Registros com neve (`Snow`).
10. Registros com vento acima de 24 km/h e visibilidade de 25 km.
11. Média de cada coluna por condição do tempo, com `groupby`.
12. Mínimo e máximo de cada coluna por condição do tempo.
13. Registros com neblina (`Fog`).
14. Registros com tempo "Clear" ou visibilidade acima de 40 km.
15. Registros com ("Clear" e umidade acima de 50%) ou visibilidade acima de 40 km.

## Como executar

1. Clone o repositório: `git clone https://github.com/mariamartins-f/NOME_DO_REPOSITORIO.git`
2. Instale as dependências: `pip install pandas jupyter`
3. Abra o notebook: `jupyter notebook clima.ipynb`
4. Ajuste o caminho do `pd.read_csv` para o local do `clima.csv` no seu computador.

## Tecnologias

Python, pandas e Jupyter Notebook.

## Autora

Maria Martins — [@mariamartins-f](https://github.com/mariamartins-f)
