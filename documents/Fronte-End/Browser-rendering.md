### 브라우저의 렌더링 과정

1. 브라우저가 HTML, CSS, JS 등 렌더링에 필요한 리소스를 요청하고 서버로부터 응답 받습니다.
2. 브라우저의 렌더링이 HTML을 파싱하여 DOM, CSS를 파싱하여 CSSOM을 생성하고 이들을 결합하여 렌더트리를 생성합니다.
   이때 화면에 렌더링 되지 않는 노드는 포함하지 않습니다.
3. 파싱 중에 script 태그를 만나게 되면 그때부터 Javascript 엔진이Javascript 코드를 파싱하여 추상구문트리(ast)를 만들고 바이트코드로 변환을 하여 실행시킵니다.
   이때 Javascript는 DOM API를 통해 DOM이나 CSSOM을 변경할 수 있고, 변경된 DOM, CSSOM은 다시 렌더트리로 결합됩니다.
4. 렌더 트리를 기반으로 HTML 요소의 레이아웃을 계산하고 브라우저 화면에 paint를 하게 됩니다.

> layout 과정은 cpu, paint 과정은 gpu가 하기 때문에 비용측면에 있어서 layout 과정이 높습니다.
