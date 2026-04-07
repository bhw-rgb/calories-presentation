# 칼로리 소모량 예측 AI 해커톤

[배경] 
안녕하세요, 칼로리 소모량 예측 AI 해커톤에 오신 것을 환영합니다!

최근에는 건강 관련 애플리케이션에서 칼로리 소모량을 추정하는 AI 모델을 개발하고 사용하는 데 관심이 높아지고 있습니다. 

체중, 성별, 운동기간, 심박수 등 생체 데이터를 기반으로 칼로리 소모량을 예측하는데,

이러한 기술은 개인의 건강과 라이프스타일에 대한 이해를 높일 수 있습니다.

생체 데이터를 이용해 칼로리 소모량 예측 모델을 만들고, 다른 사람들과 인사이트를 겨루며 알고리즘 대회의 즐거움을 느껴 보세요.



[주제]
생체 데이터로부터 칼로리 소모량을 예측하는 AI 알고리즘 개발



[설명]
칼로리 소모량을 회귀 예측하세요.


[주최 / 주관]
데이콘



[참가 대상]
[초격차] AI 헬스케어 머신러닝 트랙 참여자

1. 평가
평가산식 : RMSE(Root Mean Squared Error)
'[초격차] AI 헬스케어 머신러닝 트랙: 칼로리 소모량 예측 AI 해커톤' 은 Public에서 Test 데이터 100%를 활용하여 평가


2. 참여 규칙
개인이나 팀으로 참여 가능
개인 참가 방법: 팀 신청 없이, 자유롭게 제출 창에서 제출 가능
 

3. 외부 데이터 및 사전 학습 모델
외부 데이터 사용 불가
사전 학습 모델(Pre-trained Model) 사용 가능
 

4. 유의 사항
1일 최대 제출 횟수: 3회
모델 학습에서 평가 데이터셋 활용(Data Leakage)시 수상 제외
label encoding, one-hot encoding 시 test 데이터 셋 활용
data scaling 적용 시 test 데이터 셋 활용
test 데이터 셋에 pd.get_dummies() 함수 적용
test 데이터 셋의 결측치 처리 시 test 데이터 셋의 통계 값 활용
위 예시 외에도 test 데이터 셋이 모델 학습에 활용되는 경우에 Data leakage에 해당됨
데이콘은 부정 제출 행위를 금지하며 데이콘 대회 부정 제출 이력 있을 시 평가 제한 (참조: https://dacon.io/notice/notice/13)

Dataset Info.

train.csv [파일]
7500개의 데이터
ID : 샘플 별 고유 id
Exercise_Duration  : 운동 시간(분)
Body_Temperature(F) : 체온
BPM : 심박수
Height(Feet) : 키(피트)
Height(Remainder_Inches) : 키(피트 계산 후 더해야 할 키)
Weight(lb) : 몸무게(파운드)
Weight_Status : 체중 상태
Gender : 성별
Age : 나이
Calories_Burned : 칼로리 소모량(목표 예측값)
 

test.csv [파일]
7500개의 데이터
ID : 샘플 별 고유 id
Exercise_Duration  : 운동 시간(분)
Body_Temperature(F) : 체온
BPM : 심박수
Height(Feet) : 키(피트)
Height(Remainder_Inches) : 키(피트 계산 후 더해야 할 키)
Weight(lb) : 몸무게(파운드)
Weight_Status : 체중 상태
Gender : 성별
Age : 나이


sample_submission.csv [제출양식]
ID : 샘플 별 고유 id
Calories_Burned : 칼로리 소모량(목표 예측값)
