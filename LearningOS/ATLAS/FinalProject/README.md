# ATLAS Final Project — delayed-label-monitoring 재해석

Day 30에는 `delayed-label-monitoring`을 코드 저장소가 아니라 하나의 ML 시스템 사례로 다시 읽습니다.

## 최종 리뷰 질문

1. 문제 정의는 무엇인가?
2. 한 행의 grain은 무엇인가?
3. label은 언제 성숙하는가?
4. point-in-time correctness는 어떻게 보장하는가?
5. survivorship bias는 어디서 생길 수 있는가?
6. 어떤 metric을 왜 선택했는가?
7. prevalence 변화가 metric 해석에 어떤 영향을 주는가?
8. calibration과 ranking은 어떻게 다른가?
9. walk-forward validation은 왜 필요한가?
10. data drift와 concept drift를 어떻게 구분하는가?
11. delayed label 때문에 무엇을 직접 측정할 수 없는가?
12. partial label은 어떤 정보를 추가하는가?
13. alert는 어떻게 조사 workflow로 이어지는가?
14. 재현성을 위해 어떤 artifact와 version이 필요한가?
15. 실패 기록에서 가장 일반화 가능한 교훈은 무엇인가?

## 최종 결과물

```text
1. 시스템 구조도 1장
2. 프로젝트 리뷰 2~4페이지
3. 핵심 개념 사전
4. 실패 사례 Top 10과 교훈
5. 운영 모니터링 설계안
6. 5분 설명 스크립트
```

## 최종 목표

다음 문장을 자신의 말로 확장해서 설명할 수 있어야 합니다.

> 이 프로젝트는 단순한 부실 예측 모델이 아니라, 시점 정합성이 보장된 데이터를 만들고 희귀 이벤트 모델을 올바르게 평가하며, 정답이 늦게 도착하는 환경에서 모델 상태를 운영적으로 감시하는 ML 시스템 문제다.
