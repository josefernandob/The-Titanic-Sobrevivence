# Análise de Sobrevivência do Titanic com Machine Learning
## Visão Geral do Projeto
Este projeto é uma análise completa do famoso conjunto de dados do Titanic, utilizando técnicas de ciência de dados e Machine Learning para prever a sobrevivência de passageiros. O objetivo foi não apenas construir um modelo preditivo, mas também entender os principais fatores que influenciaram a taxa de sobrevivência, validando as descobertas através de visualizações de dados.

## Metodologia
O projeto seguiu um fluxo de trabalho padronizado em Machine Learning, passando pelas seguintes etapas:

## Pré-processamento de Dados:

Tratamento de valores ausentes (Idade, Tarifa e Embarque).

Criação de uma nova característica (Familia) a partir de colunas existentes, aprimorando a capacidade de previsão do modelo.

Separação das características (X) e da variável alvo (y).

Engenharia de Características:

As variáveis numéricas (Idade, Tarifa, Familia) foram padronizadas usando StandardScaler para evitar que grandes valores dominassem o treinamento do modelo.

As variáveis categóricas (Sexo, Embarque) foram convertidas para um formato numérico usando OneHotEncoder.

A ferramenta ColumnTransformer foi usada para aplicar todas as transformações de forma organizada.

## Modelagem e Treinamento:

Os dados foram divididos em conjuntos de treino e teste para garantir uma avaliação justa do modelo.

Dois modelos de classificação foram testados: LogisticRegression e RandomForestClassifier.

O RandomForestClassifier obteve um desempenho superior, com uma acurácia de 82.68%, sendo o modelo escolhido para a análise final.

## Análise de Descobertas:

A importância de cada característica foi extraída do modelo RandomForestClassifier, revelando quais fatores foram mais decisivos para a previsão.

Gráficos foram criados para validar visualmente as descobertas do modelo.

## Principais Descobertas
A análise dos dados e do modelo de Machine Learning resultou nos seguintes insights:

O fator mais decisivo para a sobrevivência foi o Sexo do passageiro. Historicamente, a política de "mulheres e crianças primeiro" teve um impacto significativo, e o modelo de Machine Learning refletiu isso com grande precisão.

Como mostra o gráfico abaixo: <img width="851" height="631" alt="image" src="https://github.com/user-attachments/assets/237fd944-2660-4ac2-9106-d01704ceea02" />


A Tarifa paga e a Idade também foram fatores extremamente importantes, indicando que a classe social e a idade do passageiro influenciaram as chances de sobrevivência.

Passageiros que embarcaram em Cherbourg tiveram a maior taxa de sobrevivência, uma vez que o porto era o ponto de embarque para muitos dos passageiros mais ricos e de primeira classe. Conforme gráfico:

<img width="658" height="464" alt="image" src="https://github.com/user-attachments/assets/d285fd7e-9dcd-4282-9c9a-f7b222e2e693" />


## Tecnologias e Bibliotecas
Linguagem de Programação: Python

Manipulação e Análise de Dados: Pandas

Machine Learning: Scikit-learn

Visualização de Dados: Matplotlib, Seaborn# The-Titanic-Sobrevivence

## Baixando dependências

Você pode baixar as dependências baixando o arquivo requirements.txt e utilizando o comando pip install -r requirements.txt
OBs: O arquivo precisa estar na pasta da IDE.
