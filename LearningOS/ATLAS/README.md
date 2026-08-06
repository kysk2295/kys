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

ATLAS의 Day는 처음부터 고정된 PDF를 읽는 방식이 아닙니다.

```text
ATLAS Day N 시작
→ 채팅에서 초기 교재 생성
→ 읽으면서 질문
→ 쉬운 설명과 실제 프로젝트 사례 보강
→ ATLAS Day N 완료
→ 질문을 반영한 최종 교재
→ PDF 생성
→ GitHub에 Day 확정판 누적
→ Data Analytics Journey Book에 편입
```

각 Day는 약 3~4시간 분량이며, 여러 Chapter로 나눠 웹/모바일에서 이어서 공부할 수 있습니다.

```text
오늘의 문제
→ 가장 기초적인 배경
→ 핵심 개념
→ 그림/표
→ delayed-label-monitoring 실제 사례
→ 실패 사례
→ 실무/운영 연결
→ 복습
→ 다음 Day 떡밥
```

코드가 필요한 날도 있지만 ATLAS의 중심은 코드 암기가 아니라 **데이터와 모델을 의심하고 검증하는 사고방식**입니다.

## 주요 명령

```text
ATLAS 시작
ATLAS Day 1 시작
ATLAS 계속
ATLAS Day 9 Chapter 2
ATLAS 질문: PR-AUC와 양성률 관계가 이해 안 돼
ATLAS 복습
ATLAS 시험
ATLAS 심화
ATLAS 진도
ATLAS Day 1 완료
ATLAS PDF
ATLAS Book
```

`ATLAS Day N 완료`가 정식 마감 명령입니다. 해당 Day에서 나온 질문과 보충 설명을 반영해 확정판을 만들고, 이후 PDF와 Book에 누적합니다.

전체 일정은 [`ROADMAP.md`](./ROADMAP.md), 누적 책 상태는 [`BOOK.md`](./BOOK.md)를 참고하세요.
