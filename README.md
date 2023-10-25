# # Entendendo a análise de vibração para manuntenção preditiva de elevadores

## Visão Geral

Neste projeto, vamos analisar os dados disponíveis, no conjunto de dados sobre de uma variedade de sensores IoT, para manutenção preditiva na indústria de elevadores. 

Você pode conferir o dataset e o projeto na íntegra clicando abaixo:

Link dataset: https://www.kaggle.com/datasets/shivamb/elevator-predictive-maintenance-dataset

Link do código do projeto: https://github.com/gustavoptavares/Manuten-o-Elevador/blob/main/Manuten%C3%A7%C3%A3o_Elevador.ipynb

## Problema e Solução

Vamos analisar os dados o conjunto de dados sobre de uma variedade de sensores IoT, para manutenção preditiva na indústria de elevadores. Contém dados de operação, na forma de séries temporais amostradas a 4 Hz no horário de pico alto e no uso noturno do elevador em um edifício, vamos entender, no detalhe, os dados são úteis para manutenção preditiva de portas de elevadores, como:

• Enteder o conjunto de dados para reduzir paradas não planejadas e maximizar o ciclo de vida do equipamento.

• Previsão do valor absoluto da vibração. 

## O Processo

O primeiro passo do projeto foi adquirir os dados. Utilizamos os dados do portal Kaagle, carregando-o no Google Colab, para a exploração e análise dos dados utilizando a linguagem de programação Python e suas bibliotecas, como Pandas, Matplotlib, Tensorflow e Scikit-Learn. Foi feita análise exploratória, visualização dos dados, e foi aplicado o modelo preditivo de LSTM no conjunto de dados sequências no formato de série temporais.

## Resultados

Os valores das métricas calculadas:

MSE (Erro Quadrático Médio): 31.671153220256016

MAE (Erro Absoluto Médio): 1.6311902100839857

R²(Coeficiente de Determinação): 0.9453278103520457

Vamos analisar esses valores:

MSE (Erro Quadrático Médio): O valor de MSE é relativamente baixo, o que sugere que o modelo tem um bom ajuste aos dados. No entanto, o valor absoluto do MSE pode ser mais interpretável quando comparado com outras métricas ou outros modelos.

MAE (Erro Absoluto Médio): O MAE de aproximadamente 1.63 indica que, em média, o modelo erra em cerca de 1.63 unidades ao prever a variável 'vibration'. Este valor dá uma ideia direta da magnitude do erro.

R²(Coeficiente de Determinação): Um R² de aproximadamente 0.945 é bastante alto e indica que o modelo explica cerca de 94,5% da variabilidade nos dados de 'vibration'. Isso sugere que o modelo tem um desempenho muito bom.

## Conclusões

O modelo LSTM foi utilizado para prever os valores da coluna 'vibration'. A preparação dos dados envolveu a criação de sequências temporais e a divisão em conjuntos de treinamento e teste. Após o treinamento, o modelo foi avaliado usando várias métricas.

O modelo LSTM parece ter um desempenho muito bom na previsão da variável 'vibration', com base nas métricas fornecidas. O valor alto de R² sugere que o modelo é capaz de capturar a maioria da variabilidade nos dados, e os valores de MSE e MAE sugerem que os erros nas previsões são relativamente baixos.

No entanto, sempre é uma boa prática comparar o desempenho deste modelo com outros modelos ou benchmarks para ter uma ideia mais clara de seu desempenho relativo. Também pode ser útil visualizar as previsões versus os valores reais para obter uma compreensão visual do desempenho do modelo.​
