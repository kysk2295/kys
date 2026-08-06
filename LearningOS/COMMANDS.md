# LearningOS Commands

LearningOS의 모든 과정은 **프로젝트 코드 + 공통 명령어**를 사용합니다.

핵심 운영 방식은 다음과 같습니다.

```text
Day 시작
→ 채팅에서 오늘 교재 생성
→ 질문하면서 학습
→ Day 완료
→ 질문·보충설명 반영 최종본 생성
→ PDF 생성
→ GitHub 누적
→ Book에 편입
```

## 기본 명령

```text
<PROJECT> 시작
<PROJECT> 계속
<PROJECT> Day 3 시작
<PROJECT> Day 3 Chapter 2
<PROJECT> 질문: ...
<PROJECT> 복습
<PROJECT> 시험
<PROJECT> 심화
<PROJECT> 사전 <용어>
<PROJECT> 진도
<PROJECT> Day 3 완료
<PROJECT> PDF
<PROJECT> Book
<PROJECT> 로드맵
```

예시:

```text
APEX Day 1 시작
APEX 질문: Tensor와 Matrix 차이가 아직 헷갈려
APEX 계속
APEX Day 1 완료
APEX Book

ATLAS Day 1 시작
ATLAS 질문: PIT가 왜 leakage인지 모르겠어
ATLAS Day 1 완료
ATLAS Book
```

## 명령어 의미

### `<PROJECT> 시작`
과정의 첫 진입입니다. Day 0 또는 현재 첫 미완료 Day를 안내합니다.

### `<PROJECT> Day N 시작`
해당 Day의 **초기 교재를 채팅에서 생성하고 학습을 시작**합니다.

초기 교재는 완성본이 아닙니다. 실제 질문과 막힌 지점을 수집하기 위한 학습 버전입니다.

### `<PROJECT> 계속`
마지막으로 공부하던 Day/Chapter부터 이어갑니다.

### `<PROJECT> Day N Chapter M`
원하는 위치로 직접 이동합니다.

### `<PROJECT> 질문`
현재 Day의 문맥을 유지한 채 질문합니다. 답변에서 나온 쉬운 비유, 추가 그림, 오해 교정은 Day 최종본 후보로 누적합니다.

### `<PROJECT> 복습`
최근 학습한 내용을 핵심 흐름 중심으로 다시 정리합니다.

### `<PROJECT> 시험`
암기형보다 설명형 문제를 중심으로 이해도를 확인합니다.

### `<PROJECT> 심화`
현재 개념을 한 단계 더 깊게 봅니다. 기본 진도를 방해하지 않는 선택 학습입니다.

### `<PROJECT> 사전 <용어>`
용어를 쉬운 말 → 비유 → 구조 → 실제 사용 → 전문 표현 순으로 설명합니다.

### `<PROJECT> 진도`
현재 Day, Chapter, 완료 Day, 약한 개념, 다음 권장 위치를 확인합니다.

### `<PROJECT> Day N 완료`
해당 Day를 마감합니다. 이 명령이 핵심입니다.

완료 시 다음을 수행하는 것을 원칙으로 합니다.

```text
1. 오늘의 질문과 추가 설명 회수
2. 초기에 만든 교재를 최종본으로 보강
3. 핵심 오해와 보충 설명 반영
4. 최종 복습 문제와 5문장 요약 추가
5. PDF 생성
6. GitHub Day 폴더 업데이트
7. 누적 Book 원고에 해당 Day 편입
8. 다음 Day로 이어지는 떡밥 기록
```

### `<PROJECT> PDF`
현재 Day 또는 지정 Day의 최신 확정본을 PDF로 만듭니다. 원칙적으로 `Day N 완료` 뒤에 만드는 PDF가 최종본입니다.

### `<PROJECT> Book`
지금까지 완료된 Day의 확정본을 순서대로 합쳐 **한 권의 누적 교재** 형태로 정리합니다.

예:

```text
APEX Book
→ AI Paper Journey 누적본

ATLAS Book
→ Data Analytics Journey 누적본
```

### `<PROJECT> 로드맵`
30일 전체 구조와 현재 위치를 함께 확인합니다.

## 짧은 자연어 명령도 허용

문맥이 분명하면 다음처럼 말해도 됩니다.

```text
APEX 오늘 시작하자
APEX 이어서 하자
ATLAS 오늘 거 완료 처리해줘
APEX 책 지금까지 합쳐줘
```

다만 여러 과정을 동시에 진행하므로 `Day 1 시작`보다 `APEX Day 1 시작`, `ATLAS Day 1 시작`처럼 프로젝트 코드를 붙이는 것을 기본 규칙으로 합니다.
