---
layout: post
title:  "Mike Cohn의 Better User Stories 강의"
date:   2017-03-27 09:49:00
category: agileresearch
---

<img src="/images/agileresearch/agileresearch_mikecohn_userstories.png"/>


## Lesson #1 : 스토리 작성 워크샾에서 스토리 매핑을 성공적으로 이끄는 3가지 팁

### 사용자 스토리 작성시에 가장 질문이 많고 어려운 부분 (TOP 3)
1. Getting teams engaged
2. Adding too much or too little detail
3. Splitting stories


> 스토리들이 요구사항 명세서를 단순히 대체하는 것이 아니다!!!

### 스토리 작성 워크샾을 성공적으로 이끄는 팁
* Tip #1 하나의 목적(주제)에 집중하라.
    * 프로덕트 오너는 큰 목표(big goal)를 제시하고 키 스테이크홀더(key stakeholder)들은 그 목표를 해결하기 위해서 필요한 것들을 제시합니다.
    * 제시된 내용들을 가지고 프로덕트 오너는 사용자, 관련 회사들을 돌아다니며 중요한 것이 무엇인지 그들의 생각을 듣습니다. 
    * 그리고 다음 3개월 동안 무엇에 초점을 맞춰서 작업을 해야 할 것인지를 결정합니다.
* Tip #2 올바른 참가자
    * 모든 팀멤버들이 플래닝 시간에 참가하여 자신들이 사용자 스토리에 대해 궁금한 모든 것들을 이해한다.
    * 반드시 모든 멤버가 참여해야 하는 것은 아니다. 스토리에 따라 참여가 반드시 필요한 멤버들만 참여하는 것이 좋은 경우도 있다. 모든 멤버가 모든 스토리에 대해 참여하는 것은 시간낭비 일 수도 있다.
    * 시간이 많이 소요되고 불필요한 것으로 보일 수 있지만, 무척 중요한 시간이다.
    * 예외적으로 여러개의 팀이 하나의 골을 위해서 진행될 때는 각 팀에서 가장 영향력있는 사람들만이 참여하여 진행해도 무관하다.
    * 사용자와 스테이크홀더들도 반드시 초대해야 한다.
* Tip #3 스토리의 관계를 시각화하라
    * 스토리 맵을 작성한다. 2차원으로 구성되며 x축은 시퀀스를, y축은 대체작업을 작성한다.
        * 스토리 맵을 작성함으로써 얻는 이익
            * 스토리맵은 스토리를 찾거나 살펴볼 때 한눈에 볼 수 있고, 빠진 것이 무엇인지 찾기 편하다.
            * 시퀀스의 각 스텝을 기준으로 질문을 던지기 쉽다.
                * 사용가가 다음에 가장 원하는 것이 무엇인가?
                * 사용자가 이단계에서 실수를 할 수 있는 상황이 무엇인가?
                * 사용자가 당황할만한 포인트가 무엇인가?
                * 사용자가 필요로하는 추가적인 정보가 무엇인가?
            * x축에 있는 모든 항목들은 반드시 다음 릴리즈에 포함되어야 한다는 것을 알 수 있다.
    * 대체작업은 높은 우선순위를 갖는 작업을 위쪽에 위치하고 낮은 우선순위가 밑에 위치한다.


## Lesson #2 : Using SPIDR to Split Any Story

사용자 스토리를 작게 나눈다는 것은 팀이 작은 스토리들을 해결할 때 느끼는 성취감으로 좋은 기분을 느끼게 해줄 수 있고, 다음 작업을 해야 한다는 동기를 부여해줄 수 있다.

많은 사람들이 사용자 스토리를 의미있게 나누는 것에 대해 많은 질문들을 한다. 
왜냐하면, 한 이터레이션에 명확하게 딜리버리 할 수 있을 정도의 크기로 스토리를 나눠야 되고 그렇지 않으면 많은 문제가 발생하기 때문이다.
하지만, 그렇게 나누는 것이 쉽지 않다.
* How to split stories in a way that shows progress, but can also be delivered in one iteration.
* How to avoid the temptation of splitting stories between functional areas such as programming and testing
* How to spend the right amount of time splitting stories, so you’re not doing it at the cost of getting something built.
* How to not get lost in the 50+ different ways to split a story that you can find on the internet.

### 이를 해결하기 위해 SPIDR이라는 방법론을 제안한다.

* Spike : A research activity intended to build knowledge
  * 스토리에 대해 어떤 것인지 파악하고, 어떤 기술이 좋을지에 대해서 연구하는 시간을 갖음으로써 스토리를 어떻게 나눠야할지에 대해 좋은 결론을 맺을 수 있음
  * 다른 4가지 기법을 다 해보고 나서 그래도 안될 경우에 마지막에 사용할 것

* Paths : Consider the paths through a story and split each path into its own story
  * 스토리를 분리해서 Path를 생성할 수 있는지 고민한다. 
  * 같은 유형은 하나로 묶을 수 있다. 예제에서는 페이라는 스토리가 Creditcard or Paypal로 구분되었고 Creditcard가 3개로 나눌 수 있지만, 하나의 스토리로(pay with a credit card) 구성했다.

* Interfaces : Split a story across multiple user interfaces (mobile OS, browser) or data interfaces.

* Data : Develop an initial story that supports only a subset of the data

*Rules : Relax business rules or technology standards in an initial version of a story
  * 예를 들어 티켓 8장을 판매해야 하는데, 4장은 먼저 팔고 나머지 4장은 나중에 판다고 했을 때 사용자 스토리
  * 나스닥의 그래프를 그려주는데 첫번째에는 없었던 성능 이슈가 나타났을 때(technology)
  * 이런 식으로 비지니스 룰에 의한 기술적인 부분에 의해 초기 버전의 스토리가 나오고 추후 이를 개선하기 위한 스토리를 구분할 수 있다.

스토리를 나눌 때 5가지 룰들 중 하나가 적용되었다고 끝나는 것이 아니라 적용될 수 있는 모든 룰들을 적용하여 나누는 것이 좋다.



## Lesson #3 : Solving the Problems of Too Much or Too Little Detail

목표 : 팀에 알맞은 양의 정보를 알맞은 시간에 주는 사용자 스토리를 작성 

### 사용자 스토리 작성 시 다음과 같은 두 가지 케이스로 인해 문제가 발생될 수 있음
* PO로 부터 특정 정보를 받아야 하는데 PO들을 스테이크 홀더들과 회의를 하면서 시간이 delay되어 팀에게 정보를 못넘겨주는 경우
    * 정보를 받지 못해서 작업을 진행하지 못함
* PO들이 정보를 주었지만, 정보 자체가 원래 예상했던 것보다 크기가 커서 스토리의 크기가 커진 경우
    * 너무 상세한(제약조건, ) 경우에는 구현해야 하는 작업의 양이 너무 많아서 한주가 아닌 2~4 iterations에 해결할 수 있게 됨

너무 상세하거나 너무 정보가 없는 것은 문제가 있다. 중간인 sweet spot을 찾는 것이 중요하다.

이를 위해서는 회고시간을 통해 각팀에 맞는 sweet spot이 어디인지를 찾아내야 한다.
질문은 “지난 스트린트에서 주어진 정보는 적당했는가? 그리고 알맞은 시간에 정보가 제공되었는가?”
묻는 질문에 대한 답변은 "Too much detail.”, "Too late.”, "Just right!"

회고를 진행할 때마다 같은 질문을 통해 어떻게 하는 것이 가장 좋은 방법(sweet spot)인지에 대해 결정한다.


## Reference
- [Mike Cohn 강좌 사이트](http://www.betteruserstories.com)
