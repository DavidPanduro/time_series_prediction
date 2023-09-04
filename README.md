# time_series_prediction
# Predição de Séries Temporais de Vendas

Por David Panduro

Analisaremos os dados de vendas de uma das lojas de uma grande rede de supermercados, a fim de fazer predições das vendas dos próximos 30 dias. 
A base geral conta com pouco mais de 01 mil~hao de registros. Mas inclui todas as lojas da rede de supermercados. Neste caso, por motivos de praticidade, filtraremos uma (01) loja para aplicar os conceitos de séries temporais nele. A base de amostra final fica com 942 registros, com as seguintes colunas:

  01. Date ==> É a data do evento. Está na granuladidade diária. É de tipo object, mas terá que ser convertido a índice.
  02. Sales==> É a quantidade monetária total das vendas diárias. É de tipo int, mas será convertido a float.
     
Aplicaremos métodos da estatística e de aprendizado de máquina:
  01. Visualização da série.
  02. Decomposição da série.
  03. Visualização da Autocorrelação da série.
  04. Visualização da Autocorrelação Parcial da série.
  05. Testes de Estacionaridade. Augmented Dickey-Fuller (ADF).
  06. Train/Test Split.
  07. Modelo AUTO-ARIMA.
  08. Modelo ARIMA.
  09. Modelo ARMA.
  10. Comparação dos Modelos.
  11. Modelo MultiLayer Perceptron (MLP).
  12. Modelo Support Vector Regression (SVR).
  13. Conclusões.

Finalmente, apresentamos as seguestões dos **próximos passos** a seguir, segundo os resultados observados durante o processo da modelagem.
