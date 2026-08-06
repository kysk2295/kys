# LearningOS Projects

LearningOS는 여러 학습 과정을 동시에 운영하기 위해 프로젝트 코드를 사용합니다.

| 코드 | 이름 | 설명 |
|---|---|---|
| APEX | AI Paper Explorer | AI 기초부터 실제 논문 읽기까지 |
| ATLAS | Data Analytics | 데이터 분석 기초부터 프로젝트까지 |
| ORION | GitHub Explorer | 저장소 구조, 코드, 아키텍처 분석 |
| TITAN | AI Agent Builder | Agent 설계, 도구 사용, 메모리, 평가, 구현 |
| NOVA | Math Foundations | AI/데이터 분석에 필요한 수학 기초 |
| LUMEN | LLM Internals | Transformer/LLM 내부 동작 심화 |

## 공통 운영 규칙

모든 프로젝트는 같은 명령 체계를 사용합니다.

```text
<PROJECT> 시작
<PROJECT> 계속
<PROJECT> 질문
<PROJECT> 복습
<PROJECT> 시험
<PROJECT> 진도
```

각 과정은 독립적이지만 필요하면 서로 연결합니다.

예:

```text
APEX에서 Attention을 배움
→ NOVA에서 내적을 보충
→ LUMEN에서 Multi-Head Attention을 심화
→ TITAN에서 Agent의 LLM 모듈로 연결
```

즉, LearningOS는 여러 과정을 따로 암기하는 시스템이 아니라 서로 연결되는 개인 학습 지도입니다.

## 새로운 과정 추가

새 과정이 필요하면 새로운 코드와 목표를 정의합니다.

예시:

```text
새 과정 코드: SQLX
목표: SQL 실무 분석
기간: 20일
최종 결과: 실제 데이터셋 분석 프로젝트
```

그 뒤 기존 공통 명령 체계를 그대로 사용할 수 있습니다.
