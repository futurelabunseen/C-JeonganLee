# 프로젝트 세부 기획서

1차 기획서에서 [게임 디자인 워크숍](https://github.com/fkdl0048/CodeReview/blob/main/GameDesign/GameDesignWorkshop.md) 내용을 토대로 업데이트 된 2차 기획서입니다.

## 목차

- 게임 개요
  - 레퍼런스
  - 게임 요약
  - 게임 미캐닉
- 프로젝트 목표
- 게임 설명
- 게임 설계
- 개발 일정

### 게임 개요

게임 이름: Ugh
장르: 3인칭 슈팅 액션
플랫폼: PC
개발 기간: 3개월
개발 인원: 1명

#### 레퍼런스

- [Risik of Rain2](https://store.steampowered.com/app/632360/Risk_of_Rain_2/) 장르, 디자인, 시스템
- [Gatekeeper](https://store.steampowered.com/app/2106670/Gatekeeper/) 스킬, 시스템

#### 게임 요약

3인칭 슈팅 액션게임으로 간단한 스킬과 무기를 이용해서 몰려오는 적을 처치하는 게임입니다. 슈팅 액션과 로그라이크를 결합하여 전략적 플레이를 할 수 있도록 설계할 예정입니다.

#### 게임 미캐닉

- 코어 미캐닉: 총을 쏴 몬스터를 처치하는 것
- 2차 미캐닉: 스킬과 유물의 특성을 활용하는 것
- 게임플레이 진행: 스테이지 전개(로그라이크)
- 게임의 서사: 스토리x 기능에 중점을 두기에 에셋에 맞춰서 진행할 예정입니다.

### 프로젝트 목표

약 3개월간 개발 예정이기에 프로젝트에 대한 목푤를 설정합니다.

- 완성 가능한가?
- 재미가 있는가?

개발 방향또한 빠르게 프로토 타입을 개발하고 기능을 추가하거나 보완하는 방향으로 개발할 예정입니다.

### 게임 설명

게임에 관한 상세 설명입니다.

#### 게임 플레이

게임 플로우는 다음과 같습니다.

- 로비
- 인게임
- 엔딩

##### 로비

![image](https://github.com/futurelabunseen/B-JeonganLee/assets/84510455/1a1c90e6-a5cb-493f-aed7-a73667753f55)

로비에선 자신이 플레이할 캐릭터를 선택하고, 게임을 시작할 수 있는 로비입니다. 마우스로 해당 캐릭터를 클릭하여 시작할 수 있습니다.

*프로토 타입으로 빠르게 1개의 캐릭터를 개발 후 확장 예정입니다.*

##### 인게임

![image](https://github.com/futurelabunseen/B-JeonganLee/assets/84510455/73de6b7a-9d67-42ac-8876-4f077feb9f4a)

기본으로 지급되는 스킬과 총을 사용하여 몰려오는 몬스터를 사냥합니다. 몬스터를 처치하여 골드를 수급할 수 있고 골드는 웨이브가 종료된 후 상점에서 가챠를 통해 아이템을 얻을 수 있습니다.

##### 엔딩

클리어시 간단한 엔딩 연출을 통해 게임을 종료합니다.

*실패하면 다시 로비로 돌아갑니다.*

#### 시스템 설명

해당 게임의 시스템에 대한 상세 설명입니다.

핵심적인 재미 요소는 다회차 플레이를 계속해서 유도하고 이를 위해 슈팅 액션이지만 전략적 플레이를 요구합니다.

전략적 플레이는 현재 상태를 업그레이드 하여 더 높은 스테이지에 도달하거나 약한 상태를 유지하여 골드의 수급을 늘려 높은 등급의 유물을 노리는 등 다양한 전략적 선택이 있습니다.

##### 플레이어 입력

- 로비
  - 마우스를 통해 조작합니다.
- 인게임
  - 3인칭 시점으로 마우스를 통해 방향을 결정하고, W, A, S, D로 이동합니다.
  - 마우스 왼쪽, 오른쪽으로 기본 공격과 특수 공격을 사용합니다.
  - Q, W, E로 각 캐릭터 특성에 맞는 스킬, 회피, 궁극기를 사용합니다.
  - 스페이스바로 점프합니다.
  - Shift로 달리기를 사용합니다.
- 상점
  - 마우스로 통해 조작합니다.

##### 몬스터

몬스터는 웨이브별로 점점 강해지며, 플레이어를 추격합니다.

몬스터는 지상, 공중, 보스몬스터로 구분되며, 5웨이브마다 보스몬스터가 등장합니다.

##### 골드

몬스터를 잡아서 골드를 수급합니다. 골드는 100원 단위마다 10%이자가 붙어서 증가합니다. (최대 500원)

골드를 사용하여 상점에서 가챠를 통해 아이템을 얻을 수 있습니다.

##### 상점

웨이브가 종료된 후 활성화 됩니다. 상점에선 총 3가지의 가챠를 통해 강해질 수 있습니다.

- 무기 업그레이드
  - 50골드를 통해 현재 무기의 공격력을 강화할 수 있습니다. (성공과 실패)
- 무기의 옵션 추가
  - 무기의 단계별 강화
  - 무기의 옵션을 추가로 붙입니다. 약 20%의 확률로 발동되며 특수한 옵션을 붙여 쉽게 강해질 수 있습니다.
  - ex) 탄창의 수 증가, 두발 씩 발사, 장전 속도 증가, 점프력 증가 등등..
- 유물 가챠
  - 등급에 맞는 유물을 구매할 수 있으며 플레이어의 능력치를 향상시기커나 특수한 능력을 부여합니다.
    - ex) 체력 증가, 공격력 증가, 스킬 쿨타임 감소, 특수 능력 추가 등등..
    - ex) 속성 옵션, 몬스터 처치 시 효과, 플레이어의 특성 변경, 특수 스킬 효과 등등, 게임 모드에 영향 주는 효과 등등

##### 게임 목표

게임은 최종 웨이브까지 도달하여 클리어하는 것이 목표입니다.

##### 게임 오버

플레이어가 죽으면 게임 오버가 되며, 현재 유물만을 가지고 1회차로 돌아갑니다.

### 게임 설계

#### 게임 플로우 도메인 모델

![alt text](image.png)

#### 플레이어

기본 플레이어로 개발할 캐릭터는 다음과 같습니다.

- 거너
  - 기본 공격: 단일 탄환 발사 (맥크리)
  - 특수 공격: 삿갓 발사
  - 스킬 (Q): 지뢰설치
  - 스킬 (W): 구르기 회피
  - 스킬 (E): 연속 발사

플레이어는 GAS시스템을 활용

### 개발 일정

- 프로젝트 1주차 (3/18 ~ 3/25)
  - 기본 플레이어 움직임 및 총쏘기 구현
- 프로젝트 2주차 (3/25 ~ 4/1)
  - 몬스터 생성 및 웨이브 시스템 구현
- 프로젝트 3주차 (4/1 ~ 4/8)
  - 상점 시스템 구현
- 프로젝트 4주차 (4/8 ~ 4/15)
  - 게임 플로우에 맞게 설계
- 프로젝트 5주차 (4/15 ~ 4/22)
  - 유물 및 프로토 타입 완료