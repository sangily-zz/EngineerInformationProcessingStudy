# 0. 정보처리기사 필기 공부계획 및 내용정리

## 1) 목차

[TOC]



## 2) 공부법

- 매 섹션 끝의 기출문제 따라잡기 먼저 보고, 문제 출제 유형 및 내용 확인
- 섹션 처음으로 돌아와 전문가의 조언을 읽은 후 본문 읽기
- 다시 기출문제 따라잡기 확인 후 이해되지 않는건 미결 표시 후 다음 섹션으로 넘어가기
- 한 장을 마친 후 나오는 예상문제은행도 마찬가지로 틀렸거나 이해 안되는건 미결체크 후 패스
- 1회독 후 처음으로 돌아와 기출문제 따라잡기와 에상문제은행만 다시 공부
- 시험 임박시 등급이 A,B인 섹션과 표시해둔 문제들만 다시 확인

1권(557p) + 2권(326p) - 책머리(21p + 7p) = 855p

855p / 10 = **85p / day**

| 날짜                     | 내용                                      |
| ------------------------ | ----------------------------------------- |
| Day1 (7/31 토 ~ 8/1 일)  | 1권 시작. ~85p                            |
| Day2 (8/2 월)            | ~170p                                     |
| Day3 (8/3 화)            | ~256p                                     |
| Day4 (8/4 수)            | ~340p                                     |
| Day5 (8/5 목)            | ~424p                                     |
| Day6 (8/6 금)            | ~511p                                     |
| Day7 (8/7 토)            | 1권 끝. ~557p. 2권 시작. ~51p             |
| Day8 (8/8 일)            | ~146p                                     |
| Day9 (8/9 월)            | ~233p                                     |
| Day10 (8/10 화)          | 2권 끝. ~326p                             |
| Day11 (8/11 수)          | 1권 문제 다시 다 풀어보기                 |
| Day12 (8/12 목)          | 2권 문제 다시 다 풀어보기 + 기출 풀어보기 |
| Day13 (8/13 금)          | 기출 풀이                                 |
| **필기시험날 (8/14 토)** | **송파구 가락동 가원중학교 09:00**        |





# 1. 소프트웨어 설계

## 1) 요구사항 확인

### [1] 소프트웨어 생명 주기(Software Life Cycle)

- 소프트웨어 개발 방법론의 바탕

- **요구사항 분석 및 설계, 개발, 품질 관리**의 과정을 **단계별**로 나눈 것

- 개발자는 **문제의 유형**이나 **개발 방법** 등에 따라 **특정 모형을 선택**하여 사용할 수도 있고, **개별적인 모형**을 사용할 수도 있다.

- 소프트웨어 **생명 주기 모형** = 소프트웨어 **수명 주기 모형** = 소프트웨어 **프로세스 모형** = 소프트웨어 **공학 패러다임**

- 일반적으로 사용되는 모형은 다음과 같다.

  > - [ ] **폭포수 모형**
  >
  > > - **물이 거슬러 올라갈 수 없듯,** 이전 단계로 돌아갈 수 없다는 전제하에 **각 단계를 확실히 매듭짓고 다음 단계로 진행**
  > > - 소프트웨어 공학에서 **가장 오래되고 폭넓게 사용된 전통적인 생명 주기 모형**으로, **고전적 생명 주기 모형**이라고도 한다.
  > > - **선형 순차적 모형**
  > > - **적용 및 성공 사례 多**
  > > - **메뉴얼** 작성 必
  > > - 각 단계가 끝난 후에는 다음 단계를 위한 **결과물이 명확하게 산출**되어야 한다.
  > > - 두 개 이상의 **과정 병행 X**
  >
  > <img src="C:\Users\tkddl\AppData\Roaming\Typora\typora-user-images\image-20210731171006960.png" alt="image-20210731171006960" style="zoom:50%; float:left" />

  

  

  > - [ ] **프로토타입 모형(Prototype Model, 원형 모형)** 
  >
  > >- 사용자 요구사항을 정확히 파악하기 위해 **견본(시제)품(Prototype)**을 만들어 최종 결과물을 예측하는 모형
  > >- **시제품은 UI 중점 개발**
  > >- 시스템의 모형을 만들어 추후 구현 단계에서 **골격 코드**로 사용
  > >- 소프트웨어 개발이 완료된 시점에서 오류가 발견되는 폭포수 모형의 단점을 보완
  >
  > <img src="C:\Users\tkddl\AppData\Roaming\Typora\typora-user-images\image-20210731170721041.png" alt="image-20210731170721041" style="zoom:20%; float:left;"/>

  

