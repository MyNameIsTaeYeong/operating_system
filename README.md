참고한 곳
- Operating System Concepts by Abraham Silberschatz, Greg Gagne, Peter B. Galvin
- Operating systems internals and design principles by William Stallings
- https://github.com/gyoogle/tech-interview-for-developer

# 운영체제 주요 기능
## 프로세스 관리(동시성 지원)
- Process Isolation을 보장하며 Concurrency지원.
- Shared Resource가 사용됨.
- Race condition(자원의 일관성을 해침) 발생.
- Mutual Exclusion이 필요함.
- 세마포어 지원.
- 세마포어 사용에 있어 atomic operation이 필요함.
- Mutual Exclusion을 위해 Critical Section이 지정됨.
- Shared Resource에 대한 독점권을 주다보니 DeadLock이 발생.
- 이를 해결하기 위해 프로세스에 우선순위를 주다보니 Starvation이 발생.

## 메모리 관리(자원을 효율적으로 활용)
- 프로세스의 조각들의 실제 위치와 순서를 기록한 table이 있다면
  - 프로세스는 메모리에 전부 올라와 있을 필요가 없다.
  - 프로세스는 메모리에 연속적으로 위치할 필요가 없다.
  - 메인메모리용량을 초과하여도 프로세스들을 관리할 수 있다.(가상 메모리)
