# ATLAS — Data Analytics × ML × MLOps Journey

ATLAS는 LearningOS의 데이터 분석·머신러닝·MLOps 과정입니다.

메인 사례는 [`kysk2295/delayed-label-monitoring`](https://github.com/kysk2295/delayed-label-monitoring)이며, 단순히 pandas나 모델 API를 배우는 것이 아니라 **데이터를 믿어도 되는지 판단하고, 올바르게 검증하고, 운영 환경에서 모델을 감시하는 사고방식**을 기르는 것이 목표입니다.

## 30일 후 목표

ATLAS를 마치면 다음을 설명하고 적용할 수 있는 수준을 목표로 합니다.

- 데이터셋의 grain, key, entity, event, snapshot 구분
- 결측치·이상치·중복·스키마 오류를 의미 중심으로 점검
- Point-in-Time(PIT), target leakage, look-ahead bias, survivorship bias 탐지
- Accuracy, Precision, Recall, ROC-AUC, PR-AUC, Lift의 차이와 한계 해석
- Prevalence 변화가 PR-AUC 해석에 미치는 영향 이해
- Calibration과 ranking 성능의 차이 구분
- Random split과 temporal split의 차이 이해
- Walk-forward validation 설계
- Data drift와 concept drift 구분
- Delayed label 환경에서 가능한 모니터링과 한계 설명
- Feature/data contract, versioning, lineage, reproducibility 개념 이해
- Alert, dashboard, investigation workflow를 포함한 운영 사고
- 실험 결과를 과장하지 않고 caveat와 uncertainty를 함께 전달

## 학습 방식

각 Day는 약 3~4시간 분량으로 다음 흐름을 따릅니다.

```text
1. 오늘의 문제 상황
2. 쉬운 개념 설명
3. 그림/표로 구조 이해
4. delayed-label-monitoring 실제 사례 연결
5. 실패 사례 분석
6. 실무/운영 연결
7. 복습과 설명 연습
```

코드가 필요한 날도 있지만 ATLAS의 중심은 코드 암기가 아니라 **데이터와 모델을 의심하고 검증하는 사고방식**입니다.

## 시작 명령

```text
ATLAS 시작
ATLAS 계속
ATLAS Day 9
ATLAS 질문: PR-AUC와 양성률 관계가 이해 안 돼
ATLAS 복습
ATLAS 시험
ATLAS 심화
ATLAS 진도
ATLAS PDF
```

전체 일정은 [`ROADMAP.md`](./ROADMAP.md)를 참고하세요.
