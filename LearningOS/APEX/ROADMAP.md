# APEX — AI Paper Explorer

## 목표

30일 × 하루 약 4시간, 총 약 120시간 동안 AI의 발전 과정을 하나의 이야기로 따라가며 실제 AI 논문을 읽을 수 있는 기반을 만듭니다.

APEX의 최종 목표는 모든 수식을 증명하는 것이 아니라 다음을 할 수 있는 수준입니다.

- Abstract에서 연구 문제·방법·결과 찾기
- 기존 방법의 한계 설명하기
- 구조 그림의 입력 → 모듈 → 출력 흐름 읽기
- 핵심 수식을 한국어 문장으로 번역하기
- Baseline·Benchmark·Metric·Ablation 읽기
- 최신 논문에서 아는 개념과 새로운 개념 구분하기
- 논문의 핵심과 한계를 자신의 말로 설명하기

## 학습 원칙

기술 목록을 외우지 않습니다. 매일 다음 흐름으로 학습합니다.

```text
문제
→ 기존 방법의 한계
→ 새로운 아이디어
→ 작동 방식
→ 실제 논문
→ 현재 AI에서의 사용
→ 다음 문제
```

## 30일 로드맵

### Part 1 — 컴퓨터는 왜 생각을 못할까?

**Day 1 — AI는 왜 갑자기 세상을 바꿨을까?**
AI 역사, 컴퓨터는 숫자만 본다는 사실, AI/ML/DL/LLM 큰 지도, 논문의 기본 구조. 《Attention Is All You Need》는 제목과 위치만 맛봅니다.

**Day 2 — 숫자는 어떻게 의미가 될까?**
Bit, Byte, Pixel, RGB, Scalar, Vector, Matrix, Tensor, Shape, Dimension, Embedding. BERT와 ViT 그림에서 숫자 표현을 찾아봅니다.

**Day 3 — 컴퓨터는 어떻게 공부를 시작했을까?**
Dataset, Sample, Feature, Label, Model, Weight, Bias, Parameter. Perceptron과 신경망의 출발을 연결합니다.

**Day 4 — AI는 왜 자꾸 틀릴까?**
Prediction, Logit, Softmax, Loss, Gradient, Backpropagation, Optimizer, Learning Rate, Epoch, Batch. Adam 논문을 만납니다.

**Day 5 — AI도 시험 문제를 외울 수 있다**
Train/Validation/Test, Generalization, Overfitting, Regularization, Dropout, Batch Normalization.

**Day 6 — 논문은 어디부터 읽어야 할까?**
Title, Abstract, Introduction, Figure, Method, Experiment, Conclusion, Limitation을 실제 논문에서 찾아봅니다. 첫 미니 논문 읽기.

### Part 2 — 컴퓨터는 사진을 볼 수 있을까?

**Day 7 — 사진은 사실 숫자 덩어리다**
Pixel, RGB Channel, Image Tensor, ImageNet.

**Day 8 — AI에게 돋보기를 주면?**
Filter, Kernel, Convolution, Stride, Padding, Feature Map.

**Day 9 — 선에서 얼굴까지**
ReLU, Pooling, Layer, Hierarchical Feature, Classifier.

**Day 10 — 2012년, AlexNet이 판을 바꿨다**
AlexNet, ImageNet, GPU, Deep CNN. 대표 논문의 Abstract·Figure·결과표를 읽습니다.

**Day 11 — 깊게 만들었는데 왜 더 못할까?**
Deep Network, Backpropagation 재확인, Vanishing Gradient, Degradation Problem.

**Day 12 — ResNet, 지름길을 만들다**
Residual Learning, Skip Connection, `F(x)+x`, 깊은 모델의 학습.

**Day 13 — 이미지 AI의 계보를 읽다**
AlexNet → VGG → GoogLeNet → ResNet → ViT의 문제·아이디어를 연결하고 AlexNet/ResNet 논문을 비교합니다.

### Part 3 — AI는 기억할 수 있을까?

**Day 14 — 문장은 왜 이미지보다 까다로울까?**
Sequence, Token, Vocabulary, Token ID, Embedding, 순서 정보.

