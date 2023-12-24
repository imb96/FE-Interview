### 자바스크립트의 프로토타입

자바스크립트는 함수에 자동으로 prototype이라는 객체 타입의 속성을 생성합니다.
new 연산자와 함께 함수를 호출하여 함수를 생성자 함수로써 사용할 경우, 생성된 인스턴스에는 숨겨진 속성인 **proto**(던더프로토) 속성이 자동으로 생성됩니다.
그리고 **proto**속성은 생성자 함수의 prototype속성을 참조합니다. **proto**속성은 생략이 가능하기 때문에 인스턴스에서 생성자 함수의 prototype에 정의된 메서드나 속성에 접근 할 수 있습니다.

### 프로토타입의 동작방식

- 자바스크립트에서 모든 객체는 **`prototype`**이라는 속성을 가지며, **`prototype`**은 해당 객체의 상위 프로토타입 객체를 참조하는 링크 역할을 합니다.
- **`prototype`** 체인은 프로토타입 객체 간에 상속을 가능하게 합니다. 만약 객체에서 어떤 속성이나 메서드를 찾을 때, 해당 객체에 속성이 없다면, 자바스크립트 엔진은 해당 객체의 **`prototype`** 체인을 따라 가장 가까운 프로토타입 객체에서 해당 속성이나 메서드를 찾습니다.
- 이러한 방식으로 프로토타입 체인이 만들어지기 때문에, 자바스크립트에서는 상속을 구현하는 데에 **`prototype`**을 사용합니다. 예를 들어, 생성자 함수를 사용하여 객체를 만들 때, **`prototype`**을 통해 해당 생성자 함수로부터 만들어진 모든 객체가 공유하는 속성과 메서드를 정의할 수 있습니다.
- 이러한 **`prototype`**의 동작 방식은 자바스크립트에서 상속을 구현하는 데에 중요한 역할을 합니다. 상속을 통해 코드의 재사용성을 높이고, 객체지향 프로그래밍의 핵심 개념을 자바스크립트에서도 구현할 수 있게 됩니다.