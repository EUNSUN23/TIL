### reducer 룰

- action에 따라 state구조를 바꾸는 함수.
- oldState를 첫번째, action을 두번째 인자로 받는다.
- action creator에 의해 만들어진 action에 의해 호출된다.
- 첫 생성시 자동으로 실행되고, 초기 state값을 첫번째 인자로 받는다.
- 첫 자동실행 이후에 첫번째 인자로 받는 것은 바로 직전에 return한 state값이다.
- undefined를 제외한 모든 종류의 value를 리턴할 수 있다.
- **\***reducer는 순수하게 api 요청을 하거나, 파일을 읽거나... dom에 접근하거나
  해서는 안된다. 오직 인자로 받은 previous state와 action object에 의해서만 무엇을 return할지
  결정해야한다.
- 인자로 받은 state를 내부에서 변형시킬 수 없다.