**Day 15 — AI에게 작은 메모장을 주다**
RNN, Time Step, Hidden State, Recurrent Connection.

**Day 16 — 기억할 것과 버릴 것을 고르다**
Long-term Dependency, LSTM, Cell State, Input/Forget/Output Gate.

**Day 17 — 영어를 읽고 한국어를 만드는 AI**
Seq2Seq, Encoder, Decoder, Context, Teacher Forcing, Autoregressive Generation.

**Day 18 — 모든 것을 기억하지 말고 다시 보자**
Attention의 등장, Alignment, Attention Weight, Context Vector. Bahdanau Attention 논문과 연결합니다.

**Day 19 — Q, K, V의 비밀**
Query, Key, Value, Dot Product, Scale, Softmax, Self-Attention, Mask.

**Day 20 — Transformer 탄생**
《Attention Is All You Need》를 본격적으로 읽습니다. Multi-Head Attention, Positional Encoding, Feed-Forward, Residual, LayerNorm, Encoder/Decoder 구조를 연결합니다.

### Part 4 — GPT는 왜 세상을 바꿨을까?

**Day 21 — BERT와 GPT는 같은 Transformer인데 왜 다를까?**
Encoder-only, Decoder-only, Bidirectional, Masked Language Modeling, Autoregressive Modeling.

**Day 22 — 먼저 많이 읽고, 나중에 가르친다**
Pre-training, Fine-tuning, Transfer Learning, Prompt, Context Window.

**Day 23 — 모델을 크게 만들면 무슨 일이 생길까?**
GPT-3, Zero/One/Few-shot, In-context Learning, Scaling Laws, Compute, Data, Parameter Count.

**Day 24 — 말 잘하는 모델을 '도움 되는 Assistant'로 만들기**
Instruction Tuning, SFT, Preference Data, Reward Model, RLHF, PPO, Alignment. InstructGPT 논문을 중심으로 봅니다.

**Day 25 — 거대한 모델을 다 고치지 않는 법**
LoRA, QLoRA, PEFT, Low Rank, Quantization, DPO, Preference Optimization.

### Part 5 — AI는 기억하고 검색하고 행동할 수 있을까?

**Day 26 — 다 외우지 말고 찾아보자**
RAG, Chunk, Embedding, Similarity, Vector Database, Retriever, Top-k, Context Injection, Citation.

**Day 27 — AI에게 기억을 주면?**
Short/Long-term Memory, Episodic/Semantic Memory, Retrieval, Reflection, Planning, Generative Agents/Reflexion.

**Day 28 — AI가 검색하고 계산기를 쓰기 시작했다**
Tool Use, Function Calling, API, Observation, ReAct, Toolformer, MCP의 개념적 위치.

### Part 6 — AI는 스스로 일할 수 있을까?

**Day 29 — Agent라는 시스템**
Goal, Planning, Tool Use, Memory, Feedback Loop, Evaluation, Failure Recovery, Multi-Agent. LLM과 Agent를 구분합니다.

**Day 30 — 최종 보스: 최신 논문 읽기**
그 시점의 공개된 최신 LLM/Agent 논문 중 하나를 골라 Title → Abstract → Introduction → Figure → Method → Experiment → Limitation 순서로 실제 독립 읽기에 도전합니다.

## 누적 결과물

30일 동안 다음이 누적됩니다.

- AI 역사 Timeline
- 핵심 개념 지도
- 논문 탐정 카드
- 대표 논문 요약
- 모델 계보도
- 개인 AI 논문 용어사전
- Day 30 최종 논문 리뷰

## 완료 후 수준

APEX는 연구실 석사 수준의 논문 재현 과정이 아닙니다. 목표는 **AI 논문 읽기 Level 3**입니다.

새 논문을 보면 전체가 낯선 문서로 보이는 대신, 기존에 아는 구조와 새로운 기여를 분리해 읽을 수 있고, 이해되지 않는 부분을 정확히 찾아 추가 학습할 수 있는 상태를 목표로 합니다.
