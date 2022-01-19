# Previsão Meteorológica do Tempo

Resumo geral dos dados dos dados: Ele contém quatorze dados de previsão meteorológica numérica da previsão do tempo (NWP), duas observações in-situ e cinco variáveis auxiliares geográficas sobre Seul, Coréia do Sul no verão. 

Documentos relevantes: Cho, D., Yoo, C., Im, J., & Cha, D. (2020). Avaliação comparativa de vários métodos de correção de viés baseados em aprendizado de máquina para previsões de modelos numéricos de previsão do tempo de temperaturas extremas do ar em áreas urbanas. Ciências da Terra e do Espaço.

Objetivo: Prever o clima com base em dados anteriores e verificar as variações com os valores reais.

Repositório: os dados foram obtidos através da UCI Machine Learning Repository. Você pode verificar a descrição dos dados e baixa-los por aqui: 
https://archive.ics.uci.edu/ml/datasets/Bias+correction+of+numerical+prediction+model+temperature+forecast

##  Informações Gerais do Conjunto de Dados

Os dados obtidos para tal análise são usados para fins de correção de viés da previsão das temperaturas máximas e mínimas do ar para o dia seguinte do modelo LDAPS operado pela Administração Meteorológica da Coréia sobre Seul, Coréia do Sul. Esses dados consistem em dados de verão de 2013 a 2017. Os dados de entrada são compostos em grande parte pelos dados de previsão do dia seguinte do modelo LDAPS, temperaturas in situ máximas e mínimas atuais e variáveis auxiliares geográficas. Existem duas saídas (ou seja, temperaturas máximas e mínimas do ar no dia seguinte) nestes dados.

O conjunto de dados é composto por um total de 7.752 linhas e 25 colunas. Algumas das dessas colunas incluem estação, data, latitude, longitude, temperatura atual máxima e mínima, temperatura máxima e mínima do dia seguinte, quantidade de radiação recebida, inclinação do local etc. As últimas 2 linhas do conjunto de dados têm valores ausentes de data e informações da estação, portanto, essas duas últimas foram removidas do conjunto de dados utilizado nesta análise.


As etapas principais envolvidas nesta tarefa foram:
- Premissas e Visualização dos dados;
- Previsão e Verificação de viés;
- Avaliação de Sensibilidade e Precisão;
- Sugestões e outras estratégias.

## Resultados

Para os modelos de regressão foi:
- A acurácia média para Next_Tmax é: 80,43%
- A acurácia média para Next_Tmin é: 86,29%

Para os modelos de classificação foi:
- A precisão média para Next_Tmax é: 74.22%
- A precisão média para Next_Tmin é: 80.42%