> - [ ] **나선형 모형(Spiral Model, 점진적 모형)**
>
> >- 폭포수 모형과 프로토타입 모형의 장점에 **위험 분석 기능**을 추가한 모형
> >- **점진적 모형**이라고도 한다. **(프로토타입을 지속적으로 발전)**
> >- **위험 관리 및 최소화가 목적**
> >- 점진적으로 개발 과정이 반복되므로 **요구사항을 중간에 첨가**할 수 있고, **정밀**하며, **유지보수 과정이 필요 없다.**
>
> <img src="C:\Users\tkddl\AppData\Roaming\Typora\typora-user-images\image-20210731172656735.png" alt="image-20210731172656735" style="zoom:20%; float:left;" />



> - [ ] **애자일 모형(Agile Model)**
>
> > Agile : 민첩한, 기민한
> >
> > - **고객의 요구사항 변화에 유연하게 대응**할 수 있도록 **일정 주기를 반복**하며 개발과정 진행
> > - **고객 소통**에 초점, 고객 요구사항에 **우선순위** 부여, 적극 수용 **(폭포수 모형과 대조적)**
> > - 기업 활동 전반에 걸쳐 사용
> > - 짧은 개발 주기(**스프린트**(Sprint), 또는 **이터레이션**(Iteration)) 반복
> > - 소규모 프로젝트, 숙련된 개발자, 급변하는 요구사항에 적합
> > - **애자일 기반 개발 모형**에는 **스크럼**, **익스트림 프로그래밍(XP)**, **칸반(Kanban)**, **Lean**, **크리스탈**, **ASD**, **기능 중심 개발(FDD)**, **DSDM**, **DAD** 등이 있다.
> > - **애자일 개발 4가지 핵심 가치**
> >   1. 프로세스와 도구보다는 **개인과 상호작용**에 더 가치를 둔다
> >   2. 방대한 문서보다는 **실행되는 SW**에 더 가치를 둔다
> >   3. 계약 협상보다는 **고객과 협업**에 더 가치를 둔다
> >   4. 계획을 따르기 보다는 **변화에 반응하는 것**에 더 가치를 둔다
>
> <img src="C:\Users\tkddl\AppData\Roaming\Typora\typora-user-images\image-20210731191045113.png" alt="image-20210731191045113" style="zoom:90%; float:left;" />



### [2] 소프트웨어 공학

- 소프트웨어의 **개발, 운용, 유지보수, 폐기 처분**에 대한 체계적인 접근 방안

- **기본 원칙**

  > - **현대적인 프로그래밍 기술** 지속적 적용
  > - **품질 유지** 지속적 검증
  > - 관련 사항 및 결과에 대한 **기록 유지**



## 2) 스크럼(Scrum) 기법

### [1] 개념

- 럭비 경기에서 팀이 이루는 대형을 뜻한다. 즉, **팀을 중시하여 개발의 효율성을 높인다**는 의미이다.
- **팀원 스스로가 팀을 구성**해야 하며, **개발 작업에 관한 모든 것을 스스로 해결**할 수 있어야 한다.

### [2] 스크럼 팀의 구성원

> **제품 책임자(PO; Product Owner)**
>
> > - **이해관계자**[^1] 들 중 **개발될 제품에 대한 이해도**가 높고, **요구사항을 책임지고 의사 결정**할 사람으로 선정하는데, 주로 개발 의뢰자나 사용자가 담당한다.
> > - 이해관계자의 의견을 종합하여 **제품에 대한 요구사항(백로그(Backlog)[^2])을 작성하는 주체**이다.
> > - **팀원**은 백로그에 **스토리**[^3] 를 추가할 수는 있지만 **우선순위를 지정할 수는 없다.**
> > - **PO**는 제품 테스트를 수행하며 **주기적으로 우선순위를 갱신**한다.
>
> **스크럼 마스터(SM; Scrum Master)**
>
> > - 스크럼의 원활한 수행을 위해 **객관적인 시각에서 조언**하는 가이드 역할. 팀원들을 통제하는 것이 목표가 아니다.
> > - **일일 스크럼 회의를 주관**하여 진행 사항을 점검하고, 개발 과정에서의 장애 요소를 공론화하여 처리한다.
>
> **개발팀(DT; Development Team)**
>
> > - **PO와 SM을 제외한 모든 팀원**으로, 개발자 외에도 디자이너, 테스터 등 제품 개발을 위해 참여하는 모두가 해당된다.
> > - 보통 최대 인원은 **7~8명**이 적당하다.

### [3] 스크럼 개발 프로세스











______________________________________

# 주석

[^1]: 개발 의뢰자, 개발자, 사용자 등.
[^2]: 제품 개발에 필요한 요구사항을 모두 모아 우선순위를 부여해 놓은 목록
[^3]: 백로그에 담겨질 요구사항. 단어 형태가 아닌, '고객은 상품 주문을 위해 로그인을 수행해야 한다'와 같이 서술하는 형태로 표현하기 때문에 스토리, 또는 사용자 스토리라고 칭함.
