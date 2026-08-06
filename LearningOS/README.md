# LearningOS

웹·모바일에서 ChatGPT와 함께 여러 학습 과정을 운영하기 위한 개인 학습 시스템입니다.

LearningOS의 핵심은 **프로젝트 코드 + 공통 명령어**입니다. 여러 과정을 동시에 공부해도 `Day 1`이 어느 과정인지 헷갈리지 않도록 각 과정에 이름을 붙입니다.

## 등록 과정

| 코드 | 과정 | 목적 |
|---|---|---|
| APEX | AI Paper Explorer | AI 기초부터 최신 AI 논문 읽기까지 |
| ATLAS | Data Analytics | 데이터 분석 학습 |
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
APEX Day 3 Session 2
APEX 질문: Attention이 이해 안 돼
APEX 복습
APEX 시험
APEX 심화
APEX 사전 Transformer
APEX 진도
APEX PDF
APEX Day 3 완료
```

프로젝트 이름만 바꾸면 같은 명령을 다른 과정에도 사용할 수 있습니다.

```text
ATLAS 계속
ORION 질문: 이 repository 구조가 이해 안 돼
TITAN 시험
NOVA 사전 벡터
```

## 학습 방식

기본 학습 장소는 파일이 아니라 **ChatGPT 대화 화면**입니다. PC 웹과 모바일 앱에서 같은 대화를 열어 이어서 공부합니다.

각 Day는 약 4시간 분량이지만 모바일에서도 부담 없이 진행하도록 여러 Session으로 나눕니다.

```text
Session 1  이야기와 배경
Session 2  핵심 개념
Session 3  실제 자료/논문 탐험
Session 4  현재 활용 + 복습
```

PDF는 선행 교재가 아니라, 질문과 보충 설명까지 반영한 **복습용 결과물**로 필요할 때 생성합니다.

## APEX의 목표

APEX는 30일 동안 하루 약 4시간, 총 약 120시간을 공부하는 AI 논문 읽기 과정입니다.

목표는 30일 후 모든 수식을 증명하는 연구자가 되는 것이 아니라, 실제 AI 논문을 열었을 때 다음을 할 수 있는 수준입니다.

- Abstract에서 연구 문제와 핵심 방법 찾기
- 기존 방법의 한계 파악하기
- 모델 구조 그림의 데이터 흐름 따라가기
- Transformer, Attention, Residual, RAG, LoRA, RLHF, Agent 등의 개념 연결하기
- 핵심 수식을 한국어 문장으로 해석하기
- Baseline, Benchmark, Metric, Ablation 등 실험 표 읽기
- 논문의 강점과 한계를 자신의 말로 설명하기
- 새로운 논문에서 모르는 20%를 찾아가며 읽기

APEX는 기술 목록을 암기하는 과정이 아니라 **AI가 어떤 문제를 만나고 어떤 아이디어로 해결해 왔는지 하나의 이야기로 따라가는 과정**으로 설계합니다.

자세한 명령어는 [`COMMANDS.md`](./COMMANDS.md), APEX 운영법은 [`APEX_GUIDE.md`](./APEX_GUIDE.md), 실제 하루 학습 흐름은 [`STUDY_WORKFLOW.md`](./STUDY_WORKFLOW.md)를 참고하세요.
