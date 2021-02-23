# SOCAR 보험사기 예측 프로젝트
해당 프로젝트는 패스트캠퍼스 데이터사이언티스트 15기 과정중 진행.<br>
본 프로젝트는 머신러닝을 기반으로 카쉐어링업계에서 극심해지는 보험 사기를 예측해보기 위함에 있음.<br>

#### 1. 데이터 수집
데이터는 카쉐어링업체 SOCAR로부터 제공받았으며, 16000 rows X 35 columns의 데이터로 구성되어 있음.<br>

#### 2. 진행 과정
- 데이터 탐색
- 데이터 전처리
- 모델링
- 모델 검증
- 결론<br>

#### 3. 데이터 불균형
전체 16000건의 데이터중에서 보험사기는 단 41건. <br>
데이터 불균형을 해소하기 위해서 다양한 Oversampling 기법을 시도하여, 평가. <br>
<img src="https://user-images.githubusercontent.com/72846750/105158413-4ac78380-5b51-11eb-8d2e-8b9462323210.png" width="300" height="200"/>

#### 4. 데이터 전처리
- 결측치 및 이상치 제거     
- 오버샘플링                
- 스케일링                 
- PCA를 통한 Feature 생성
- 원핫인코딩
- Feature Importance 확인후 Feature Extraction
오버샘플링, Feature Importance 확인후 Feature Extraction만이 성능을 향상시킴.<br>


#### 5. 평가 기준
이전 기수인 14기에서 본 프로젝트로 얻었던 최적의 성능을 Baseline 으로 두었음.
  - accuracy 0.493, precision 0.003, recall 0.714
데이터 불균형으로, 모든 사고를 No Fraud 로 예측시, accuracy 0.997. accuracy는 중요한 평가 척도가 되기 어려움.<br>
객관적인 성능 평가를 위하여 precision, recall 을 평가 기준으로 결정.
  <img src="https://user-images.githubusercontent.com/72846750/105166682-0b9e3000-5b5b-11eb-8eb0-947cc225af05.png" width="500" height="170"/> <br>

#### 6. 구조도
<img src="https://user-images.githubusercontent.com/72846750/105805859-38809600-5fe6-11eb-8128-bed4bc8f39eb.png" width="500" height="610"/> <br>


#### 7. 최종 모델
총 4가지를 모델로 다음과 같은 성과를 거두었으며, 그 중에서도 LightGBM이 가장 높은 성능을 보임. <br>
<img src="https://user-images.githubusercontent.com/72846750/108803330-c3e94900-75dd-11eb-9504-f51755183875.JPG" width="450" height="120"/> <br>

#### 참조
1) Cross-Validation for Imbalanced Datasets: Avoiding Overoptimistic and Overfitting Approaches<br>
https://www.researchgate.net/publication/328315720_Cross-Validation_for_Imbalanced_Datasets_Avoiding_Overoptimistic_and_Overfitting_Approaches<br>

#### 기여자
* 김준성(a.k.a 튜닝몬스터) https://github.com/whistle-boy
* 방희란(a.k.a 판다스의 신) https://github.com/Heeran-cloud
* 정혜주(a.k.a 논문통찰자) https://github.com/hjung53
