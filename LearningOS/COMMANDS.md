# LearningOS Commands

모든 과정은 **프로젝트 코드 + 공통 명령어**를 사용합니다.

## 기본 명령

```text
<PROJECT> 시작
<PROJECT> 계속
<PROJECT> Day 3
<PROJECT> Day 3 Session 2
<PROJECT> 질문: ...
<PROJECT> 복습
<PROJECT> 시험
<PROJECT> 심화
<PROJECT> 사전 <용어>
<PROJECT> 진도
<PROJECT> PDF
<PROJECT> Day 3 완료
```

예시:

```text
APEX 시작
APEX 계속
APEX Day 12 Session 3
APEX 질문: QKV가 아직 헷갈려
APEX 사전 Residual Connection
APEX 복습
APEX 시험
APEX PDF
```

다른 프로젝트도 같은 방식입니다.

```text
ATLAS 계속
ORION 질문: 이 저장소의 entry point가 어디야?
TITAN 심화
NOVA 사전 내적
```

## 권장 명령

### `시작`
해당 과정의 첫 진입. 과정의 목표와 현재 진도를 확인한 뒤 첫 학습 세션을 시작합니다.

### `계속`
마지막으로 학습한 Day/Session 다음 지점부터 이어갑니다.

### `Day N`
원하는 Day로 바로 이동합니다.

### `Day N Session M`
하루를 나눈 특정 세션부터 시작합니다.

### `질문`
현재 과정의 문맥을 유지한 채 질문합니다. 가능하면 막힌 문장이나 개념을 그대로 붙여 넣습니다.

### `복습`
최근 학습 내용의 핵심 개념, 연결 관계, 놓친 포인트를 다시 확인합니다.

### `시험`
암기보다 설명 중심으로 이해도를 확인합니다.

### `심화`
현재 개념을 한 단계 더 깊게 봅니다. 기본 진도를 방해하지 않도록 선택 학습으로 취급합니다.

### `사전`
용어를 쉬운 말 → 비유 → 구조 → 논문 표현 순으로 설명합니다.

### `진도`
현재 Day, Session, 완료 범위, 약한 개념을 확인합니다.

### `PDF`
채팅에서 실제로 공부한 내용과 질문·보충 설명을 반영한 복습용 PDF를 생성합니다.

### `완료`
해당 Day의 학습을 마치고 이해도와 약한 개념을 기록한 뒤 다음 Day로 연결합니다.

## 짧은 명령도 허용

문맥이 분명할 때는 다음처럼 자연어로 입력해도 됩니다.

```text
APEX 이어서 하자
APEX 오늘 공부 시작
APEX 방금 내용 시험 봐줘
APEX 이 부분 더 쉽게
```

단, 여러 과정을 동시에 진행하므로 `Day 1 시작`보다 `APEX Day 1 시작`처럼 프로젝트 코드를 붙이는 것을 기본 규칙으로 합니다.
