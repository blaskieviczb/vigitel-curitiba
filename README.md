# Hábitos alimentares em Curitiba: análise de microdados do Vigitel

## Sobre o projeto

Este projeto analisa mudanças nos hábitos alimentares da população adulta de Curitiba entre 2006 e 2024, investigando tendências de consumo e diferenças relacionadas a sexo, idade e escolaridade.

A pesquisa combina análise quantitativa de dados com interpretação sociológica dos resultados.

## Base de dados

- **Fonte:** Vigitel — Ministério da Saúde.
- **Localidade:** Curitiba (PR).
- **População:** adultos com 18 anos ou mais.
- **Período:** 2006–2024, conforme a disponibilidade dos indicadores.
- **Amostra:** aproximadamente 31 mil registros de Curitiba.
- **Indicadores:** consumo de frutas, hortaliças, feijão, refrigerantes e alimentos ultraprocessados.

Os microdados e a documentação estão disponíveis no [portal oficial do Vigitel](https://svs.aids.gov.br/daent/cgdnt/vigitel/).

As prevalências foram calculadas utilizando os pesos amostrais disponibilizados na base.

## Metodologia

As análises foram desenvolvidas em Python e envolveram:

- Importação, limpeza e organização dos microdados.
- Cálculo de prevalências ponderadas.
- Análise exploratória e de séries temporais.
- Comparações por sexo, idade e escolaridade.
- Visualização de dados.
- Regressões lineares e logísticas exploratórias.

## Principais resultados

O consumo regular de frutas apresentou tendência de crescimento ao longo da série histórica, enquanto o consumo regular de refrigerantes diminuiu.

O consumo regular de feijão caiu de 64,4% em 2015 para 47,8% em 2016, uma redução de 16,6 pontos percentuais.

Foram identificadas diferenças entre faixas etárias: o consumo regular de frutas foi mais frequente entre adultos de faixas etárias mais avançadas, enquanto refrigerantes e alimentos ultraprocessados apresentaram maior consumo entre adultos jovens.

Os modelos estatísticos também identificaram associações entre hábitos alimentares, sexo, idade e escolaridade.

## Investigação sociológica

Além da análise estatística, o projeto investiga a queda do consumo de feijão em 2016 e as mudanças observadas durante a pandemia.

Os resultados são discutidos considerando o contexto econômico e as práticas alimentares, sem pressupor relações causais.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

## Estrutura do repositório

| Notebook | Descrição |
|---|---|
| [01_analise_vigitel_curitiba.ipynb](01_analise_vigitel_curitiba.ipynb) | Preparação dos dados, análise exploratória, indicadores, séries temporais e visualizações. |
| [02_investigacao_sociologica.ipynb](02_investigacao_sociologica.ipynb) | Investigação dos resultados, contextualização sociológica e modelos estatísticos. |

## Como reproduzir as análises

Os notebooks foram desenvolvidos no Google Colab, utilizando microdados armazenados no Google Drive.

Para executar as análises:

1. Acesse o [portal oficial do Vigitel](https://svs.aids.gov.br/daent/cgdnt/vigitel/) e obtenha os microdados em formato CSV.
2. Prepare uma base consolidada compatível com a utilizada no projeto, denominada `vigitel-2006-2024-peso-rake_slabel.csv`.
3. Armazene o arquivo no Google Drive.
4. Abra os notebooks no Google Colab e atualize o caminho definido na variável `arquivo_vigitel`.
5. Execute as células na sequência.

A base consolidada utilizada nas análises não está incluída neste repositório. Os arquivos disponibilizados pelo Ministério da Saúde podem exigir preparação e harmonização antes da execução dos notebooks.

## Limitações

As análises são observacionais e não permitem estabelecer relações causais. As séries consideram a disponibilidade e a comparabilidade dos indicadores ao longo do período.

Os modelos estatísticos têm caráter exploratório e não incorporam integralmente a estrutura amostral complexa do Vigitel.

## Autoria

**Bruna Stall Blaskievicz**

Mestre em Sociologia e Antropologia pela Universidade Federal do Rio de Janeiro (UFRJ) e pós-graduanda em Análise de Dados e Big Data pela Pontifícia Universidade Católica do Paraná (PUC-PR).
