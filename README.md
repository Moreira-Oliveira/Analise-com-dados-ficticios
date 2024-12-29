# Analise-com-dados-ficticios

Programa utilizado

![Captura de tela 2024-12-29 145350](https://github.com/user-attachments/assets/54113d46-b866-42a8-ab4c-eeb5c414883c)

🏁 Projeto

Segue os prints das execuções em ambiente
Geração de dados

![Captura de tela 2024-12-29 150022](https://github.com/user-attachments/assets/3a597c0f-52ea-45ed-bea3-d66f51098790)

A procedura gera 1000 registros simulados na tabela, variando dados como valores, datas, centros de custo, moedas e taxas de conversão. É particularmente útil para criar dados de teste com características próximas a um cenário real, como variação de valores, categorias, e aleatoriedade controlada.

Resultado:

![Captura de tela 2024-12-29 150519](https://github.com/user-attachments/assets/b0f7df5c-4428-4077-9122-92a976e50cc9)

Sumarização de Dados

![Captura de tela 2024-12-29 151020](https://github.com/user-attachments/assets/d8f03337-4a71-4fad-93e4-082342cf77be)

Essa query fornece uma visão detalhada de como os lançamentos contábeis estão distribuídos entre os diferentes centros de custo. Inclui contagens, estatísticas básicas (soma, média, mediana, maior e menor valores) e somas específicas por moeda (USD, EUR, BRL). Além disso, avalia a média das taxas de conversão e organiza os resultados pelos centros de custo com maior soma total de valores.
Essas informações podem ser usadas para identificar os centros de custo mais relevantes, avaliar padrões em diferentes moedas e detectar outliers.

Distribuição de Dados

![Captura de tela 2024-12-29 151401](https://github.com/user-attachments/assets/e6b0b06d-7360-4e05-9653-f33a49557f5a)

Análise estatística dos lançamentos financeiros agrupados por centro de custo. Ela fornece contagem de lançamentos, soma total, média, maior e menor valor, soma dos valores por moeda (USD, EUR, BRL), média das taxas de conversão e a mediana dos valores. Os resultados são ordenados pelos centros de custo com maior soma total de valores.

Identificando outliers nos lançamentos

![Captura de tela 2024-12-29 151833](https://github.com/user-attachments/assets/e62aeca4-aef7-4f41-99ce-b9e4631b33ff)

Essa query identifica outliers nos lançamentos contábeis com base no Intervalo Interquartil (IQR) para cada combinação de centro_custo e moeda. Ela calcula os limites inferior e superior dos valores permitidos e filtra os registros que estão fora desses limites. Esses outliers são então exibidos ordenados por valor, centro de custo e moeda.

Calculando média móvel de 3 dias

![Captura de tela 2024-12-29 152129](https://github.com/user-attachments/assets/76d11344-6e32-445d-88c8-94a7c1eff439)

Essa query calcula a média móvel de 3 dias para os lançamentos contábeis, agrupando-os por centro_custo e ordenando por data_lancamento. A média móvel é calculada considerando os dois dias anteriores e o dia atual. Além disso, ela cria um ranking para cada data de lançamento, com base na média móvel, em ordem decrescente. O resultado é exibido ordenado por data de lançamento e pelo ranking da média móvel.
