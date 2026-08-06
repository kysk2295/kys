# ATLAS 30-Day Roadmap

> 데이터는 왜 우리를 속이고, 모델은 왜 운영에 들어가면 조용히 망가질까?

ATLAS는 `delayed-label-monitoring` 프로젝트를 하나의 실전 교과서처럼 사용합니다. 각 Day는 앞날의 질문이 다음 날의 주제로 이어지도록 설계합니다.

## Part 1 — 데이터는 왜 자꾸 우리를 속일까? (Day 1–6)

| Day | 이야기 제목 | 핵심 개념 | 프로젝트 연결 |
|---|---|---|---|
| 1 | 좋은 분석은 코드보다 질문에서 시작한다 | target, unit of analysis, observation/prediction window, leakage | 기업 부실을 언제 예측하는가 |
| 2 | 데이터 한 행은 대체 무엇을 뜻할까? | grain, entity, event, snapshot, primary/composite key, duplicate | 같은 식별자가 여러 재무제표 맥락에 존재 |
| 3 | 결측치와 이상치는 그냥 지우면 될까? | missingness, outlier, clipping, winsorization, rare binary | F-020 희귀 이진값 clipping |
| 4 | 데이터는 언제 존재하게 되었을까? | event time, ingestion time, available time, effective time, PIT | 공시 시차와 PIT correctness |
| 5 | 미래를 몰래 보면 성능이 좋아진다 | target leakage, look-ahead bias, survivorship bias | PIT 위반 약 8% 성능 부풀림 |
| 6 | 숫자가 이상하면 코드보다 먼저 의심하라 | schema/range/cardinality/volume/distribution checks | 782% coverage, 표본 0건 등 |

## Part 2 — 모델 성능 숫자는 왜 거짓말할까? (Day 7–12)

| Day | 이야기 제목 | 핵심 개념 | 프로젝트 연결 |
|---|---|---|---|
| 7 | Accuracy 95%인데 왜 쓸모없을까? | class imbalance, confusion matrix, precision, recall, specificity | 희귀 부실 이벤트 |
| 8 | ROC-AUC와 PR-AUC는 같은 성능표가 아니다 | ROC, PR, prevalence, baseline | 부실 예측 평가 |
| 9 | PR-AUC가 올랐는데 모델은 안 좋아졌다 | prevalence sensitivity, metric contamination | F-013 |
| 10 | Lift는 왜 필요한가? | lift, gain, ranking performance | PR-AUC ÷ prevalence |
| 11 | 확률 80%는 정말 80%일까? | calibration, Brier, reliability, Platt, isotonic | F-019 balanced output 해석 위험 |
| 12 | Threshold를 정하는 순간 비즈니스 문제가 된다 | FP/FN cost, operating point, alert budget | F-011 synthetic threshold 이전 실패 |

## Part 3 — 시간 데이터에서는 검증 방식이 달라진다 (Day 13–17)

| Day | 이야기 제목 | 핵심 개념 | 프로젝트 연결 |
|---|---|---|---|
| 13 | 랜덤 분할이 미래를 훔쳐보게 만들 수 있다 | random vs temporal split, rolling/expanding window | 연도 기반 기업 데이터 |
| 14 | 과거에서 미래로 걸어가는 검증 | walk-forward validation | 월별 115개 checkpoint |
| 15 | 1년 뒤 부실과 3년 뒤 부실은 같은 문제가 아니다 | prediction horizon, label maturity | 365/730/1095일 horizon |
| 16 | 한 시기의 성능만 보고 모델을 믿지 마라 | regime change, structural break, stability | 시기별 성능 차이 |
| 17 | Backtest가 좋아 보여도 과적합일 수 있다 | selection bias, multiple testing, benchmark choice | 분석 조건 선택 위험 |

## Part 4 — 모델은 운영에 들어가면 왜 조용히 망가질까? (Day 18–23)

