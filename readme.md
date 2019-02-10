~~~
~~~
# APT 가격예측 문제
Dacon에서 출제한 APT 가격 예측문제를 머신러닝 기법을 통해서 해결하고 데이터 분석 중에
산출된 가격이 의미가 있어서 TEST SET을 10년 기간으로 늘려 산출하였음
> Machine Learning is an idea to learn from examples and experience, without being explicitly programmed. Instead of writing code, you feed data to the generic algorithm, and it builds logic based on the data given.


## SIMPLE_EDA와 예측 모형
* 머신러닝 모형을 이용하여 거래가 되지 않는 아파트의 가격을 예측하는 문제임
* light_gbm을 이용하여 예측모형을 생성하였는데 예상보다 시계열에 대해 높은 정확도를 보임

##APT_결과데이터_시계열분석_KB월간자료와 비교 .

* 생성된 ML 모형 가격을 통하여 구별로 가격 시계열을 만들고 시각화하였음  
* 3918개의 아파트가 서울시 구별로 대표성을 가진다면 ML 모형으로 만들어지는 지수는 의미가 있음
* KB 통계자료와 비교시 ML모형으로 생성된 가격이 높게 형성되는 것을 확인할 수 있음

## APT_결과데이터_위치분석(지하철,학교, 지역클러스터링)
* 아파트 가격에 가장 영향을 주는 것이 지역요소임으로 이를 어떻게 처리해주냐에 따라 예측 모형 성능이 높아질 수 있음  
* Bokeh, Plotly를 사용하여 APT 모형 가격에 대해서 지하철, 학교, 지역으로 시각화 자료를 생성하였음
