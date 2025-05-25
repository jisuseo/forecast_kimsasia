📈 forecast_kimsasia
킴스아시아 물류 데이터 분석 및 예측 프로젝트 (개선된 버전)

📋 프로젝트 개요
forecast_kimsasia는 킴스아시아의 구매 및 수요 데이터를 기반으로 데이터 전처리, 탐색적 분석, 시각화 및 예측 모델링을 수행한 프로젝트입니다.
**랜덤 포레스트 회귀(RandomForestRegressor)**와 Prophet 시계열 분석을 적용하여,
물류 데이터의 패턴을 이해하고, 미래 수요를 예측하려는 시도를 포함합니다.

🔍 주요 내용 및 개선 포인트
📊 데이터 전처리 및 탐색적 분석

결측치 처리, 날짜 컬럼(BDaAU, BDaRG) 변환, 불필요 열 제거, 이상치 탐지

공급자별, 제품별, 월별 데이터 분포 및 매출 기여도 분석

🎯 랜덤 포레스트 기반 수요 예측

날짜(BDaAU)를 숫자(ordinal)로 변환하여 학습

RandomForestRegressor를 이용해 미래 수요량(Menge) 예측

실제값과 예측값의 평균제곱오차(MSE) 계산 및 산포도 시각화로 비교

🔮 Prophet 시계열 예측 추가

날짜(BDaAU)와 수량(Menge)으로 Prophet 시계열 모델 학습

미래 1년치 수요량을 예측하고 시각화

실제값과 Prophet 예측값 비교 그래프 추가

🖼️ 시각적 결과

공급자별 매출 기여도, 제품별 매출 및 주문량 상위, 월별 트렌드 그래프

랜덤 포레스트 예측 및 Prophet 예측 결과 비교 시각화

🛠️ 사용 기술 및 라이브러리
Python: Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, Prophet

예측 모델: RandomForestRegressor, Prophet

시각화: Matplotlib, Seaborn

환경: Google Colab (또는 로컬 Python)

📊 예측 결과 예시 (추가할 이미지)
✅ 랜덤 포레스트: 실제 vs 예측 산포도

✅ Prophet: 미래 1년치 수요 예측 그래프

✅ Prophet: 실제값 vs 예측값 비교 라인차트
(포트폴리오용 스크린샷 추가 예정)

📂 데이터
20.10.2022-03.12.2024_purchase.csv: 구매 데이터

20.10.2022-03.12.2024_demand.csv: 수요 데이터

🚀 향후 발전 방향
ARIMA, Prophet 등 다양한 시계열 모델을 비교 적용

제품별/공급자별 특성을 반영한 예측 모델 고도화

Power BI, Tableau를 통한 대시보드 구축 및 자동화 보고서 생성

주간/월간 자동화된 데이터 업데이트 및 예측 프로세스 구현

🔗 포트폴리오 메인으로 돌아가기