| Day | 이야기 제목 | 핵심 개념 | 프로젝트 연결 |
|---|---|---|---|
| 18 | MLOps는 배포 버튼이 아니다 | training/inference/feature pipeline, registry, observability | 연구→운영 콘솔 전환 |
| 19 | 입력 데이터가 달라지기 시작했다 | data drift, covariate shift, PSI, KS, Wasserstein | 자연 구간 drift 지표 |
| 20 | 데이터는 비슷한데 정답 규칙이 바뀌었다 | concept drift, P(X), P(Y\|X) | 모델 관계 변화 |
| 21 | 정답이 1~3년 뒤에 도착한다면? | delayed label, immature label, feedback window | 프로젝트 핵심 문제 |
| 22 | 정답 없이 성능 저하를 감지할 수 있을까? | proxy metric, prediction drift, monitoring limits | 자연 AUC 0.685, 높은 오경보 |
| 23 | 일부 정답만 먼저 오면 무엇이 달라질까? | partial labels, delayed feedback estimation | 부분 라벨 36.7% 개선 |

## Part 5 — 실제 MLOps 시스템은 어떻게 유지되는가? (Day 24–27)

| Day | 이야기 제목 | 핵심 개념 | 프로젝트 연결 |
|---|---|---|---|
| 24 | Feature가 바뀌면 모델도 사실 다른 모델이다 | data/feature contract, schema, versioning | 운영 DB 적재 계약 |
| 25 | 같은 실험을 6개월 뒤 다시 만들 수 있는가? | model/data/code version, seed, artifact, lineage | 재현성·캐시 검증 |
| 26 | Dashboard는 예쁜 그래프가 아니라 조사 도구다 | dashboard, alert, triage, investigation, escalation | Streamlit 운영 콘솔 |
| 27 | 장애는 모델 밖에서도 발생한다 | logs, metrics, retry, timeout, cache, smoke test | F-001/F-009/F-016/F-018 |

## Part 6 — 분석가에서 ML 시스템 사고로 (Day 28–30)

| Day | 이야기 제목 | 핵심 개념 | 프로젝트 연결 |
|---|---|---|---|
| 28 | 좋은 분석은 반증 가능한 가설을 만든다 | hypothesis, control, confounder, ablation, sensitivity | PIT 효과의 1~3월 집중 가설 |
| 29 | 틀린 결론을 고치는 것도 분석 실력이다 | uncertainty, caveat, descriptive vs causal language, reproducible reporting | 주 결론 수정 과정 |
| 30 | 처음부터 다시 보면 프로젝트가 다르게 보인다 | end-to-end system review | delayed-label-monitoring 전체 리뷰 |

## Day 30 최종 리뷰 프레임

```text
문제 정의
→ 데이터 grain/key
→ 라벨 정의
→ 시간 정합성/PIT
→ survivorship bias
→ 전처리/feature
→ validation
→ metric
→ calibration
→ drift
→ delayed labels
→ monitoring
→ alert design
→ reproducibility
→ productization
→ failures
→ lessons learned
```

## 최종 통과 기준

30일 후 아래 질문에 스스로 답할 수 있으면 ATLAS 1단계를 완료한 것으로 봅니다.

1. 이 데이터 한 행은 정확히 무엇을 의미하는가?
2. 이 시점에 이 정보가 실제로 존재했는가?
3. 이 평가 지표는 표본 구성에 영향을 받는가?
4. 이 검증 방식은 미래 정보를 누설하지 않는가?
5. 모델의 확률은 calibration 되어 있는가?
6. 운영 중 입력 분포가 변하면 무엇을 볼 것인가?
7. 정답이 늦게 도착할 때 무엇을 알고 무엇을 모르는가?
8. 경보가 울리면 사람이 어떤 순서로 조사할 것인가?
9. 6개월 후 같은 결과를 재현할 수 있는가?
10. 이 결과를 어디까지 주장할 수 있고 어디부터는 주장하면 안 되는가?
