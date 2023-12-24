### 호이스팅

호이스팅이란 변수의 정의가 그 범위에 따라 `선언`과 `할당`으로 분리되는 것을 의미합니다. 변수가 함수 내에서 정의되었을 경우, 선언이 함수의 최상위로, 함수 바깥에서 정의되었을 경우, 전역 컨텍스트의 최상위로 변경이 됩니다.

선언문은 자바스크립트 엔진에서 구동시 가장 최우선으로 해석하므로 호이스팅 되고, 할당 구문은 런타임 과정에서 이루어지기 떄문에 호이스팅이 되지 않습니다.

함수가 자신이 위치한 코드에 상관없이 함수 선언문 형태로 정의한 함수의 유효범위는 전체 코드의 맨 처음부터 시작합니다. 함수 선언이 함수 실행 부분보다 뒤에 있더라도 자바스크립트 엔진이 함수 선언을 끌어올리는 것을 의미합니다. 함수 호이스팅은 함수를 끌어올리지만 변수의 값은 끌어올리지 않습니다.

### 호이스팅이 일어나는 이유

자바스크립트 엔진에 두가지 역할이 있습니다. 코드평가와 코드실행이 있습니다. 코드 평가 단계에서 실행할 코드에 대한 정보를 모두 수집합니다. 이 과정에서 자바스크립트 엔진은 모든 스코프(실행컨텍스트)를 탐색하며 각 스코프의 변수 객체에 여러 식별자를 수집합니다. 즉, 실행 시점으로 넘어가기 전에 선언된 식별자에 대한 정보를 이미 수집해놓았기 때문에 실행시점에서 스코프의 어느 지점이든 관련된 함수/변수를 참조할 수 있게 됩니다. 그래서 호이스팅이 필요하게 됩니다.