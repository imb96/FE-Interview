var, let, const의 차이

var: 함수 스코프를 갖습니다. 즉, 함수 내에서 선언된 경우 해당 함수 내에서만 접근할 수 있습니다. 함수 외부에서 선언되면 전역 변수가 됩니다. 변수의 재선언 및 재할당이 가능하기 때문에 예기치 않은 버그가 발생할 수 있습니다.

let: 블록 스코프를 갖습니다. 재할당은 가능하지만 재선언은 불가능합니다. let을 사용하여 선언된 변수를 선언되기 전에 접근하면 ReferenceError가 발생합니다.

const: 블록 스코프를 갖습니다. 재할당이나 재선언이 불가능한 상수 변수를 생성합니다. 선언시 초기화되어야 하며 한번 초기화되면 값을 변경할 수 없습니다. const 를 사용하여 선언된 변수를 선언되기 전에 접근하면 ReferenceError가 발생합니다.