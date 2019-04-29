# **서울시 공공자전거 편중 해소 방안 제안**

공공자전거는 편도 형식으로 이용하여 대여/ 반납의 편중이 심한 대여소들이 존재한다. <br>
또한,	24시간 사람이 서울시 전체 2천 곳이 넘는 대여소를 실시간 모니터링하여 편중을 해소하고 있어 효과적이지 못하다. <br>

**목표**: 자전거 수요 예측 모델 개발 및 편중 해소 아이디어 제안 <br>
**과정**
1. 사용언어 & 툴: R, Python, TensorFlow, Keras, MS Excel
2. 데이터 수집: 서울시 열린데이터광장 (공공자전거 대여이력 정보), 기상청 (기상 데이터)
3. 데이터 전처리: 특성공학을 통한 변수 추가 (캘린더 변수), 시각화를 통한 수요 예측이 필요한 요일 및 시간대 도출, 사회 네트워크 분석을 통한 대여소의 권역 군집화, 대여소의 이용패턴별 군집화
4. 데이터 분석: 1차, 2차 linear regression 및 RNN을 활용한 대여소의 수요 예측 모델링 

**성과**
1.	자전거의 왕래가 많은 대여소끼리의 군집화를 통해 권역을 구성
2. 이용패턴이 비슷한 대여소끼리 군집화
3. 대여가 가장 많은 113번 대여소의 수요 예측 모델 개발
4. 아이디어 제안: 수요가 많을 것으로 예상되는 대여소로 시민들이 공공자전거를 이동시킬 수 있는 편도 무료이용 서비스 및 마일리지 서비스를 제안 <br>

**논의**<br>
권역 군집화 결과를 통해 각 권역 내 편중 해소 관리소의 최적 위치 선정시, 해당 관리소에서 권역 내 편중이 심한 대여소의 수요를 미리 예측하고 조치를 취하여 편중을 해소 할 수 있을 것으로 예상

---
**Contents**

1. 라이브러리 로드
2. 데이터 적재
3. 데이터 정제
4. 특성 공학 (변수 추가)
5. 자전거 이용량 시각화
6. 특성 공학 (데이터 가공)
7. 특성 공학 (변수 추가)
8. 자전거 편중 시각화
9. 네트워크 분석을 통한 군집화 결과 로드
10. 권역별 주요 편중 시간대 시각화
11. 특성 공학 (변수 추가)
12. 특정 대여소 수요 예측 모델링
