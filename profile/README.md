# AiDeep

<img width="13501" height="5625" alt="main" src="https://github.com/user-attachments/assets/092e90b4-01d0-410c-8bfb-f8114d19318c" />

> 흩어진 기록을 구조화·연결·검색해 개인과 팀의 시간을 줄여주는 AI 기반 지식 허브

---
[![Wiki](https://img.shields.io/badge/📖_Wiki-온보딩-blue?style=for-the-badge)](https://github.com/Won-Life/.github/wiki)


## 📌 What is AiDeep?

AiDeep은 회의·업무·학습 등에서 쌓이는 **줄글 중심 기록의 비효율을 줄이고, 중요한 일에 쓸 시간을 되돌려주는 기록 활용 서비스**입니다.

“예전에 어디에 적어놨더라?”, “한번 정리했던 내용인데 또 만들고 있다” 같은 순간을 최소화하고, 개인과 팀이 의사결정에 집중하도록 돕습니다.

---

### 🎯 Problem

### 개인의 Pain

- 정보와 할 일은 계속 늘어나는데, **정리·복기·검색에 하루 40~50분 이상을 쓰고 있음**
- 회의/보고용으로 같은 내용을 여러 번 다시 정리해야 함

→ 실제 일·성장·학습에 쓸 시간이 연간 **두 달 이상** 사라집니다.

### 팀의 Pain

- 문서만으로 맥락을 이해하기 어려워 **회의가 길어지고 설명이 반복**됨
- 신규 합류자는 ‘옆자리 선배의 기억’에 의존해 온보딩 비용이 큼

→ 개인의 비효율이 팀 전체의 **생산성 저하 악순환**으로 이어집니다.

---

## 🧩 Root Cause

1. 폴더·텍스트 기반 문서 구조의 한계
    - 전체 흐름과 연결 관계를 **한눈에 파악하기 어렵습니다.**
2. 여러 일을 동시에 하는 개인에게 맡겨진 기록 관리
    - 다양한 맥락의 기록을 직접 분류·정리하느라 **인지 리소스가 낭비**됩니다.
3. 여기저기 흩어진 기록
    - 도구/폴더/채널마다 나뉜 기록은 **다시 쓰이지 못하고**, 기억 속에서 사라집니다.

---

## 💡 Solution

AiDeep은 사람이 해야 할 인지 노동을 최소화하고, **“기억·검색”이 아닌 “판단·결정”에 집중**할 수 있게 만드는 것을 목표로 합니다.

### 1) 그래프 기반 시각 구조화

- 회의록, 아이디어, 프로젝트 문서 등을 **그래프 형태로 시각화**합니다.
- 필요한 노드만 추려 시퀀스·연관 관계를 한눈에 볼 수 있습니다.
- 전체 구조를 빠르게 이해하고, 지금 해야 할 일을 쉽게 파악할 수 있습니다.

→ 내용 이해와 온보딩에 들어가는 **시간·비용 직접 절감**

### 2) AI 기반 연관 기록 자동 추천

- 현재 작업 맥락과 과거 기록의 **의미적 유사도**를 AI가 계산합니다.
- 과거 회의록·자료·아이디어 중 관련 있는 것들을 자동으로 찾아 추천합니다.
- 결과물/성과와 연결된 기록을 함께 보여줘 **“기록 → 실행”**으로 이어지게 합니다.

→ **기억 의존 노동에서 자유로워지고, 기록이 실제 성과와 자연스럽게 연결**

### 3) 외부 자료 연동 + AI 챗봇 통합 검색

- Notion, Google Docs, 파일 저장소 등 외부 자료를 연동합니다.
- “예전에 굿즈 주문 어디에 맡겼더라?” 같은 질문을 **한 번의 질의로 검색**합니다.
- 출처 기반 검색으로, 정확한 링크·문서까지 바로 도달할 수 있습니다.

→ 팀 전체의 **두 번째 브레인(Second Brain)** 역할을 하는 커뮤니케이션 & 레코드 허브

---

## 🧪 MVP & 검증

20대 초반 대학생/프리랜서를 대상으로 한 초기 검증 결과:

- 서비스 무료 이용 의향: **89.3%**
- 팀 도입 제안 의향: 30.4%
- 지인·동료 추천 의향: 26.8%

문제 해결·정확도 인식:

- 정보 검색·정리 시간 **60% 이상 감소될 것 같다**: 82.2%
- 원하는 정보를 잘 찾는 것 같다 (정확도 만족): **91%**

사용하고 싶은 활용 케이스:

- 강의 노트·취업 준비 자료 업로드 후 빠른 검색
- 복잡한 업무 전체 흐름·연결성 이해
- 과거 업무 내용 복기 및 재활용

---

## 🛠 Tech Stack

### Backend & AI

- Node.js, Nest.js, TypeScript
- Python, Flask
- RAG (Retrieval-Augmented Generation)
- AWS 등 클라우드 인프라 기반 아키텍처 설계

### Frontend
- **Next.js 15** – App Router 기반 풀스택 프레임워크, API rewrite로 백엔드 프록시 처리
- **React 19** – Concurrent rendering 지원 UI 라이브러리
- **React Compiler** – 자동 memoization으로 렌더링 최적화
- **TypeScript** – Node / Edge / API 전반의 타입 안전성 확보

### Graph & Visualization
- **@xyflow/react** – 인터랙티브 마인드맵 캔버스 (drag, edge connection, zoom/pan)
- **D3 (d3-force)** – AABB collision 기반 커스텀 force layout으로 노드 겹침 방지


---

## 👥 Team

> “문제를 가장 잘 이해하는 팀이, 문제를 가장 잘 푼다.”

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/seoki180">
        <img src="https://github.com/seoki180.png" width="100px;" style="border-radius:50%"/><br/>
        <sub><b>서석희</b></sub>
      </a><br/>
      <sub>Backend Lead</sub>
    </td>
    <td align="center">
      <a href="https://github.com/Jimin0430">
        <img src="https://github.com/Jimin0430.png" width="100px;" style="border-radius:50%"/><br/>
        <sub><b>최지민</b></sub>
      </a><br/>
      <sub>Frontend Lead</sub>
    </td>
    <td align="center">
      <a href="https://github.com/aeongiing">
        <img src="https://github.com/aeongiing.png" width="100px;" style="border-radius:50%"/><br/>
        <sub><b>정예원</b></sub>
      </a><br/>
      <sub>Frontend</sub>
    </td>
      <td align="center">
      <a href="https://github.com/codie0226">
        <img src="https://github.com/codie0226.png" width="100px;" style="border-radius:50%"/><br/>
        <sub><b>조희승</b></sub>
      </a><br/>
      <sub>Backend</sub>
    </td>
  </tr>
</table>

---

## 📬 Contact

**Project:** AiDeep  

- **Team Lead & Frontend – Jimin Choi (지민 최)**  
  Email: tangbole@naver.com  
  GitHub: https://github.com/Jimin0430  

- **Backend & AI – Seokhee Seo (서석희)**  
  Email: seoki180@inha.edu / seoki180@naver.com  
  GitHub: https://github.com/seoki180

> Don’t remember everything. **Focus on today.**
> 
> 
> 사람만이 할 수 있는 중요한 판단에 더 많은 시간을 쓸 수 있도록,
> 
> AiDeep이 기록과 정보를 대신 기억하고 연결합니다.
> 
