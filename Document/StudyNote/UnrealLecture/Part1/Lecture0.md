# 언리얼 프로그래밍을 효과적으로 공부하는 방법

## 서론

- 언리얼엔진을 공부해야 하는 이유
  - 대부분의 게임들이 언리언 엔진을 사용한다.
  - 5의 강력한 기능(루멘, 나나이트)

## 실력있는 언리얼 프로그래머를 찾기 어려운 이유

언리얼 프로그래밍에 대한 잘못된 접근 때문이다.

게임은 많은 그래픽과 데이터를 처리해야 하기에 저수준의 프로그래밍과 하이레벨의 기능을 같이 갖춘 언어가 필요하다. 따라서 `C++`의 기능에서 성능과 안정성을 높인 `언리얼 C++`를 사용한다.

*마치 C++,++같다.*

이런 부분을 공부하고 나아가야 하는데, 대부분의 프로그래머가 잘못된 방식으로 공부한다.

## 프로그래밍 언어만 알면 게임을 만들 수 있는가?

게임을 제작하기 위해서 언리얼이라는 툴을 사용하듯이 게임에서는 게임의 구조에 맞는 프레임웍을 사용해야 하는데, 언리얼 엔진은 자체적으로 제공한다. (유니티는 베이스가 없음)

기반을 다지고, 기둥을 세우고, 지붕을 덮는 과정 -> 이런 빌딩 구조를 언리얼 엔진에서 잘 만들어 둠

## 언리얼 프로그래밍은 어떻게 공부해야 하는가?

목적을 분명하게 해야함, 툴 자체가 매우 방대하기 때문에 겉만 돌다가 끝날 수 있다.

언리얼 엔진을 잘 다룬다는 영역은 크게 두가지로 나눌 수 있는데, 먼저 프로그래머에 의해 게임에 맞게 제작된 에디터를 사용하여 게임의 창작하는 영역과 프로그래머 영역에서 사용할 수 있는 클라이언트 에디터를 다루는 수준으로 나눌 수 있다.

대부분은 전자를 다루면 언리얼을 쓴다고 생각하지만, 동작 원리를 모르면 사실상 역량 향상의 목적은 이룰 수 없다.
*하지만 언리얼 엔진을 처음 써보거나 이해하는 측면에서는 매우 유용하다.*

잘 다루기 위해선 기초 체력인 `언리얼 C++`와 기본기인 `게임 프레임웍`에 대해서 깊게 공부해야 한다. (딥다이브가 필요한 영역)

### Part1: 언리얼 C++의 학습 방법

먼저 모던 겍치지향의 설계 기법을 학습하고, 언리얼 엔진의 자료구조, 메모리 관리, 에셋 및 빌드 시스템에 대해서 파악해야 함

- 언리얼 오브젝트
- 모던 객체지향설계
- 자료구조와 메모리
- 에셋과 빌드시스템

### Part2: 언리얼 게임 프레임웍의 학습 방법

기본기인 게임 프레임웍에 대한 학습 방법으로 게임을 구성하는 주요 요소를 파악해 전체 구조에 알맞게 커스터마이징 하되, 스케일업에 대응할 수 있도록, 효과적인 구조를 설계하는 것이 중요하다.

- 콘텐츠의 기본 구조
- 캐릭터 애니메이션
- 물리엔진과 이벤트
- 게임데이터와 인공지능
- 게임의 완성

**Part1과 Part2를 제한하지 말고 자신에게 필요한 영역을 우선적으로 학습하며 나아가는 것이 중요하다.**