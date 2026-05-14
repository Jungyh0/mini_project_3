# mini_project_3
## 목차
  - [개요](#개요) 
  - [구현](#구현)
  - [DB](#DB)
  - [대시보드](#대시보드)
  - [Agent_Graphs](#Agent_Graphs)
## 개요
<img width="875" height="365" alt="image" src="https://github.com/user-attachments/assets/c06da4a2-e999-4034-b83a-205473a95e13" />

기존 리뷰 분석 방향은 긍/부정 여부만 사람이 직접 판단하는 방식이었고,
리뷰들의 형식이 정규화 되지 않고 각각 다르기 때문에 분석에 어려움이 있었다.
이러한 방식은 시간과 관리 비용이 증가하는 비효율적인 방법이라 판단 
AI_Agent를 활용해 분석과 결과를 볼 수 있는 데시보드를 제공함으로써 문제 해결 방향을 잡았다.

## 구현
<img width="946" height="373" alt="image" src="https://github.com/user-attachments/assets/bd6f6e69-6694-4299-a0db-151249f2a9db" />

[구성 요소]
- supervisor 패턴의 리뷰 분석 Agent
- Router 패턴의 개선 방향 도출 Agent
- 상품의 속성 관리 DB

