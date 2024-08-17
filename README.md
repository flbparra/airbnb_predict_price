# Projeto de previsao dos precos AirBnB

 No Airbnb, qualquer pessoa que tenha um quarto ou um imóvel de qualquer tipo (apartamento, casa, chalé, pousada, etc.) pode ofertar o seu imóvel para ser alugado por diária.

Você cria o seu perfil de host (pessoa que disponibiliza um imóvel para aluguel por diária) e cria o anúncio do seu imóvel.

Nesse anúncio, o host deve descrever as características do imóvel da forma mais completa possível, de forma a ajudar os locadores/viajantes a escolherem o melhor imóvel para eles (e de forma a tornar o seu anúncio mais atrativo).

Existem dezenas de personalizações possíveis no seu anúncio, desde quantidade mínima de diária, preço, quantidade de quartos, até regras de cancelamento, taxa extra para hóspedes extras, exigência de verificação de identidade do locador, etc.

Com base nessas informações, podemos tentar criar modelos preditivos em relação ao preço de aluguel dos imóveis ofertados, visando a identificação de preços competitivos com base em ofertas semelhantes.

### Perguntas:
-  Fazer uma análise no dataset utilizando as ferramentas aprendidas no
período; 
> In result.ipynb
b. Demonstrar como pré-processar e representar os diferentes tipos de
dados;
> In result.ipynb
- Demonstrar a utilização de técnicas como one-hot encoding, redução de
dimensionalidade e PCA;
> In result.ipynb
- Como a redução da dimensionalidade afetou no desempenho do
modelo?
> No meu melhor modelo (DecisionTreeClassifier) MAE: 4531.9171935825025, MSE: 17.9343849148309, R2: 0.9148252333115133 esses foram os resultados  sem o PCA, o r2 está próximo de 1, MSE segue baixo, o que indica melhor ajuste aos dados, em contra mão temos MAE está em 4 mil, o que indica que minhas previsoes não estão sendo precisas. O PCA ajuda no decaimento do MAE, resultado com o PCA - MAE: 149.69793440692766, tornando o modelo mais preciso. E mais sensivel a outlines, pois MSE aumento bastante.
> Em result.ipynb
   Aplicar regressão nos dados - dividir o dataset em treinamento e
validação e aplicar, pelo menos, 3 algoritmos distintos de regressão para
prever o preço do imóvel. Testar visualizar os resultados, comparando o
desempenho dos modelos treinados;
- Qual modelo performou melhor?
> No meu caso, foi o DecisionTreeClassifier, com R2 acima de 0.9.
- Avaliar o desempenho do(s) modelo(s) treinado(s). A métrica da
competição será o erro quadrático médio (MSE), porém, recomenda-se a
avaliação do modelo por outras métricas adicionais, como o R² e o erro
médio absoluto (MAE).
> Fiz isso também, meu modelo usou 3 metricas (MSE, MAE e R2), gostei bastante de ver os modelos de Arvores binarias em acao.



### Requerimentos:
- requerimentos.txt

### Tecnologias usada:
- Python
- Pandas
- Numpy
- Sklearn
- Statsmodels
- MatlibPlot e Seaborn
- Jupyter e Goole colabe

