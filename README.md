SOCAR 보험사기 예측 프로젝트 
=================================================
이 프로젝트는 카쉐어링 기업 SOCAR에서 제공받은 16,000건에 달하는 사고 데이터를 토대로 보험 사기를 예측해보기 위함에 있다.
머신러닝을 기반으로 한 데이터 분류 모델링을 진행하였다. <br>
보험사기는 전체 사고 비중에서 0.26%를 차지하는 극히 드문 케이스로, "데이터 불균형"속에서 모델링의 성능을 높여가는 것은 전처리, 파라미터 튜닝을 끊임없이 수정하는 작업의 연속이었다. <br>
최근 접근성이 용이한 카쉐어링 서비스를 악용한 보험사기가 급증하고 있다. 그로 인한 카쉐어링업체의 피해 또한 늘어나며 고초를 겪고 있다. 해당 프로젝트가 실제 업무 현장에서 기업의 손해를 최소화하기 위한 시스템 형성에 일조할 수 있기를 희망한다.

#### 데이터 불균형
데이터 불균형은 현실적인 데이터에서는 일반적으로 나타나고 있다. <br>
본 프로젝트에서는 전체 16,000건의 데이터중에서 보험사기는 단 41건으로 모델이 학습할 수 있는 보험사기의 데이터가 굉장히 작은 상황에서 출발하였다. <br><br>
<img src="https://user-images.githubusercontent.com/72846750/105158413-4ac78380-5b51-11eb-8d2e-8b9462323210.png" width="300" height="200"/>

#### 프로젝트 평가 기준
해당 프로젝트는 패스트캠퍼스 데이터사이언티스트 15기 과정 중 일부로 진행되었다. 하여, 이전 14기수에서 동일한 프로젝트로 진행하면서 얻었던 성능을 Baseline으로 두어 보다 향상된 모델을 만들고자 하였다. <br>
테스트셋을 기준으로 하며, Support Vector Machine 모델로 진행되었다고 한다. <br>
* Baseline Metric : accuracy 0.492791, precision 0.003153, recall 0.714286 <br>

데이터 불균형으로 인하여, 모든 사고를 "No Fraud"로 예측하더라도 accuracy는 0.99임으로 accuracy는 중요한 평가의 척도가 되기는 어려워 보인다. 하여, 실제 보험사기중에 얼마나 많이 예측해냈는지를 나타내는 recall과, 예측한 보험사기중에 얼마나 많은 실제 보험사기가 있었느냐를 나타내는 precision을 중요한 평가 기준으로 하였다.

#### 보험사기 소개
카쉐어링 서비스는 스마트폰 애플리케이션만으로 비대면 차량 출고와 반납이 가능하여, 면허증이 없거나 운전에 미숙한 10대,20대가 차량을 쉽게 빌릴 수 있어 보험사기 주 타겟이 되어가고있다. <br> 현재 논란이 되고 있는 현실에 맞지 않은 법 체계로 인하여 보험사기를 실제로 신고하고 적발하는 건수가 많지 않은 것으로 알려져있다.1) <br>
본 프로젝트의 데이터 또한 법적으로 보험사기가 실제 적발된 경우에 한해서만 "Fraud"로 분류하고 있어, 실제 보험사기보다는 적은 데이터만이 "Fraud"로 분류되어진 것으로 보인다. <br><br>


본론
=================================================

본 프로젝트에서는 트리 계열의 모델 중 Decision Tree, Random Forest, LightGBM과 경사하강법 기반의 Logistic Regression 모델을 사용하였다. 최적의 예측 모델은 LightGBM으로 accuracy 0.964114, precision 0.043478, recall 0.714286의 성능을 얻을 수 있었다.
나머지 3가지 모델에서도 Baseline 대비 뛰어난 성능을 만들어낼 수 있었다. <br>


#### 컨텐츠
* 문제 정의
* 데이터 탐색
* 평가 기준
* 데이터 전처리
* 모델링
* 모델 검증
* 결론 <br><br>


#### 참조
1)https://programs.sbs.co.kr/culture/maninblackbox/clip/55706/OC451916010 <br><br>


#### 기여자
* 김준성(a.k.a 튜닝몬스터) https://github.com/whistle-boy
* 방희란(a.k.a 판다스의 신) https://github.com/Heeran-cloud
* 정혜주(a.k.a 논문통찰자) https://github.com/hjung53
