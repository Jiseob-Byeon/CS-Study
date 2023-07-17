# 운영체제 Intro(운영체제란?)

## 운영체제란?
- 컴퓨터의 하드웨어를 관리하는 소프트웨어_공룡책, 3p
- 정부(Government) 같은 것 - 그 자체로는 유용한 기능이 없으나, 다른 프로그램들이 효과적으로 동작하기 위한 환경을 제공_같은 책, 4p

## 가장 중요한 질문: 운영체제를 왜 배우는가?
- _공룡책 Ans.

<a href="https://ibb.co/9sWjVrs"><img src="https://i.ibb.co/wM41wzM/Screenshot-2023-07-17-at-10-19-42-PM.png" alt="Screenshot-2023-07-17-at-10-19-42-PM" border="0"></a>

- 대부분의 프로그래머가 실제로 운영체제를 설계하거나 구현할 일은 없겠지만, 운영체제를 잘 알아야 경제적이고 안전하게 프로그램을 설계할 수 있기 때문

## 운영체제의 필요성 - **하드웨어와 App을 이어주는 glue logic의 역할**
- 컴퓨터 시스템을 크게 네 부분으로 나누면 1. 하드웨어 2. 운영체제, 3. App 4.사용자로 나눌 수 있는데,
  운영체제는 하드웨어와 App을 이어줌
- 컴퓨터 시스템은 크게 사용자 관점과, 시스템 관점으로 바라볼 수 있음
- 사용자 관점에서는 쓰기 편한 것이 가장 중요하며, 자원의 활용을 덜 고려함
- 반대로 시스템 관점에서는 운영체제는 하드웨어와 직접 관련. 이 맥락에서는 운영체제를 자원 관리자로 볼 수 있음(자원을 효율적이고 공평하게 할당)
- 운영체제는 사용자가 더 편하게 사용할 수 있는 환경을 제공하며, 자원을 효율적으로 배분하게 도와줌

## 운영체제의 역할 1) 자원 관리자로서의 운영체제
- 운영체제는 여러 역할을 맡고 있는데, 그 중 하나가 자원 관리
- 프로세스: 실행중인 프로그램으로, 메모리 상에 올라감
- 자원: 프로세스가 작동하기 위해 필요한 모든 것으로, CPU 사용 시간, 메모리 공간 등이 있음

- 자원 관리자로서 운영체제는 1. 자원을 추상화하고 2. 자원을 관리(공유)


### 1. 자원의 추상화
<a href="https://ibb.co/qRPqchh"><img src="https://i.ibb.co/sFMxNcc/IMG-1441.jpg" alt="IMG-1441" border="0"></a>

- 추상화: 더 중요한 내용을 강조하기 위해 다른 정보를 제거하거나, 일반화시키는 것. - 위키피디아
- 추상화의 핵심은 주어진 맥락에서 관련 있는 정보를 남기고, 관련 없는 정보는 잊어버리는 것이다. - John.V.Guttag

- 사용자 인터페이스 쪽으로 갈수록 정보가 간단해지고, 하드웨어쪽으로 갈수록 정보가 복잡해짐
Q. 파일을 저장하기 위해서, 프로그램이 어떻게 저장장치에 정보를 저장하는지(전공지식)를 알 필요가 있을까?
- 운영체제는 하드웨어와 맞닿아있고, I/O에 관여함 -> 사용자는 추상화된 정보를 통해서 파일을 쉽게 저장할 수 있음


### 2. 자원 관리 ex) 멀티 프로그래밍 - CPU 사용 시간 관리
- 프로그램 실행에서 I/O가 차지하는 시간은 8~90%, CPU는 10% 내외의 시간만 사용
<a href="https://ibb.co/BBhSCtZ"><img src="https://i.ibb.co/5LQfR68/IMG-1443.jpg" alt="IMG-1443" border="0"></a>

- 위의 그림에서 색칠된 부분이 CPU 사용 시간
- 한 번에 하나의 프로그램만 실행한다면, CPU는 오랜 시간 놀게 될 것(CPU 사용률 낮음)
- 하지만 동시에 여러 프로그램을 실행해, CPU가 여러 프로그램을 돌며 연산하게 한다면, CPU 사용률을 훨씬 높일 수 있음

## 운영체제의 4대 기능
<a href="https://ibb.co/THcmnB6"><img src="https://i.ibb.co/BgLq7Vb/IMG-1444.jpg" alt="IMG-1444" border="0"></a>
1. 프로세스, 쓰레드, 자원 관리
2. 메모리 관리
3. 파일 관리
4. 디바이스 관리

### 운영체제의 다른 기능
5. 보안
6. 타이머
7. 가상화
등 많은 기능을 수행함

## References
1. Operating Systems Concepts_10ed. Silberschatz
2. 강순주 교수님 운영체제 강의+PPT(23.Spring)
3. https://en.wikipedia.org/wiki/Abstraction_(computer_science)