# SOCAR 보험사기 예측 프로젝트
본 프로젝트는 패스트캠퍼스 데이터사이언스 15기 수업에서 진행되었음.<br>
보험사기로 멍들고 있는 카셰어링 업계에 기여할 수 있기를 희망함.

## 발표 자료
첨부예정.

## 데이터 수집
데이터는 쏘카로부터 제공받았으며, 16,000 rows 와 35 columns 로 구성됨. <br>

## 평가 기준
- 전 기수인 14기에서 본 프로젝트로 얻었던 최적의 성능을 Baseline 으로 두었음.
  - accuracy 0.493, precision 0.003, recall 0.714
- 데이터 불균형이 극심함.
  - 전체 데이터 중 Fraud 는 41개. 모든 사고를 No Fraud 로 예측시, accuracy 0.997.
  - 객관적인 성능 평가를 위하여 precision & recall 을 함께 평가함.
  <img src="https://user-images.githubusercontent.com/72846750/105166682-0b9e3000-5b5b-11eb-8eb0-947cc225af05.png" width="600" height="200"/>

## 구조도
<img src="https://user-images.githubusercontent.com/72846750/105805353-294d1880-5fe5-11eb-83a2-905302636d75.png" width="600" height="900"/>

## 과정
- 데이터 탐색
- 데이터 전처리
- 모델링
- 모델 평가
- 결론

## 상세
- 데이터 탐색
  - 33개 피처 중 별 다른 상관성은 없었음.
  - 데이터 불균형이 극심함.
- 데이터 전처리
  - 여러 전처리를 시도하였으나, 성능은 개선되지 않았음.
  - 최적의 성능을 가져온 전처리는 다음과 같음.

## 참조
1)https://programs.sbs.co.kr/culture/maninblackbox/clip/55706/OC451916010 <br><br>

## 기여자
* 김준성(a.k.a 튜닝몬스터) https://github.com/whistle-boy
* 방희란(a.k.a 판다스의 신) https://github.com/Heeran-cloud
* 정혜주(a.k.a 논문통찰자) https://github.com/hjung53
