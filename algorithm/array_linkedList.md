# Array, Linked List

#### Array

배열은 크기가 정해진 데이터의 공간입니다.
배열은 각 원소에 즉시 접근할 수 있습니다.(rooms[0])  
여기서, 원소의 순서는 0부터 시작하고 이를 인덱스라고 부릅니다.  
이 때, 즉시 접근 가능하다는 말은 상수 시간 내에 접근할 수 있음을 의미합니다.
즉, O(1) 내에 접근할 수 있다고 말하곤 합니다.  
배열은 원소를 중간에 삽입/삭제 하려면 모든 원소를 다 옮겨야 합니다.  
최악의 경우 배열의 길이 N 만큼을 옮겨야 하므로 O(N)의 시간 복잡도를 가집니다.  
인덱스를 새로 추가하려면, 새로운 공간을 할당해야 하므로 매우 비효율적인 자료구조입니다.

#### Linked List

리스트는 크기가 정해지지 않은 데이터의 공간입니다.  
연결 고리로 이어주기만 하면, 자유자재로 늘어날 수 있습니다!  
리스트는 특정 원소에 접근하려면 연결 고리를 따라 탐색해야 합니다.  
최악의 경우에는 모든 칸을 탐색해야 하므로 O(N)의 시간 복잡도를 가집니다.  
여기서, 앞으로 연결 고리를 포인터라 부르고, 각 칸을 노드라고 부르겠습니다.  
리스트는 원소를 중간에 삽입/삭제 하기 위해서는 앞 뒤의 포인터만 변경하면 됩니다.
따라서 원소 삽입/삭제를 O(1)의 시간 복잡도 안에 할 수 있습니다.

#### Array VS LinkedList

|       경우       |                     Array |                   LinkedList |
| :--------------: | ------------------------: | ---------------------------: |
| 특정 인덱스 조회 |                      O(1) |                         O(N) |
|  중간 삽입 삭제  |                      O(N) |                         O(1) |
|   데이터 추가    | 새로운 메모리 공간을 할당 | 맨 뒤의 노드만 동적으로 추가 |
|       정리       |    데이터에 접근하는 경우 |           삽입과 삭제가 빈번 |