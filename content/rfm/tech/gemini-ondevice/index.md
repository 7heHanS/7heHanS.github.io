---
title: "Gemini On-Device, RFM의 경량화는 어디까지 왔는가?"
date: 2025-07-02
tags: ["RFM", "Gemini", "On-device", "EdgeAI", "DeepMind"]
categories: ["rfm", "tech"]
---

> 로봇에게 두뇌를 심는다는 것은 이제 AI 서버를 연결하는 일이 아니라,  
> 그 자체로 ‘두뇌’를 **로컬에 직접 넣는 일**이 되고 있다.

---

## 로봇의 두뇌, 어디까지 작아질 수 있을까?

RFM(Robot Foundation Model)의 핵심은 다양한 센서 입력을 통합하고,  
상황에 맞는 행동을 생성해내는 범용 추론 능력이다.  
하지만 지금까지의 대부분 RFM은 클라우드 연산에 의존하고 있었다.

- 연산 성능과 메모리 요구가 높고  
- 지연 시간, 연결 문제도 존재했다

---

## DeepMind의 해답: **Gemini Robotics On-Device**

2025년 6월, Google DeepMind는  
[RoboCat, RT-X 등의 연장선]에서 새로운 시도를 공개했다:

**Gemini On-Device**  
→ RFM을 휴머노이드와 같은 실제 로봇에 **직접 탑재**할 수 있도록 경량화한 모델이다.

📌 자세한 내용:  
🔗 [공식 블로그 – Gemini Robotics On-Device](https://deepmind.google/discover/blog/gemini-robotics-on-device-brings-ai-to-local-robotic-devices/)

---

## 왜 이게 중요한가?

| 기존 문제점             | Gemini On-Device의 해결책                           |
|----------------------|--------------------------------------------------|
| 클라우드 연산 의존        | 로컬 SoC, ARM 계열에서 직접 실행 가능                |
| 지연 시간 문제           | on-device 추론으로 실시간 반응 달성                 |
| 높은 전력 소비           | 효율적인 모델 구조로 전력 최적화                   |
| 연결 불안정             | 네트워크 없이도 완전 동작 가능                     |

로컬에서 작동하는 RFM은 이미 스마트폰의 NPU처럼 **로봇의 핵심 컴퓨팅 모듈**이 될 수 있다.

![Apptronik Apollo에 탑재된 Gemini On-Device](google-deepmind-on-device.webp)

이 이미지는 Google이 직접 시연한 Apptronik의 휴머노이드에 **Gemini On-Device를 안정적으로 탑재**한 예시입니다.
일반 네트워크 없이도 행동 예측과 제어가 가능한 점이 핵심이죠.

---

## 스마트폰 → 로봇: 플랫폼의 진화

Gemini On-Device는 로봇을 하나의 **스마트 컴퓨팅 기기**로 진화시키는 기반이 될 수 있다.

- SoC 위에서 RFM 실행  
- OTA 업데이트로 기능 확장  
- 모듈 교체형 하드웨어 + 소프트웨어 스택  
- App Store → Action Store?

---

## 내가 주목한 키워드

- **경량화(Lite RFM)**: 기존 Transformer 모델의 최적화  
- **엣지 추론(Edge Inference)**: ROS2 + GPU 없이도 동작  
- **하드웨어 독립성**: ARM 기반 다양한 폼팩터에 이식 가능  
- **SDK 출시**: MuJoCo 시뮬레이터 기반 개발자 접근성 강화

---

## 마치며

RFM의 미래는 더 강해지는 게 아니라, **더 가까워지고 더 실용적으로** 진화하는 방향입니다.  
로컬에 탑재된 ‘두뇌’가 진짜 혁명의 시작이라는 걸 **Gemini On-Device가 증명**하고 있습니다.

> “나는 먼저 엿보고 왔다. 그래서 기록하고, 이해하고, 나아간다.”

