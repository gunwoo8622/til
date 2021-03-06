# 스택 stack, 큐 queue

#### stack

스택(stack)은 제한적으로 접근할 수 있는 나열 구조이다. 그 접근 방법은 언제나 목록의 끝에서만 일어난다. 끝먼저내기 목록(Pushdown list)이라고도 한다.

스택은 한 쪽 끝에서만 자료를 넣거나 뺄 수 있는 선형 구조(LIFO - Last In First Out)으로 되어 있다. 자료를 넣는 것을 '밀어넣는다' 하여 푸쉬(push)라고 하고 반대로 넣어둔 자료를 꺼내는 것을 팝(pop)이라고 하는데, 이때 꺼내지는 자료는 가장 최근에 푸쉬한 자료부터 나오게 된다. 이처럼 나중에 넣은 값이 먼저 나오는 것을 LIFO 구조라고 한다.

이를테면, a부터 b와 c를 순서대로 넣은 다음 자료를 하나씩 꺼내면 c부터 b와 a의 순서로 나오게 된다. S를 스택, x를 데이터 요소(element)라고 하자. 그러면 스택에서는 아래와 같은 중요한 연산이 존재하는 것을 알 수 있다.

- S.top(): 스택의 가장 윗 데이터를 반환한다. 만약 스택이 비었다면 이 연산은 정의불가 상태이다.
- S.pop(): 스택의 가장 윗 데이터를 삭제한다. 스택이 비었다면 연산 정의불가 상태.
- S.push(): 스택의 가장 윗 데이터로 top이 가리키는 자리 위에(top = top + 1) 메모리를 생성, 데이터 x를 넣는다.
- S.empty(): 스택이 비었다면 1을 반환하고,그렇지 않다면 0을 반환한다.

<img src=https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Data_stack.svg/300px-Data_stack.svg.png>

출처 : [https://ko.wikipedia.org/wiki/%EC%8A%A4%ED%83%9D](https://ko.wikipedia.org/wiki/%EC%8A%A4%ED%83%9D)

#### 큐

큐(queue)는 컴퓨터의 기본적인 자료 구조의 한가지로, 먼저 집어 넣은 데이터가 먼저 나오는 FIFO (First In First Out)구조로 저장하는 형식을 말한다. 영어 단어 queue는 표를 사러 일렬로 늘어선 사람들로 이루어진 줄을 말하기도 하며, 먼저 줄을 선 사람이 먼저 나갈 수 있는 상황을 연상하면 된다.

나중에 집어 넣은 데이터가 먼저 나오는 스택과는 반대되는 개념이다.

프린터의 출력 처리나 윈도 시스템의 메시지 처리기, 프로세스 관리 등 데이터가 입력된 시간 순서대로 처리해야 할 필요가 있는 상황에 이용된다.

큐는 put(insert)와 get(delete)을 이용하여 구현된다. put는 큐에 자료를 넣는 것을, get은 큐에서 자료를 꺼내는 것을 의미한다. front(head)와 rear(tail)는 데이터의 위치를 가리킨다! front는 데이터를 get할 수 있는 위치를, rear은 데이터를 put할 수 있는 위치를 의미한다. 또, 큐가 꽉 차서 더 이상 자료를 넣을 수 없는 경우(put 할 수 없는 경우)를 오버플로우(Overflow), 큐가 비어 있어 자료를 꺼낼 수 없는 경우(get 할 수 없는 경우)를 언더플로우(Underflow)라고 한다.

출처 : [https://ko.wikipedia.org/wiki/%ED%81%90*(%EC%9E%90%EB%A3%8C*%EA%B5%AC%EC%A1%B0)](<https://ko.wikipedia.org/wiki/%ED%81%90_(%EC%9E%90%EB%A3%8C_%EA%B5%AC%EC%A1%B0)>)
