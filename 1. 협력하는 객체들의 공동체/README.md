# 협력하는 객체들의 공동체

“시너지를 생각하라. 전체는 부분의 합보다 크다.” - 스티븐 코비(Stephen R. Covey)

## 서론

객체지향 프로그래밍: 현실 속에 존재하는 사물을 최대한 유사하게 모방해 소프트웨어 내부로 옮겨오는 작업
- 객체지향 소프트웨어: ~~실세계의 투영~~
- 객체: 사물에 대한 추상화

<br/>
소프트웨어 객체와 실세계 사물 사이 연관성 희미

→ 객체지향의 목표: **새로운 세계의 창조**

<br/>
‘캡슐화’하는 ‘자율성’ - 스스로 생각하고 스스로 결정

‘메시지’ → ‘협력’ - 암묵적인 약속과 명시적인 계약을 기반으로 협력하여 목표 달성해 나가는 과정

‘연결완전성’ - 실세계의 사물을 기반으로 소프트웨어 객체를 식별하고 구현까지

<br/>

# 협력하는 사람들

## 커피 공화국의 아침

손님의 커피 주문 → 주문 받는 캐시어 → 바리스타의 커피 제조 → 캐시어에게 제조 완료된 커피 전달 → 손님에 제공

<br/>
손님, 캐시어, 바리스타의 조율과 조화 = 역할, 책임, 협력의 조화

### 역할 role

1. 손님
2. 캐시어
3. 바리스타

### 책임 responsibility

1. 손님 - 커피 주문
2. 캐시어 - 손님이 하는 주문 받기
3. 바리스타 - 주문된 커피 제조

### 협력 collaboration

커피가 정확하게 주문되고 주문된 커피가 손님에게 정확하게 전달될 수 있도록 맡은 바 역할과 책임을 다하고 있는 것

<br/>

## 요청과 응답으로 구성된 협력

### 요청 request

1. 손님이 캐시어에게 커피 주문 = 커피를 제공해 줄 것을 요청
2. 캐시어가 바리스타에게 주문 내역 기록된 컵 전달 = 주문된 커피를 제조해 줄 것을 요청

### 응답 response

요청과 반대 방향으로 연쇄적으로 전달

1. 바리스타이 캐시어에게 커피 제조 완료 전달 = 캐시어의 요청에 응답
2. 캐시어가 손님에게 커피 제공 = 손님의 요청에 응답

<br/>

## 역할과 책임

### 역할

협력에 참여하는 특정한 사람이 협력 안에서 차지하는 책임이나 임무

- 손님, 캐시어, 바리스타
- ‘책임’ 내포

### 책임

특정한 역할 = 특정한 책임

- 손님 - 커피 주문
- 캐시어 - 주문, 커피 전달
- 바리스타 - 커피 제조

<br/>

## 역할과 책임 수행

1. 여러 사람이 동일한 역할을 수행할 수 있다.

   → 매일 캐시어가 달라도, 주문을 받고 커피가 완성됐음을 통보하는 책임을 이행하면 된다.

    - 손님 - 주문한 커피를 마실 수만 있으면, 어떤 캐시어가 주문을 받는지 중요하지 않음
    - 캐시어 - 자신이 전달한 주문 내역에 맞게 커피를 제조할 수만 있으면, 어떤 바리스타가 커피를 제조해도 상관 없음<br/><br/>
2. 역할은 대체 가능성을 의미한다.

   → 손님 입장에서 캐시어는 **대체 가능**(substitutable)

    - 두 명이 동일한 역할을 수행할 수 있으면, 요청자 입장에서 어떤 사람이어도 문제되지 않음<br/><br/>
3. 책임을 수행하는 방법은 자율적으로 선택할 수 있다.

   → 응답하는 사람은 요청을 처리하는 방법을 자유롭게 선택할 수 있다.

    - 바리스타는 자신만의 독특한 방법으로 커피를 제조할 수 있음
    - 동일한 요청을 받아도, 바리스타의 역할을 수행하는 사람들마다 다른 방식으로 처리할 수 있음
    - **다형성**(polymorphism): 동일한 요청에 다른 방식으로 응답할 수 있는 능력<br/><br/>
4. 한 사람이 동시에 여러 역할을 수행할 수 있다.

   → 한 사람이 캐시어와 바리스타의 역할을 동시에 수행할 수 있다.
