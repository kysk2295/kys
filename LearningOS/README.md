# LearningOS

웹·모바일에서 ChatGPT와 함께 여러 학습 과정을 운영하기 위한 개인 학습 시스템입니다.

LearningOS의 핵심은 **프로젝트 코드 + 공통 명령어 + 누적형 커리큘럼**입니다. 여러 과정을 동시에 공부해도 `Day 1`이 어느 과정인지 헷갈리지 않도록 각 과정에 이름을 붙입니다.

## 등록 과정

| 코드 | 과정 | 목적 |
|---|---|---|
| APEX | AI Paper Explorer | AI 기초부터 최신 AI 논문 읽기까지 |
| ATLAS | Data Analytics × ML × MLOps | 데이터 신뢰성, 검증, 모델 평가, 운영 모니터링까지 |
| ORION | GitHub Explorer | GitHub 프로젝트 구조와 코드 분석 |
| TITAN | AI Agent Builder | AI Agent 설계·구현 |
| NOVA | Math Foundations | 수학 기초와 AI 수학 |
| LUMEN | LLM Internals | LLM 내부 구조 심화 |

## 기본 사용법

ChatGPT 웹 또는 모바일에서 아래처럼 입력합니다.

```text
APEX 시작
APEX 계속
APEX Day 3
APEX 질문: Attention이 이해 안 돼

ATLAS 시작
ATLAS 계속
ATLAS Day 9
ATLAS 질문: 왜 PR-AUC가 양성률에 영향을 받아?
```

공통 명령어:

```text
<PROJECT> 시작
<PROJECT> 계속
<PROJECT> Day N
<PROJECT> Day N Session M
<PROJECT> 질문
<PROJECT> 복습
<PROJECT> 시험
<PROJECT> 심화
<PROJECT> 사전 <용어>
<PROJECT> 진도
<PROJECT> PDF
<PROJECT> Day N 완료
```

## 학습 방식

기본 학습 장소는 **ChatGPT 대화 화면**입니다. PC 웹과 모바일 앱에서 같은 대화를 열어 이어서 공부합니다.

각 Day는 긴 요약문을 한 번에 던지는 대신 여러 Session으로 나누고, 앞에서 생긴 질문이 다음 Session과 다음 Day로 이어지게 설계합니다.

```text
Session 1  이야기와 배경
Session 2  핵심 개념
Session 3  실제 논문/프로젝트 탐험
Session 4  현재 활용 + 복습
```

PDF는 선행 교재가 아니라 질문과 보충 설명까지 반영한 **복습용 결과물**로 필요할 때 생성합니다.

## APEX

APEX는 30일 동안 AI 기초부터 실제 최신 논문 읽기까지 가는 과정입니다.

- AI 발전사를 문제→해결의 이야기로 이해
- Transformer, LLM, RAG, Agent 개념 연결
- Abstract, Figure, Method, Experiment, Limitation 읽기
- 핵심 수식을 한국어 문장으로 해석

→ [`APEX/ROADMAP.md`](./APEX/ROADMAP.md)

## ATLAS

ATLAS는 `kysk2295/delayed-label-monitoring`을 메인 실전 사례로 사용하는 30일 Data Analytics × ML × MLOps 과정입니다.

- 데이터 grain/key와 품질
- PIT, leakage, survivorship bias
- ROC-AUC, PR-AUC, Lift, calibration
- temporal split과 walk-forward validation
- data drift와 concept drift
- delayed/partial labels
- feature/data contract, lineage, reproducibility
- monitoring, alert, investigation workflow

목표는 단순히 모델을 만드는 것이 아니라 **데이터와 평가를 믿어도 되는지 판단하고 운영 중 모델을 감시하는 사고방식**을 기르는 것입니다.

→ [`ATLAS/README.md`](./ATLAS/README.md)  
→ [`ATLAS/ROADMAP.md`](./ATLAS/ROADMAP.md)

자세한 공통 명령어는 [`COMMANDS.md`](./COMMANDS.md), 학습 방식은 [`STUDY_WORKFLOW.md`](./STUDY_WORKFLOW.md), 전체 과정 목록은 [`PROJECTS.md`](./PROJECTS.md)를 참고하세요.
