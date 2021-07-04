# Redux

##### Redux란?

Redux는 "action"이라는 이벤트를 사용하여 전역 애플리케이션 상태를 관리하고 업데이트하기위한 패턴 및 라이브러리입니다. 데이터를 한 군데로 몰아넣고, 여기저기에서 꺼내볼 수 있게 중앙 저장소 역할을 합니다.

##### 상태관리

동일한 상태를 공유하고 사용해야하는 여러 구성 요소가있는 경우 특히 이러한 구성 요소가 응용 프로그램의 다른 부분에있는 경우 단순성(단방향 데이터 흐름)이 무너질 수 있습니다 . 때때로 이것은 부모 컴포넌트로 "상태를 올려서" 해결할 수 있지만 항상 도움이되는 것은 아닙니다.

이를 해결하는 한 가지 방법은 구성 요소에서 공유 상태(state)를 추출하여 구성 요소 트리 외부의 중앙 위치에 배치하는 것입니다. 이를 통해 컴포넌트 트리는 큰 "뷰"가되고 모든 컴포넌트는 트리의 어디에 있든 상관없이 상태에 액세스하거나 작업을 트리거 할 수 있습니다.

상태 관리와 관련된 개념을 정의 및 분리하고 뷰와 상태 간의 독립성을 유지하는 규칙을 시행함으로써 코드에 더 많은 구조와 유지 관리를 제공합니다.

<img src='https://ko.redux.js.org/assets/images/one-way-data-flow-04fe46332c1ccb3497ecb04b94e55b97.png' width=80%>

##### redux 용어

- state
  리덕스에서는 저장하고 있는 상태값("데이터"라고 생각하셔도 돼요!)를 state라고 불러요.  
   딕셔너리 형태({[key]: value})형태로 보관합니다

- action
  action은 자바스크립트 객체이고, 상태에 변화가 필요할 때(=가지고 있는 데이터를 변경할 때) 발생하는 것입니다.

- action creator
  action 객체를 생성하고 반환하는 함수입니다.

- reducer
  state와 action객체를 업데이트하고, 새로운 상태를 반환합니다.  
  액션 생성 함수를 부르고 → 액션을 만들면 → 리듀서가 현재 상태(=데이터)와 액션 객체를 받아서 → 새로운 데이터를 만들고 → 리턴해줍니다.

- store
  프로젝트에 리덕스를 적용하기 위해 만드는 거예요!
  스토어에는 리듀서, 현재 애플리케이션 상태, 리덕스에서 값을 가져오고 액션을 호출하기 위한 몇 가지 내장 함수가 포함되어 있습니다.
  생김새는 딕셔너리 혹은 json처럼 생겼어요.

- dispatch
  상태를 업데이트하고 작업 객체 를 호출 하고 전달하는 것 입니다

- selector
  store state value에서 특정 정보를 추출하는 함수입니다.

##### redux 애플리케이션 데이터 흐름

<img src='https://ko.redux.js.org/assets/images/ReduxDataFlowDiagram-49fa8c3968371d9ef6f2a1486bd40a26.gif' width=80% >

- UI가 action을 전달합니다.
- store는 reducer를 실행하고 발생한 상황에 따라 state가 업데이트됩니다.
- store은 state가 변경되었음을 UI에 알립니다.
- 새로운 state에 따라 UI가 다시 렌더링됩니다.

출처 : [https://ko.redux.js.org/tutorials/essentials/part-1-overview-concepts#terminology](https://ko.redux.js.org/tutorials/essentials/part-1-overview-concepts#terminology)
