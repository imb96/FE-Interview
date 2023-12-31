### 클로저

- 클로저는 두 개의 함수로 만들어진 환경으로 이루어진 특별한 객체의 한 종류입니다.
- 여기서 환경이라 함은 클로저가 생성될 때 그 범위에 있던 여러 지역 변수들이 포함된 컨텍스트를 말합니다.
- 이 클로저를 통해서 자바스크립트에는 없는 비공개 속성 메소드, 공개 속성 메소드를 구현할 수 있는 방안을 마련할 수 있습니다.
- 클로저가 생성되는 조건에는 내부 함수가 익명 함수가 되어 외부 함수의 반환값으로 사용되고
- 내부 함수는 외부 함수의 실행 환경에서 실행되며 내부 함수에는 사용되는 변수는 외부 함수의 변수 스코프에 있으면 생성되게 됩니다.
- 이렇게하면 외부 함수 호출이 종료되더라도 외부 함수의 지역 변수 및 변수 스코프 객체의 체인 관계를 유지할 수 있는 있는데 이러한 구조를 클로저라고 하며
- 보다 정확히는 외부 함수에 의해 반환되는 내부함수를 가리키는 말입니다.

### 클로저와 스코프의 관계

- Closure는 함수와 그 함수가 선언됐을 때의 렉시컬 스코프와의 조합입니다.
- 즉, 함수가 선언될 때의 스코프 체인을 유지하면서, 함수가 반환된 이후에도 외부 함수의 변수에 접근할 수 있는 메커니즘입니다.
- 이를 통해, 함수 내부에서 선언된 변수를 외부에서 접근하지 못하도록 보호하면서도,
- 필요한 경우에는 클로저를 이용하여 접근할 수 있습니다.
- 스코프는 함수를 호출할 때마다 생성되며, 함수 실행이 끝나면 스코프는 소멸합니다.
- 하지만, 클로저는 스코프 체인을 유지하면서 스코프가 소멸해도 외부 변수에 접근할 수 있는 메커니즘입니다.
