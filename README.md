# SOCAR 보험사기 예측 프로젝트
해당 프로젝트는 패스트캠퍼스 데이터사이언티스트 15기 과정중 진행.<br>
본 프로젝트는 머신러닝을 기반으로 카쉐어링업계에서 극심해지는 보험 사기를 예측해보기 위함에 있음.<br>

## 발표 자료
첨부.<br>

## 데이터 수집
데이터는 카쉐어링 기업 SOCAR로부터 제공받았으며, 16,000 rows X 35 columns의 데이터임.<br>

## 데이터 불균형
전체 16,000건의 데이터중에서 보험사기는 단 41건. <br>
<img src="https://user-images.githubusercontent.com/72846750/105158413-4ac78380-5b51-11eb-8d2e-8b9462323210.png" width="300" height="200"/>

## 평가 기준
이전 기수인 14기에서 본 프로젝트로 얻었던 최적의 성능을 Baseline 으로 두었음.
  - accuracy 0.493, precision 0.003, recall 0.714
데이터 불균형으로, 모든 사고를 No Fraud 로 예측시, accuracy 0.997. 객관적인 성능 평가를 위하여 precision, recall 을 평가 기준으로 결정.
  <img src="https://user-images.githubusercontent.com/72846750/105166682-0b9e3000-5b5b-11eb-8eb0-947cc225af05.png" width="600" height="200"/> <br>

## 구조도
<img src="https://user-images.githubusercontent.com/72846750/105805859-38809600-5fe6-11eb-8128-bed4bc8f39eb.png" width="650" height="760"/> <br>

## 과정
- 데이터 탐색
- 데이터 전처리
- 모델링
- 모델 검증
- 결론

## 최종 모델
본 프로젝트에서는 사용된 모델과 최종 성능은 아래와 같음. <br>
<img src="https://user-images.githubusercontent.com/72846750/108803330-c3e94900-75dd-11eb-9504-f51755183875.JPG" width="600" height="200"/> <br>

## 참조
1) https://www.researchgate.net/publication/328315720_Cross-Validation_for_Imbalanced_Datasets_Avoiding_Overoptimistic_and_Overfitting_Approaches <br><br>

## 기여자
* 김준성(a.k.a 튜닝몬스터) https://github.com/whistle-boy
* 방희란(a.k.a 판다스의 신) https://github.com/Heeran-cloud
* 정혜주(a.k.a 논문통찰자) https://github.com/hjung53
