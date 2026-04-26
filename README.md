# Previsao do Numero de Servidores da Secretaria de Educao - 2026

Análise de Série Temporal: Servidores da Educação (Uberlândia/MG)

Este projeto realiza o estudo estatístico e a previsão do número de servidores da Secretaria de Educação de Uberlândia utilizando dados abertos da prefeitura (período de 2021 a 2025). O objetivo principal é fornecer previsões para os próximos 12 meses.


<img width="576" height="301" alt="SERIE_ORIGINAL" src="https://github.com/user-attachments/assets/19d5096a-80ac-414d-8fd1-fc8155ef42d4" />


🚀 Destaques Técnicos

Análise Exploratória: Identificação de tendência de crescimento e forte sazonalidade, com quedas acentuadas em janeiro devido à dinâmica contratual do setor.

<img width="576" height="301" alt="SAZONALIDADE" src="https://github.com/user-attachments/assets/7da75865-3a79-4163-8e9a-63654a13f386" />


Modelagem Comparativa: Foram testados modelos paramétricos (ARIMA/SARIMA) com transformações de Box-Cox, e modelos não paramétricos como GAM (Modelos Aditivos Generalizados) e STL.

Validação: Utilização de técnica de treino e teste para seleção do modelo com base no MAPE (Erro Percentual Absoluto Médio).

Resultado: O modelo STL+Naive foi o mais adequado, apresentando o menor erro (MAPE de 2,32%), demonstrando um comportamento repetitivo e conservador nas contratações.

<img width="576" height="301" alt="PREVISAO" src="https://github.com/user-attachments/assets/dcc9b04f-de64-420b-8145-fa52b88bbc02" />


🛠️ Ferramentas Utilizadas

Linguagem: R.Bibliotecas: forecast, mgcv, ggplot2, tseries, entre outras.

Testes Estatísticos: Ljung-Box (independência) e Shapiro-Wilk (normalidade) para diagnóstico de resíduos.
