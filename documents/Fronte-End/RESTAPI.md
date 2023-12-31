### RestAPI?

- REST는 웹 서비스의 아키텍처 스타일 중 하나입니다.
- REST는 자원을 정의하고 해당 자원에 대한 상태를 주고받는 방식으로 서비스를 구현합니다.
- 이 아키텍처 스타일은 네트워크 상에서 분산된 시스템을 위한 간단하고 경량화된 솔루션을 제공합니다.
- REST API는 다음과 같은 주요 특징을 가지고 있습니다.

- 모든 `자원` 은 고유한 식별자를 가지고 있으며, 이를 통해 자원에 접근합니다. 자원은 웹 상에 존재하는 모든 것을 의미할 수 있습니다.
- 자원의 상태는 여러 `형태` 로 표현될 수 있습니다. 주로 사용되는 표현은 JSON 또는 XML형식 입니다. 클라이언트가 자원의 특정 표현을 요청하면 서버는 해당 표현을 제공합니다.
- 각각의 요청은 클라이언트의 상태를 서버에 저장하지 않고, 요청 자체에 필요한 모든 정보를 포함하여 처리됩니다. 이는 서버의 부하를 줄이고 확장성을 높이는 데에 기여합니다.
- REST는 `일관된 인터페이스` 를 제공하기 위해 특정한 규칙을 따릅니다. 이는 리소스에 대한 표준화된 인터페이스를 통해 시스템의 아키텍처를 단순화하고 독립성을 유지합니다.
- 시스템은 `계층 구조` 로 구성될 수 있어, 각 계층은 특정한 역할을 수행하고 상위 계층은 하위 계층의 구현 내용을 알 필요가 없습니다. 이는 시스템의 확장성과 유지보수성을 향상시킵니다.
  REST API는 HTTP 프로토콜을 기반으로 하며, 주로 CRUD 연산을 통해 자원을 관리합니다. 클라이언트는 HTTP 메서드를 사용하여 서버의 자원을 조작합니다. RESTfulAPI는 REST아키텍처 스타일을 따르는 API를 의미하며, 이는 간결하고 효율적인 서비스를 제공할 수 있도록 설계된 API를 의미합니다.
