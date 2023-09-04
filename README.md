# Predição de Séries Temporais de Vendas

Por David Panduro :computer:

Analisaremos os **dados de vendas** de uma das lojas de uma grande **rede de supermercados**, a fim de fazer predições das vendas dos **próximos 30 dias**. 
A base geral conta com pouco mais de 01 mil~hao de registros. Mas inclui todas as lojas da rede de supermercados. Neste caso, por motivos de praticidade, filtraremos uma (01) loja para aplicar os conceitos de séries temporais nele. A base de amostra final fica com 942 registros, com as seguintes colunas:

  01. Date ==> É a data do evento. Está na granuladidade diária. É de tipo object, mas terá que ser convertido a índice.
  02. Sales==> É a quantidade monetária total das vendas diárias. É de tipo int, mas será convertido a float.
     
Aplicaremos métodos da estatística e de aprendizado de máquina:
  01. Visualização da série.<br><br>
  02. Decomposição da série.<br><br>  

  ![image](https://github.com/DavidPanduro/time_series_prediction/assets/45201867/025fb3a8-8609-4fe9-8b72-8522afbf20ce)  
  <p style="text-align: center;">Fig.02. _Seasonal Decomposition of Sales Dataset_</p><br>
  03. Visualização da Autocorrelação da série.<br><br>
  
  ![image](https://github.com/DavidPanduro/time_series_prediction/blob/master/acp_sales.jpg)
  <p style="text-align: center;">Fig.03. Autocorrelation of Sales Dataset</p><br>
  04. Visualização da Autocorrelação Parcial da série.<br><br>  
  
  ![image](https://github.com/DavidPanduro/time_series_prediction/blob/master/pacf_sales.jpg).
  <p style="text-align: center;">Fig.04. Autocorrelation Partial of Sales Dataset </p><br>
  05. Testes de Estacionaridade. Augmented Dickey-Fuller (ADF).<br><br>
  
  ![image](https://github.com/DavidPanduro/time_series_prediction/assets/45201867/58a22bc9-4156-436d-9d11-87f986387377)
  <p style="text-align: center;">Fig.05. Teste Augmented Dickey-Fuller </p><br>

  Nota: O teste de estacionaridade retornou que **os dados são estacionários**, sendo assim não precisaremos de suavização por diferenciação, de modo que, d=0. <br><br>
  06. Train/Test Split.<br><br>
  > Para os métodos estatísticos, a divisão ficou assim: O tamanho da data de treinamento ficou estabelecido em **751 registros** e os dados de teste ficaram em **30 registros**.
  > Para aprendizado de máquina, a divisão ficoua ssim: | Particao de Treinamento: 0 375 | Particao de Validação: 375 564 | Particao de Teste: 562 751 |
  07. Modelo AUTO-ARIMA.<br><br>
  08. Modelo ARIMA.<br><br>
  09. Modelo ARMA.<br><br>
  10. Comparação dos Modelos.<br><br>
  11. Modelo MultiLayer Perceptron (MLP).<br><br>
  12. Modelo Support Vector Regression (SVR).<br><br>
  13. Conclusões.<br><br>

Finalmente, apresentamos as seguestões dos **_próximos passos_** a seguir, segundo os resultados observados durante o processo da modelagem.

# time_series_prediction
