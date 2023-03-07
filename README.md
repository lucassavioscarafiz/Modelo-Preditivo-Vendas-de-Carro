# Modelo Preditivo para Vendas de Carro

## 1.0 OBJETIVO DO CASE 💻

👉 Com crescentes demandas e competições acirradas no mercado, uma loja fictícia do ramo de carros está buscando prever o preço dos carros para os próximos anos e o aumento de vendas.

👉 Neste case irei abordar diferentes **modelos supervisionados preditivos** de **regressão** utilizando os principais algoritmos de Machine Learning, buscando prever o preço de venda de carros baseado nas informações fornecidas pelo dataset como Kilometragem do veículo, anos de uso, combustível e assim por diante. 

👉 Além de criar diferentes modelos baseados nos principais algoritmos, o objetivo é buscar aperfeiçoá-lo evitando-se assim o seu overfitting e, ou, underfitting.

👉 Também irei trazer diferentes Insights e importantes indicadores de negócios que auxiliam na tomada de decisão na construção dos modelos preditivos regressivos, bem como na tomada de decisão baseada em Vendas.


## 2.0 METODOLOGIA 🔧

Utilizei algoritmos de Machine Learning como: `Regressão Linear`, `Regressão Lasso`, `Regressão Ridge`,`KNNRegressor`, `RandomForestRegressor`,e `GradientBoostingRegresor`para buscar o melhor modelo regressivo, além de analisar importantes métricas de pontuação do modelo como: `R²`, `Mean Absolute Absolute Erros`,`Mean Squared Erros`,e `Root Mean Squared Erros`. Também foi utilizado `GridSearch` e `RandomizedSearch` para encontrar os melhores hiperparâmetros a serem utilizados nos modelos que foram utilizados os algoritmos de `RandomForestRegressor` e `GradientBoostingRegresor`.


## 3.0 RESULTADOS 🤖

As tabelas abaixo indicam os valores das principais métricas de pontuação utilizadas para medição do erro e acerto de cada um dos modelos criados ao longo do estudo. Os gráficos apresentam na linha vermelha o valor real dos dados que foram separados para teste e a linha azul os valores previstos pelo modelo

* #### 3.1) Modelo de Regressão Linear Simples

Mean Absolute Erros  | Mean Squared Error | Root Mean Squared Error|   R²  | 
-------------------  | ------------------ | ---------------------- | ----- | 
1.313                | 4.422              | 2.103                  | 0.747 | 

![image](https://user-images.githubusercontent.com/81670585/223466563-b4647022-2898-4dce-9d9e-df0ebfcbf581.png)

* #### 3.2) Modelo de Regressão Ridge (Alpha = 10)

Mean Absolute Erros  | Mean Squared Error | Root Mean Squared Error|   R²  | 
-------------------  | ------------------ | ---------------------- | ----- | 
1.341                | 4.979              | 2.231                  | 0.817 | 

![image](https://user-images.githubusercontent.com/81670585/223467174-16754225-6926-49d8-83ce-6a3ba4340f16.png)

* #### 3.3) KNNRegressor (K=5)

Mean Absolute Erros  | Mean Squared Error | Root Mean Squared Error|   R²  | 
-------------------  | ------------------ | ---------------------- | ----- | 
0.863                | 1.482              | 1.2176                 | 0.915 | 

![image](https://user-images.githubusercontent.com/81670585/223467600-6355a227-ed8b-457d-bf2e-d64b53e64cb9.png)

* #### 3.4) RandomForestRegressor (default)

Mean Absolute Erros  | Mean Squared Error | Root Mean Squared Error|   R²  | 
-------------------  | ------------------ | ---------------------- | ----- | 
0.516                | 0.6614             | 0.8132                 | 0.962 | 

![image](https://user-images.githubusercontent.com/81670585/223467807-316e0b99-2e9e-4a21-bb28-0046d3e072c8.png)

* #### 3.5) GradientBoostingRegressor (default)

Mean Absolute Erros  | Mean Squared Error | Root Mean Squared Error|   R²  | 
-------------------  | ------------------ | ---------------------- | ----- | 
0.484                | 0.4823             | 0.6944                 | 0.972 | 

![image](https://user-images.githubusercontent.com/81670585/223468173-fdee8c74-841c-4465-a884-0bf2bf98d29f.png)

* #### 3.6) GradientBoostingRegressor (learning_rate=0.01, max_depth=7, n_estimators=1200)

Mean Absolute Erros  | Mean Squared Error | Root Mean Squared Error|   R²  | 
-------------------  | ------------------ | ---------------------- | ----- | 
0.554                | 0.7939             | 0.8910                 | 0.954 | 

![image](https://user-images.githubusercontent.com/81670585/223468462-a92bcb33-9ad0-41a4-9792-ea44f771aef9.png)

* #### 3.7) Previsões

* Dados fornecidos para que o modelo consiga prever o preço de venda do carro

Present_Price  | Kms_Driven | Fuel_Type| Seller_Type | Transmission| Owner | Car_Age |
-------------  | ---------- | -------- | ----------- | ----------- | ------| ------- |
10.52          | 38000      | 1        | 1           | 2           | 1     | 4       |

* Preços previstos por cada modelo

Regressão Ridge  | KNN        | RandomForest| GradientBoosting |
---------------  | ---------- | ----------- | ---------------- | 
7.05             | 4.97       | 7.3         | 7.32             | 

<h3 align="left">Contato:</h3>
<p align="left">
<a href="https://linkedin.com/in/lucassavioscarafiz" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="lucassavioscarafiz" height="30" width="40" /></a>
</p>

📫 **lucassavioscarafiz@gmail.com**

<h3 align="left">Linguagens e Ferramentas:</h3>
<p align="left"> <a href="https://cloud.google.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://scikit-learn.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="scikit_learn" width="40" height="40"/> </a> <a href="https://seaborn.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" alt="seaborn" width="40" height="40"/> </a> </p>
