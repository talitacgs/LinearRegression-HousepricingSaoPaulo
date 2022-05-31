# LinearRegression-HousepricingSaoPaulo

## 1. Project Motivation 

Esse projeto foi desenvolvido na 4° Edição da Imersão de Dados da Alura, onde foram ministradas aulas durante uma semana, introduzindo conceitos de Ciência de Dados e Machine Learning. O projeto final consiste no desenvolvimento de um modelo de machine learning supervisonado com algoritmo de Regressão Linear para predição do valor dos imóveis da cidade São Paulo, Brasil.  

## 2. Data 

Foi disponibilizado um dataset com informações básicas de imóveis da cidade de São Paulo. Durante a imersão, foi estimulado o cruzamento de dados com outros dataset, dentre eles o disponibilizado pelo IBGE, no qual era necessário consultar documentação de levantamento dos dados, para compreensão do significado de cada coluna. O modelo contou também com dataset de endereços e enriquecimento de informação de geolocalização através de biblioteca específica.

## 3. Implementation

Na fase de processamento dos dados, foi realizada o tratamento de valores faltantes/nulos. Construção de um único dataframe através do cruzamento de dataset provenientes de diferentes fontes, bem como manipulações pertinentes ao processo, tais quais seleção de colunas relevantes para o modelo, mudança de tipo de variávels, coluna calculada, informação através de geolocalização. 
A análise gráfica se deu através de gráficos boxplot, onde foi considerado outliers imóveis acima de 60Mi e abaixo de 100K por sua baixa representatividade. Foram plotados gráficos de pontos e histograma, para avaliar a distribuição dos dados, e gráfico de correlação que demonstra sinais de correlação entre as variáveis e a que o modelo quer prever. 
Após o processamento, os dados foram separados em 70% treino e 30% teste e os valores foram normalizados para uma mesma escala. Nesse momento, foi importante excluir a variável calculada, por conter informações que o modelo deveria prever.

## 4. Result

 O gráfico de linha mostra o Y_pred e o Y_true para os 70 primeiros resultados, que possuem zonas com boa capacidade de predição e outras com erros significativos. Para quantificar, foi utilizado a métrica de R2 e MAE (Mean Absolute Error), que apresentaram resultados pouco satisfatórios, demonstrando que a etapa de processamento de dados deverá ser revisitada. Para próximos passos, uma abordagem possível seria a remoção das variáveis com valores praticamente constantes, observados no histograma.
