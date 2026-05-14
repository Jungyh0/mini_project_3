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

## DB

<img width="673" height="571" alt="스크린샷 2026-05-14 165146" src="https://github.com/user-attachments/assets/87d66791-d4cf-4f13-80c9-f3801e8f72a8" />


[column]
- review: 사용자 리뷰 원문
- aspect: 리뷰에서 추출한 속성
- label: aspect와 1대1로 매칭된 만족도 (1: 만족, 0: 불만족)
- score: 별점 점수(보완점을 찾을 비류 검출용)


<img width="549" height="299" alt="image" src="https://github.com/user-attachments/assets/c7fe394f-de52-42e1-8fee-fe58e4c11287" />

<img width="557" height="262" alt="image" src="https://github.com/user-attachments/assets/97ae2bba-4970-4e6b-bbaa-483531c0af39" />

<img width="553" height="225" alt="image" src="https://github.com/user-attachments/assets/7c1fdb7f-ff39-482e-8511-4b73bdb9f4a0" />


## 대시보드
### [상품 이류 등록/ 분석 대시보드]

<img width="549" height="299" alt="image" src="https://github.com/user-attachments/assets/cc78ddbb-0e2e-4607-81a5-04921fc60e28" />

### [aspect의 만족 분포도]

<img width="549" height="299" alt="image" src="https://github.com/user-attachments/assets/0415f9c4-8a77-428e-89fe-44c23e7c213c" />

### [개선 방향 도출 대시보드]

<img width="1342" height="1035" alt="image" src="https://github.com/user-attachments/assets/530249b5-e04e-4e8e-bd1e-76606dbaf1c3" />


<img width="1356" height="378" alt="image" src="https://github.com/user-attachments/assets/cab80cde-752c-4e39-a373-df1d7e02afc5" />


<img width="1009" height="1034" alt="image" src="https://github.com/user-attachments/assets/866e347b-4b64-4c0f-b16c-d87e4419d106" />



## Agent_Graphs
### Supervisor 패턴 Agent graph

<img width="267" height="204" alt="image" src="https://github.com/user-attachments/assets/f756f6eb-8d25-4c9c-8f09-937d316c3dab" />


### Router 패턴 Agent graph

<img width="267" height="204" alt="image" src="https://github.com/user-attachments/assets/8fe8faef-3b46-41a2-937e-3cca5b5a0e28" />
