# Lpoint_Big_Comp_2022

◾ **프로젝트 목적**

- RFM (기업 매출 기여도) 기반으로 고객 등급화 진행 후, 고객 등급 예측 모델 개발
- 상위 등급별 군집 분석을 통해 고객층을 세분화하여 마케팅 전략 수립

◾ **데이터 셋**

- 제공: 롯데멤버스
- 사용 데이터: 고객 데모 정보, 상품 구매 정보, 제휴사 이용 정보, 상품 분류 정보, 점포 정보, 엘페이 이용
- 데이터 형식: csv

◾ **프로젝트 과정 (1. RFM 기반 고객 등급화)**

- 데이터 EDA 및 전처리 (pandas, seaborn 등 이용)
- 고객별 Recency, Frequency, Monetary 값 추출 (pandas 등 이용)
- 고객 군집화 진행 (K-means 이용)
- 군집별 등급화 및 점수화 진행 (pandas 등 이용)

◾ **프로젝트 과정 (2. 고객 등급 예측 모델 개발)**

- feature 생성 및 전처리 (pandas, sklearn 등 이용)
(ex) 고객 장바구니 평균 상품 개수, 주요 구매 시간대, 2회 이상 구매 품목 수 외 총 12개 생성
- 모델 학습 및 평가 (XGBoost 이용하여 Classification 진행)

◾ **프로젝트 과정 (3. 상위 등급 고객 군집 세분화 분석)**

- 매출 기여도 비율을 기반으로 상위 두 그룹만 마케팅 진행
- 각 그룹 고객 군집 세분화하여 주요 feature 추출 (K-means, PCA, seaborn 등 이용)
- 세그먼트 된 고객 군집별 마케팅 전략 제시

◾ **결론**

- 전체 고객 4등급으로 분류 (상위 두 그룹이 전체 매출 약 73% 차지)
- 예측 모델 Training set 정확도 86%, Test set 정확도 78%
- 상위 2그룹을 세분화 분석하여, 고객들의 연령층, 주요 이용 유통사, 소비 패턴 등을 파악
- 최종적으로 롯데 브랜드 충성 고객층, 고급 명품 상품 구매 고객층 등으로 고객 세그먼트 및 마케팅 전략 제시
