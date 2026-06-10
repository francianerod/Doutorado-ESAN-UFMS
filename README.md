# Doutorado-ESAN-UFMS
# Classificação da Estiagem na Sojicultura com Machine Learning: uma abordagem aplicada à região de Dourados/MS

Repositório contendo os códigos desenvolvidos durante a pesquisa de doutorado:

**RODRIGUES, F. Classificação da Estiagem na Sojicultura com Machine Learning: uma abordagem aplicada à região de Dourados/MS. 2025. 90 f. Tese (Doutorado em Administração) – Escola de Administração e Negócios, Universidade Federal de Mato Grosso do Sul (UFMS), Campo Grande, MS, 2025.**

---

## Sobre a Pesquisa

A estiagem é um dos principais fatores responsáveis pelas perdas de produtividade na cultura da soja. Apesar da ampla utilização de indicadores climáticos para monitoramento agrícola, ainda existem limitações na identificação de eventos de estiagem diretamente relacionados às necessidades hídricas da cultura.

Esta pesquisa teve como objetivo desenvolver e avaliar um modelo de Machine Learning capaz de classificar a ocorrência de estiagens na sojicultura em Dourados/MS, contribuindo para o monitoramento climático e fornecendo subsídios para a tomada de decisão por produtores, cooperativas e instituições públicas.

A pesquisa foi orientada pela seguinte questão:

> Como o desenvolvimento de um modelo de Machine Learning, baseado em um indicador específico de estiagem para a sojicultura, pode apoiar a classificação, o monitoramento contínuo e a mitigação dos impactos da estiagem em Dourados/MS?

---

## Principal Contribuição

O principal resultado da pesquisa foi a proposição do conceito de:

### Estiagem da Cultura da Soja

Um indicador agroclimático desenvolvido especificamente para a sojicultura, integrando os conceitos de estiagem e veranico em uma única métrica operacional.

O indicador foi construído a partir de:

* Séries históricas meteorológicas de Dourados/MS;
* Precipitação acumulada em janelas móveis de cinco dias;
* Análises estatísticas e climatológicas;
* Avaliação das exigências fenológicas da cultura.

A pesquisa definiu como limiar crítico:

**20,6 mm de precipitação acumulada em cinco dias.**

Valores inferiores a esse limite indicam condições favoráveis à ocorrência de estiagem para a cultura da soja.

Este indicador mostrou-se mais aderente às necessidades da cultura do que abordagens climáticas genéricas tradicionalmente utilizadas.

---

## Estrutura do Repositório

### Estudos Preliminares

Os códigos a seguir representam estudos exploratórios realizados durante o desenvolvimento da pesquisa. Embora não integrem diretamente a metodologia final da tese, foram fundamentais para compreender o contexto climático e produtivo da sojicultura em Mato Grosso do Sul.

| Arquivo      | Descrição                                                                                                                                                                                                                                                                                         |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Código 1** | Caracterização da produtividade da sojicultura em Mato Grosso do Sul e análise da relação com a Temperatura da Superfície do Mar (TSM). Utiliza Análise Exploratória de Dados e Testes de Hipótese para o período de 1995 a 2021. Fontes: PAM/IBGE e CPC/NOAA.                                    |
| **Código 2** | Avaliação do grau de significância do fator clima na Produtividade Total dos Fatores (PTF) da soja e proposta de modelo regressivo para rendimento (kg/ha). Utiliza técnica multivariada confirmatória com dados de 2006 e 2017. Fontes: PAM/IBGE, Censo Agropecuário, Ipeadata e ERA5/meteoblue. |

### Desenvolvimento da Tese

Os códigos abaixo constituem a base metodológica da tese.

| Arquivo      | Descrição                                                                                                                                                                                                                                                      |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Código 3** | Estudo climatológico da precipitação e temperatura em Dourados/MS, construção inicial do indicador de estiagem e primeiros experimentos com Machine Learning.                                                                                                  |
| **Código 4** | Código final da tese. Contém a definição do indicador de estiagem da cultura da soja, o treinamento, teste e validação dos modelos Random Forest, Extra Trees e XGBoost, além das análises utilizadas para construção dos resultados e conclusões da pesquisa. |

---

## Metodologia

A metodologia foi desenvolvida em quatro etapas principais:

1. Análise climatológica das séries históricas de precipitação e temperatura de Dourados/MS;
2. Construção do indicador de estiagem baseado em precipitação acumulada;
3. Desenvolvimento de modelos supervisionados de Machine Learning;
4. Validação dos modelos em safras com comportamentos climáticos contrastantes.

Foram avaliados os seguintes algoritmos:

* Random Forest;
* Extra Trees;
* XGBoost.

---

## Principais Resultados

### Indicador de Estiagem

* Limiar crítico definido em 20,6 mm acumulados em cinco dias;
* Indicador desenvolvido especificamente para a cultura da soja;
* Capacidade de monitoramento contínuo das condições hídricas durante o ciclo produtivo.

### Desempenho dos Modelos

#### Random Forest

* Acurácia de treinamento: 96,24%;
* Acurácia de teste: 85,79%.

#### Extra Trees

* Redução significativa de falsos negativos;
* Maior incidência de falsos positivos.

#### XGBoost

Melhor desempenho geral:

* Acurácia de treinamento: 96,90%;
* Acurácia de teste: 87,36%;
* Precisão: 0,94;
* Recall: 0,87.

O modelo apresentou melhor equilíbrio entre confiabilidade e capacidade de detecção de estiagens da cultura.

---

## Aplicações

O modelo possui potencial de aplicação em:

* Sistemas de alerta climático;
* Monitoramento agrícola;
* Cooperativas agropecuárias;
* Planejamento de irrigação;
* Gestão de riscos climáticos;
* Apoio à tomada de decisão no agronegócio.

---

## Tecnologias Utilizadas

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Scikit-Learn
* XGBoost
* Imbalanced-Learn (SMOTE)

---

## Palavras-chave

Inteligência Artificial • Machine Learning • Agricultura • Soja • Estiagem • Indicadores Agroclimáticos • Mudanças Climáticas

---

## Autora

**Franciane Rodrigues**
Doutora em Administração
Escola de Administração e Negócios (ESAN)
Universidade Federal de Mato Grosso do Sul (UFMS)
