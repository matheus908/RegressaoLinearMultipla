# Regressão Linear Múltipla

##### Código:
https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/3820285923208374/1720956257738858/7208511417105602/latest.html

#### 1. Pergunta de negócio

* entendimento dos preços de aluguel e custo dos imóveis para alugar em São Paulo
* conseguir criar um modelo de consiga estimar o preço de aluguel desses imóveis

#### 2. Base de dados de preços de aluguel em São Paulo

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/a1cb5b8f-8df0-4738-a0a5-8040dd63ee77)

#### 3. Convertendo os tipos de daoos

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/30bf2510-7dfa-458e-a630-ddf4d748b1c2)

#### 4. Identificando outliers

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/1adc91f7-fa3b-4e7e-9c16-dbbfb7ea14fd)

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/44a7d10b-f6ff-44a8-97d2-9d2d388b55ca)

#### 5. criando novas colunas

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/2ad3943a-2995-4dd1-a9d3-41306f9abb50)

* Percebemos através da indentificação de outliers, desconsideramos da base anúncios de preços de aluguel, com área menor do que 10 metros quadrados.

#### 6. Criação de base para modelo de regressão linear múltipla

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/e8ce602a-fd6a-4511-bcf6-f40c7814a5e4)

#### 7. Criação de variáveis dummies

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/0df3e743-c941-4c55-8371-33f85d0e9bd3)

* Regressão linear multipla, só permite variáveis numéricas
* Variáveis dummies, são variáveis categóricas em que cada elemento dessa variável categorica é transformada em uma coluna de variável numérica
* Só assim é possível usar essas variáveis em um modelo de regressão liner múltipla

#### 8. Separando bases de treino/teste e gerando o modelo

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/3feb5eda-eb0e-4ae9-8a10-7d36aba419fd)

#### 9. Gerando resultados do modelo

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/3c022b33-5039-4039-86cd-25cec8e0ca8e)

* o Coeficiente de determinação R2 = mede o grau de explicação das variáveis explicativas sobre a variável resposta(Preço do Aluguel)
* Grau de explicação nesse caso é 77,8% de grau de explicação.

#### 10. Relatório de resultados do modelo

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/1925301d-12a8-4431-bffe-8cc779fba95c)

![image](https://github.com/matheus908/RegressaoLinearMultipla/assets/60456455/c1e3a3c9-6bf9-4ce7-b8aa-0e4e518f3663)

* Como mostra o relatório o R2 é 0.778
* Também é importante citar o P>|t|, também conhecido como p-valor
* Se o p-valor for menor que 0.05 ou 5%, significa que aquela variável explicativa, é siginificativa para determinar a variável resposta
* Como sugestão de melhora do modelo, as variáveis DsTemMetro e Casa em condomínio, são maiores 0.05
* Portanto poderiam ser retiradas do modelo, pois não ajudam a explica a variável resposta.













