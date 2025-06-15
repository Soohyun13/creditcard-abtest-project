# 🧠 신용카드 고객 이탈 예측 및 개선 전략 분석

> **신용카드 거래 데이터를 활용한 고객 이탈 예측 모델링 및 A/B 테스트 프로젝트**

---

## 📌 프로젝트 개요

고객 이탈은 금융 산업에서 수익 손실과 직결되는 핵심 문제입니다.  
본 프로젝트에서는 신용카드 사용자 데이터를 기반으로 고객의 이탈 여부를 예측하고,  
A/B 테스트 설계를 통해 이탈 방지를 위한 전략 수립 가능성을 검토합니다.

---

## 🎯 목표

- 고객 이탈 여부를 예측하는 분류 모델 구축  
- 고객 특성 및 거래 행동 기반으로 주요 이탈 요인 도출  
- 개선 전략의 효과를 검증하기 위한 A/B 테스트 시나리오 설계

---

## 📂 데이터 개요

- **데이터셋**: [BankChurners.csv (Kaggle)](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers)  
- **총 샘플 수**: 약 10,000건  
- **주요 변수**:
  - `Attrition_Flag`: 고객 이탈 여부 (이진 분류 대상)
  - `Customer_Age`, `Gender`, `Income_Category`, `Months_on_book` 등 고객 메타 정보
  - `Total_Trans_Ct`, `Total_Revolving_Bal`, `Avg_Open_To_Buy` 등 거래 행동 변수

---

## 🛠 사용 기술

- **언어/환경**: Python (Jupyter Notebook)
- **데이터 처리**: pandas, numpy
- **시각화**: matplotlib, seaborn
- **모델링**: scikit-learn (Logistic Regression, RandomForestClassifier), XGBoost
- **성능 평가**: Accuracy, F1 Score, Confusion Matrix
- **기타**: Label Encoding, StandardScaler, K-Fold Cross Validation

---

## 🧪 분석 및 모델링 과정

1. **데이터 전처리**
   - 불필요한 변수 제거 및 결측값 처리
   - 범주형 변수 인코딩 (LabelEncoder)
   - 수치형 변수 정규화 (StandardScaler)

2. **EDA (탐색적 데이터 분석)**
   - 고객군별 이탈율 확인
   - 변수별 분포 및 상관관계 시각화

3. **이탈 예측 모델링**
   - Logistic Regression, Random Forest, XGBoost 모델 비교
   - K-Fold 교차 검증 기반 성능 비교
   - F1 Score 기준 최적 모델 선정

4. **A/B 테스트 설계**
   - 캠페인 메시지/혜택 적용 그룹 분리 시나리오 작성
   - 이탈율 비교를 통한 전략 효과 평가 구조 제안

---

## 📈 성과 및 인사이트

- 최종 모델 F1 Score 기준 안정적 성능 확보
- `Total_Trans_Ct`, `Customer_Age`, `Credit_Limit` 등 주요 변수들이 이탈과 밀접한 상관관계를 가짐
- 단순 예측을 넘어, 실질적인 고객 유지 전략으로 확장 가능한 A/B 테스트 기반 제안 도출

---

## 🙌 팀원

- 김수현 외 2인

---

## 📌 폴더 구조 예시

📁 Final_Project
│
├── 📜 CreditCard_A/BTest_Project.ipynb # 전체 분석 코드
├── 📜 README.md # 프로젝트 소개 문서


---
