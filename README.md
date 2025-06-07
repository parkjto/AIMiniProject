# 정형 데이터 회귀 분석

## 문제 정의
정형 데이터 회귀  
입력 변수 : MYCT, MMIN, MMAX, CACH, CHMIN, CHMAX  
출력 변수 : PRP

## 데이터 설명
데이터 개수:  총 209개 샘플  
속성: 6개의 입력변수, 1개의 출력변수  
80% 학습, 20% 테스트  
학습 데이터 내 25%

## 전처리 과정 
불필요한 컬럼 제거 : vendor, model, ERP  
MinMaxScaler 사용하여 0~1 범위로 정규화 수행

## 최종 하이퍼 파라미터
Earlystopping : val_loss가 20회 연속 개선되지 않으면 학습 중단

## 최종 성능 
Test 1의 MSE가 가장 낮다 따라서 Test 1의 구조가 가장 적합하다
