# styled-components

**styled-components**는 React 컴포넌트 시스템을 스타일링하기 위해 CSS를 어떻게 향상시킬 수 있는지 궁금해한 결과입니다. 단일 사용 사례에 집중함으로써 우리는 개발자를 위한 경험과 최종 사용자를 위한 결과물을 최적화할 수 있었습니다.

- **Automatic critical CSS** : styled-components는 페이지에서 렌더링되는 구성 요소를 추적하고 완전히 자동으로 해당 스타일만 삽입합니다. 코드 분할과 결합하면 사용자가 필요한 최소한의 코드를 로드할 수 있습니다.

- **No class name bugs** : styled-components는 스타일에 대한 고유한 클래스 이름을 생성합니다. 중복, 중복 또는 철자 오류에 대해 걱정할 필요가 없습니다.

- **Easier deletion of CSS** : 클래스 이름이 코드베이스의 어딘가에서 사용되는지 여부를 알기 어려울 수 있습니다. styled-components는 스타일의 모든 비트가 특정 구성 요소에 연결되어 있기 때문에 이를 명확하게 합니다. 구성 요소가 사용되지 않고(도구가 감지할 수 있음) 삭제되면 해당 구성 요소의 모든 스타일도 함께 삭제됩니다.

- **Simple dynamic styling** : 수십 개의 클래스를 수동으로 관리할 필요 없이 props 또는 전역 테마를 기반으로 구성 요소의 스타일을 적용하는 것이 간단하고 직관적입니다.

- **Painless maintenance** : 구성 요소에 영향을 주는 스타일을 찾기 위해 여러 파일을 검색할 필요가 없으므로 코드베이스가 아무리 크더라도 유지 관리는 케이크 조각입니다.

- **Automatic vendor prefixing** : CSS를 현재 표준으로 작성하고 나머지는 styled-components가 처리하도록 합니다.

출처 : [https://styled-components.com/docs/basics](https://styled-components.com/docs/basics)
