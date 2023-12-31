### 데이터 단방향 바인딩과 양방향 바인딩

- 데이터 바인딩이란 화면상에 보여지는 데이터(View)와 브라우저 메모리에 있는 데이터(Model)를 묶어서(Binding) 서로 간의 데이터를 동기화하는 것입니다.
- 예를들어, HTML에서 서버 혹은 스크립트상에서 받아온 데이터를 화면상에 그려주고 있다고 가정을 했을 때, 해당 값이 변경이 될 경우 다시 HTML 상에 데이터(값)를 변경된 값에 따라서 맞추어 주는 동작입니다.

### 단방향 데이터

- Javascript(Model)에서 HTML(View)로 한 방향으로만 데이터를 동기화하는 것을 의미합니다.
- 단방향 데이터 바인딩이기에 역으로 HTML(View)에서 JS(Model)로의 직접적인 데이터 갱신은 불가능합니다.
- 이벤트 함수(onClick, onChange,...)를 주고 함수를 호출한 뒤 Javascript에서 HTML로 데이터를 변경해야 합니다.
- 컴포넌트 간에서 단방향 데이터 바인딩은 부모 컴포넌트에서 자식 컴포넌트로만 데이터가 전달되는 구조입니다.
- 대표적으로 SPA Framework에서는 React에서 단방향 데이터 바인딩을 합니다.

### 양방향 데이터

- Javascript(Model)와 HTML(View) 사이에 ViewModel이 존재하여 하나로 묶여서(Binding) 되어서 둘 중 하나만 변경되어도 함께 변경되는 것을 의미합니다.
- 컴포넌트 간에서는 부모 컴포넌트에서 자식 컴포넌트로는 Props를 통해 데이터를 전달하고, 자식 컴포넌트에서 부모 컴포넌트로는 Emit Event를 통해서 데이터를 전달하는 구조입니다.
- 대표적으로 SPA Framework에서는 Vue.js, Angular에서 양방향 데이터 바인딩을 합니다.
