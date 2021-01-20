프로젝트 개요
=================================================
이 프로젝트는 카쉐어링 기업 쏘카에서 제공받은 16,000건에 달하는 사고 데이터를 토대로 보험 사기를 예측해보기 위함에 있다.
머신러닝을 기반으로 한 데이터 분류 모델링을 진행하였다. 
보험사기는 전체 사고 비중에서 0.26%를 차지하는 극히 드문 케이스로, "데이터 불균형"속에서 모델링의 성능을 높여가는 것은 전처리, 파라미터 튜닝을 끊임없이 수정하는 작업의 연속이었다.
최근 접근성이 용이한 카쉐어링 서비스를 악용한 보험사기가 급증하고 있다. 그로 인한 카쉐어링업체의 피해 또한 늘어나며 고초를 겪고 있다. 해당 프로젝트가 실제 업무 현장에서 기업의 손해를 최소화하기 위한 시스템 형성에 일조할 수 있기를 희망한다.

#### 데이터 불균형
데이터 불균형은 여러 산업에서 일반적으로 발생하고 있다. 생산공정내에서 발생하는 불량, 공항입국자 중 테러리스트, 암환자등을 예측해보는 경우를 대표적인 예시로 들 수 있겠다.
해당 프로젝트를 진행해봄으로써 향후 다뤄볼 프로젝트에도 많은 긍정적인 영향을 줄 것으로 기대한다. 

#### 프로젝트 평가 기준
해당 프로젝트는 패스트캠퍼스 데이터사이언티스트 15기 과정 중 일부로 진행되었다. 하여, 이전 14기수에서 동일한 프로젝트로 진행하면서 얻었던 성능을 Baseline으로 두어 보다 향상된 모델을 만들고자 하였다. 
테스트셋을 기준으로 하며, Support Vector Machine 모델로 진행되었다고 한다.
* Baseline Metric : accuracy 0.492791, precision 0.003153, recall 0.714286

데이터 불균형으로 인하여, 모든 사고를 "No Fraud"로 예측하더라도 accuracy는 0.99임으로 accuracy는 중요한 평가의 척도가 되기는 어려워 보인다. 하여, 실제 보험사기중에 얼마나 많이 예측해냈는지를 나타내는 recall과, 예측한 보험사기중에 얼마나 많은 실제 보험사기가 있었느냐를 나타내는 precision을 중요한 평가 기준으로 하였다.

#### 보험사기 소개
금감원은 2019년 보험사기로 적발된 피해 금액이 8,809억원에 달함을 발표한바 있다.
이외에 적발되지 않은 보험사기건수까지 합해진다면, 그 금액은 1조 이상에 달할 것으로 예측하고 있다. 

카쉐어링 서비스는 스마트폰 애플리케이션만으로 비대면 차량 출고와 반납이 가능하여, 면허증이 없거나 운전에 미숙한 10대,20대가 차량을 쉽게 빌릴 수 있는 환경이 되면서 보험사기가 늘고 있다. 
차로를 바꾸는 승용차와 일부러 부딪히는 수법이 주로 쓰이고 있는데, 이 또한 법을 악용하기 위함에 있다.
피해 운전자가 차량 변경을 위한 충분한 행동이 있었음에도, 보험사기 차량임을 입증하기 이전까지는 오히려 피해 운전자에게 불리하게 작용되어 최대 면허 정지까지 이를 수 있기 때문이다.1)
이로 인해 보험사기를 실제로 신고하고 적발되는 건수는 많지 않다. 본 프로젝트의 데이터 또한 이로 인하여, 법적으로 보험사기가 실제 적발된 경우만 "Fraud"로 분류하고 있으므로, 현실에 맞는 법 개선이 반드시 필요해보인다. 

프로젝트 본론
=================================================

본 프로젝트에서는 트리 계열의 모델 중 Decision Tree, Random Forest, LightGBM과 경사하강법 기반의 Logistic Regression 모델을 사용하였다. 최적의 예측 모델은 LightGBM으로 accuracy 0.964114, precision 0.043478, recall 0.714286의 성능을 얻을 수 있었다.
나머지 3가지 모델에서도 Baseline 대비 뛰어난 성능을 만들어낼 수 있었다. 


#### 컨텐츠
* 문제 정의
* 데이터 수집
* 데이터 탐색
* 데이터 모델링
* 데이터 전처리
* 데이터 모델링_2
* 모델 검증
* 결론


참조
1)https://programs.sbs.co.kr/culture/maninblackbox/clip/55706/OC451916010


기여자
* 김준성(a.k.a 튜닝몬스터) https://github.com/whistle-boy
* 방희란(a.k.a 판다스의 신) https://github.com/Heeran-cloud
* 정혜주(a.k.a 논문통찰자) https://github.com/hjung53
