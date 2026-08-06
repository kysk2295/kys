# LearningOS Book Workflow

LearningOS의 최종 산출물은 Day별 PDF 묶음이 아니라 **과정별 한 권의 누적 교재**입니다.

## 원칙

```text
Day 시작
→ 초기 교재
→ 학습/질문
→ Day 완료
→ 최종 교재
→ PDF
→ GitHub
→ Book 누적
```

## 책 이름

- APEX → **AI Paper Journey**
- ATLAS → **Data Analytics Journey**

향후 다른 프로젝트도 같은 방식으로 과정별 Book을 가질 수 있습니다.

## Day 확정판

`<PROJECT> Day N 완료`가 실행되면 그 Day는 다음 요소를 갖춘 확정판으로 정리합니다.

- 이야기 흐름이 앞 Day와 자연스럽게 연결될 것
- 질문에서 나온 쉬운 설명이 본문에 흡수될 것
- 핵심 개념과 전문 용어가 모두 포함될 것
- 실제 논문/프로젝트 사례가 포함될 것
- 오해하기 쉬운 포인트가 포함될 것
- 5문장 요약과 설명형 복습 문제가 포함될 것
- 다음 Day의 질문으로 자연스럽게 끝날 것

## Book 누적 규칙

Book은 Day 문서를 단순 결합하지 않습니다.

누적할 때 다음을 정리합니다.

1. Day 사이의 반복 설명 제거
2. 이전 Day에서 이미 배운 용어는 짧게 연결
3. Chapter 제목과 번호 통일
4. 앞뒤 연결 문장 추가
5. 그림/표 번호 정리
6. 용어사전 후보 누적
7. 참고 논문/프로젝트 출처 누적
8. 주차별 큰 흐름을 Part 단위로 묶기

## 명령어

```text
APEX Book
ATLAS Book
```

이 명령은 지금까지 완료된 Day를 기준으로 누적본을 정리하는 의미로 사용합니다.

30일 완료 시 최종적으로 다음을 목표로 합니다.

```text
AI Paper Journey v1.0
Data Analytics Journey v1.0
```

각 책은 별개의 강의 노트가 아니라 처음부터 끝까지 이어지는 한 권의 입문서가 되어야 합니다.
