# mingi_SpringBoot
<h1>Spring Boot 공부</h1>
<hr>
<h3>Maven 이란?</h3>
  자바의 대표적인 관리 도구였던 Ant를 대체하기 위해 개발됨<br>
  프로젝트의 외부 라이브러리를 쉽게 참조할 수 있게 pom.xxl 파일로 명시하여 관리<br>
  참조한 외부 라이브러리에 연관된 다른 라이브러리도 자동으로 관리됨<br>
<hr>

<h3>Maven 대표 태그 설명</h3>
  modelVersion : maven의 버전을 의미<br>
  groupId : 프로젝트 그룹 id를 뜻하며, 일반적으로 대표하는 사이트 도메인을 역순으로 적어 사용
            (ex : mingi0416.studio -> studio.mingi0416)
  artifactId : groupId외에 다른 프로젝트와는 구분될 수 있는 프로젝트의 Id 작성<br>
  version : 프로젝트의 버전을 의미하며 개발 단계에 따라 구분하여 작성<br>
  name : 프로젝트의 이름<br>
  description : 해당 프로젝트의 간략한 설명을 작성<br>
  properties : pom.mxl 파일 내에서 빈번하게 사용되는 중복 상수를 정의하는 영역
               해당 영영의 상우를 사용하기 위해서는 ${태그명} 의 형태로 사용하면 됨<br>
  dependendies : 해당 프로젝트에서 의존성을 가지고 사용하는 라이브러리를 정의하는 영역
                 각 라이브러리마다 <dependency> 태그를 사용하여 구분<br>
  build : 프로젝트 빌드와 관련된 정보를 설정하는 영역<br>
<hr>

<h3>Gradle 이란?</h3>
  Groovy 스크립트를 활용한 빌드 관리 도구
  안드로이드 프로젝트의 표준 빌드 시스템으로 채택
  멀티 프로젝트의 빌드에 최적화 하여 설계됨<br>
  Maven에 비해 더 빠른 처리속도를 가지고 있음(최대 100배정도 처리속도 차이가 남)<br>
  Maven에 비해 더 간결한 구성이 가능함
<hr>

<h3>Gradle 대표 용어 설명</h3>
repositories : 라이브러리가 저장된 위치 등 설정<br>
mavenCentral : 기본 Maven Repository<br>
dependencies : 라이브러리 사용을 위한 의존성 설정<br>
<hr>

<h3>Gradle과 Maven 비교</h3>
Gradle에 비해 Maven이 점유율이 더 높은 상황 (점차 Gradle 점유율 오르는 중)<br>
Gradle에 비해 Maven의 성능이 떨어짐<br>
Maven에 비해 Gradle이 대규모 프로젝트에서 성능이 좋음<br>
Maven : pom.xml   Gradle : build.gradle<br>
Gradle은 설치 없이 사용할 수 있다(Gradle Wrapper)<br>
<hr>

<h3>대표 Repository Site</h3>
Maven Repository : https://mvnrepository.com/
<hr>

<h3> 디자인 패턴이란? </h3>  
(소프트웨어)디자인 패턴이란 특정 문맥에서 공통적으로 발생하는 문제에 대해 쓰이는 재사용 가능한 해결책<br>
목적별로 일정한 패턴이 제시되어 있음 <br>
완전한 정답이 되는 알고리즘과 달리 현재 상황에 맞춰 최적화된 패턴을 결정하여 사용하는 것이 좋음 <br>
대표적으로 구체화된 디자인 패턴은 GoF(Gang of Four)에서 제시한 총 23개의 패턴이 있음 <br>
  <hr>
  
  <h3> 디자인 패턴의 장점</h3>
  개발자 간의 원할한 협업이 가능 <br>
  소프트웨어의 구조를 파악하기 용이함 <br>
  재사용을 통해 개발 시간 단축 <br>
  설계 변경이 있을 경우 비교적 원할하게 조치가 가능 <br>
  <hr>
  
  <h3> 디자인 패턴의 단점</h3>
  객체지향적 설계를 고려하여 진행해야 함 <br>
  초기 투자 비용이 많이 들어감 (돈 뿐만 아니라 시간 등 포함) <br>
  <hr>
  
  <h3> 디자인 패턴 정리한 사이트 공유</h3>
  https://4z7l.github.io/2020/12/25/design_pattern_GoF.html
  <hr>
  
  <h3>API란?</h3>
  Application Programming Interface의 줄임말 <br>
  응용 프로그램에서 사용할 수 있도록 다른 응용 프로그램을 제어할 수 있게 만든 인터페이스를 뜻함 <br>
  API를 사용하면 내부 구현 로직을 알지 못해도 정의되어 있는 기능을 쉽게 사용할 수 있음 <br>
  <br>
  여기서 인터페이스란 어떤 장치간 정보를 교환하기 위한 수단이나 방법을 의미함 <br>
  대표적인 인터페이스 예로는 마우스, 키보드, 터치패드 등이 있음 <br>
  <hr>
  
  <h3>REST란?</h3>
  REST는 Representational State Transfer(자원상태전달)의 줄임말로 <br>
  자원의 이름으로 구분하여 해당 자원의 상태를 교환하는 것을 의미  <br>
  REST는 서버와 클라이언트의 통신 방식 중 하나임 <br>
  HTTP URI를 통해 자원을 명시하고 HTTP Method를 통해 자원을 교환하는 것 <br>
  <br>
  *HTTP Method : Create, Read, Update, Delete <br>
  <hr>
  
  <h3>REST 특징</h3>
  <h5>Server-Clinet 구조</h4>
  자원이 있는 쪽이 Server, 요청하는 쪽이 Client <br>
  클라리언트와 서버가 독립적으로 분리되어 있어야 함<br>
  <br>
  
  <h4>Stateless</h4>
  요청 간에 클라이언트 정보가 서버에 저장되지 않음 <br>
  서버는 각각의 요청을 완전히 별개의 것으로 인식하고 처리 <br>
<br>
  
  <h4>Cacheable</h4>
  HTTP 프로토콜을 그대로 사용하기 때문에 HTTP의 특징인 캐싱 기능을 적용 <br>
  대량의 요청을 효율적으로 처리하기 위해 캐시를 사용 <br>
<br>
  
  <h4>계층화(Layered System)</h4>
  클라리언트는 서버의 구성과 상관 없이 REST API 서버로 요청 <br>
  서버는 다중 계층으로 구성될 수 있음 (로드밸런싱, 보안 요소, 캐시 등) <br>
  <br>
  
  <h4> Code on Demand(Optional) </h4>
  요청을 받으면 서버에서 클라이언트로 코드 도는 스크립트(로직)을 전달하여 클라이언트 기능 확장 <br>
  <br>
  
  <h4> 인터페이스 일관성 (Uniform Interface)</h4>
  정보가 표준 형식으로 전송되기 위해 구성 요소간 통합 인터페이스를 제공 <br>
  HTTP 프로토콜을 따르는 모든 플랫폼에서 사용 가능하게끔 설계 <br>
  <hr>
  
  <h3>REST의 장점</h3>
  HTTP 표준 프로토콜을 사용하는 모든 플랫폼에서 호환 가능 <br>
  서버와 클라이언트의 역할을 명확하게 분리 <br>
  여러 서비스 설계에서 생길 수 있는 문제를 최소화 <br>
  <hr>
  
  <h3>REST API란?</h3>
  REST 아키텍처의 조건을 준수하는 어플리케이션 프로그래밍 인터페이스를 뜻함 <br>
  최근 많은 API가 REST API로 제공되고 있음 <br>
  일반적으로 REST 아키텍처를 구현하는 웹 서비스를 RESTful 하다고 표현한다 <br>
  <hr>
  
  <h3>REST API 특징</h3>
  REST 기반으로 시스템을 분산하여 확장성과 재사용성을 높임 <br>
  HTTP 표준을 따르고 있어 여러 프로그래밍 언어로 구현할 수 있음 <br>
  <hr>
  
  <h3>REST API 설계 규칙</h3>
  <h4>웹 기반의 REST API를 설계할 경우에는 URI를 통해 자원을 표현해야 함</h4>
  https://thinkground.studio/member/589 <br>
  Resource : member <br>
  Resource id : 589 <br>
  
  <h4>자원에 대한 조작은 HTTP Method(CRUD)를 통해 표현해야 함</h4>
    URI에 행위가 들어가면 안됨 <br>
  HEADER를 통해 CRUD를 표현하여 동작을 요청해야 함 <br>
  
  <h4>메세지를 통한 리소스 조작</h4>
  HEADER를 통해 content-type을 지정하여 데이터를 전달 <br>
  대표적 형식으로는 HTML, MXL, JSON, TEXT가 있음 <br>
  <hr>
  
  <h3>REST API 설계 규칙</h3>
  URI에는 소문자를 사용 <br>
  Resource으 ㅣ이름이나 URI가 길어질 경우 하이픈(-)을 통해 가독성을 높일 수 있음 <br>
  언더바(_)는 사용하지 않음 <br>
  파일 확장자를 표현하지 않음 <br>
  <hr>
  
  <h3>pom.mxl</h3>
  Maven 프로젝트를 생성하면 루트 디렉토리에 생성되는 파일 <br>
  Project Object Model 정보를 담고 있음 <br>
  주요 설정 정보 <br>
  - 프로젝트 정보 : 프로젝트의 이름, 개발자 목록, 라이센스 등 <br>
  - 빌드 설정 정보 : 소스, 리소스, 라이프 사이클 등 실행할 플러그인 등 <br>
  - POM 연관 정보 : 의존 프로젝트(모듈), 상위 프로젝트, 하위 모듈 등 <br>
  <hr>
  
  <h3>프로젝트 기본 정보</h3>
  pom 파일에서 프로젝트 정보와 관련된 태그는 아래와 같음 <br>
  name : 프로젝트 명<br>
  url : 프로젝트 사이트 URL<br>
  description : 프로젝트에 대한 간단한 설명<br>
  organization : 프로젝트를 관리하는 단체 설명<br>
  <hr>
  
  <h3>프로젝트 연관 정보</h3>
  pom 파일에서 프로젝트 정보와 관련된 태그는 아래와 같음<br>
  groupId : 프로젝트의 그룹 ID 설정<br>
  artifactId : 프로젝트 아티팩트 ID 설정<br>
  version : 프로젝트의 버전<br>
  packaging : 패키징 타입 설정<br>
  -jar : 자바 프로젝트 압축 파일<br>
  -war : 웹 어플리케이션을 위한 패키징 방식<br>
  <hr>
  
  <h3>프로젝트 의존 설정</h3>
  프로젝트에서 사용하는 라이브러리에 대한 의준성 설정과 관련된 태그는 아래와 같음 <br>
  dependencies : 라이브러리 의존성 정보를 가지고 있는 dependency 태그를 묶은 태그<br>
  dependency : 각 라이브러리 정보를 담는 태그<br>
  groupId : 의존성 라이브러리의 group ID<br>
  artifactId : 의존성 라이브러리의 아티팩트 ID<br>
  version : 의존성 라이브러리의 버전<br>
  scope : 해당 라이브러리의 이용 범위를 지정<br>
  optional : 다른 프로젝트에서 이 프로젝트를 의존성 설정을 할 경우 사용할지 결정<br>
  <hr>
  
  <h3>scope 태그</h3>
  <h4> compile(default) </h4>
  아무것도 지정되지 않았을 경우 설정되는 값 <br>
  이 값으로 설정하는 경우 모든 클래스 경로에서 사용할 수 있음 <br>
  컴파일 및 배포 상황에서 같이 제공됨 <br>
  
  <h4> provided </h4>
  compile과 유사 하지만 JDK 혹은 Container가 런타임 시에만 제공 <br>
  컴파일 혹은 테스트 경로에서만 사용하며, 배포 시에는 빠짐 <br>
  
  <h4> runtime </h4>
  컴파일 시에는 사용하지 않고, 실행 상황에서만 사용됨 <br>
  런타임과 테스트 경로에서는 있지만, 컴파일 클래스 경로에는 존재하지 않음 <br>
  
  <h4> test </h4>
  테스트 상황에서만 사용되는 라이브러리를 의미 <br>
  실 가동 상황에서는 필요 없는 라이브러리를 사용할 경우에 설정 <br>
  종속된 다른 프로젝트에는 영향을 미치지 않음 <br>
  
  <h4> system </h4>
  provide와 유사하지만 저장소에서 관리되지 않고 직접 관리하는 JAR를 추가 <br>
  systemPath를 추가해서 작성해야함
  <hr>
  
  <h3>mingi_spring boot 프로젝트에 현재 시점에 설정되어 있는 라이브러리 설명(향후 업데이트 예정)</h3>
  
  <h4>Spring Boot Starter Parent </h4>
  프로젝트에서 사용하는 다양한 라이브러리 간의 버전 충돌 문제가 발생할 수 있는 것을 방지 <br>
  의존성 조합간 충돌 문제가 없는 검증된 버전 정보 조합을 제공 <br>
  
  <h4>Spring Boot Starter Web </h4>
  Spring MVC를 사용한 REST 서비스를 개발하는데 사용 <br>
  
  <h4>Spring Boot Starter Test</h4>
  JUnit, Hamcrest, Mockito를 포함한 스프링 어플리케이션의 데스트 기능을 제공 <br>
  <hr>
  
  <h3>MVC패턴</h3>
  <h4> MVC (Model View Controller)</h4>
  디자인 패턴 중 하나인 MVC 패턴은 Model, View, Controller의 줄임말로 어플리케이션을 구성할 때 <br>
  그 구성요소를 세가지의 역할로 구분한 패턴을 의미 <br>
  사용자 인터페이스로부터 비즈니스 로직을 분리하여 서로 영향 없이 쉽게 고칠 수 있는 설계가 가능 <br>
  <hr>
  
  <h3>컨트롤러(Controller)</h3>
  모델과 뷰 사이에서 브릿지 역할을 수행 <br>
  앱의 사용자로부터 입력에 대한 응답으로 모델 및 뷰를 업데이트 하는 로직을 포함 <br>
  사용자의 요청은 모두 컨트롤러를 통해 진행되어야 함 <br>
  컨트롤러로 들어온 요청은 어떻게 처리할지 결정하여 모델로 요청을 전달함 <br>
  <br>
  예) 쇼핑몰에서 상품을 검색하면 그 키워드를 컨트롤러가 받아 모델과 뷰에 적절하게 입력을 처리하여 전달함
  <hr>
  
  <h3>모델(Model)</h3>
  데이터를 처리하는 영역 <br>
  데이터베이스와 연동을 위한 DAO(Data Access Object)와 데이터의 구조를 표현하는 DO(Data Object)로 구성됨 <br>
  <br>
  예) 검색을 위한 키워드가 넘어오면 데이터베이스에서 관련된 상품의 데이터를 받아 뷰에 전달 <br>
  <hr>
  
  <h3>뷰(View)</h3>
  데이터를 보여주는 화면 자체의 영역을 뜻함 <br>
  사용자 인터페이스(UI) 요소들이 여기에 포함되며, 데이터를 각 요소에 배치함 <br>
  뷰에서는 별도의 데이터를 보관하지 않음 <br>
  <br>
  예) 검색 결과를 보여주기 위해 모델에서 결과 상품 리스트 데이터를 받음<br>
  <hr>
  
  <h3>MVC 패턴의 특징</h3>
  어플리케이션의 역할을 세 구간으로 나누어 설계함으로써 서로 간의 의존성이 낮아짐 <br>
  각 영역이 독립적으로 구성되어 개발자 간 분업 및 협업이 원활해짐 <br>
  한 영역을 업데이트 하더라도 다른 곳에 영향을 주지 않음 <br>
  <hr>
  
  <h3>@RestController</h3>
  Spring Framwork 4버전부터 사용가능한 어노테이션<br>
  @Controller에 @responseBody가 결합된 어노테이션 <br>
  컨트롤러 클래스 하위 메소드에 @ResponseBody 어노테이션을 붙이지 않아도 문자열과 JSON 등을 전송할 수 있음 <br>
  View를 거치지 않고 HTTP ResponseBody에 직접 Return값을 담아 보내게 됨 <br>
  <hr>
  
  <h3>첫 기능 만들기</h3>
  <h4> 도식화 </h4>
  <br>
  <p>
  <img src = "https://user-images.githubusercontent.com/70953813/223666496-561c748e-a9ac-4cdb-b61e-5d10642405af.PNG">
  </p>
  <hr>
  
  <h3>@RequestMapping</h3>
  MVC의 핸들러 매핑을 위해서 DefaultAnnotationHandlerMapping을 사용 <br>
  DefaultAnnotationHandlerMapping 매핑정보로 @RequestMapping 어노테이션을 활용 <br>
  클래스와 메소드의 RequestMapping을 통해 URL을 매핑하여 경로를 설정하여 해당 메소드에서 처리 <br>
  <br>
  value : url 설정<br>
  method : GET, POST, DELETE, PUT, PATCH 등<br>
  <br>
  스프링은 4.3버전 부터 메소드를 지정하는 방식보다 간단하게 사용할 수 있는 어노테이션을 사용할 수 있음 <br>
  -@GetMapping <br>
  -@PostMapping <br>
  -@DeleteMapping <br>
  -@PutMapping <br>
  -@PatchMapping <br>
  
  <hr>
  
  <h3>@GetMapping(without Param)</h3>
  별도의 파라미터 없이 GET API를 호출하는 경우 사용되는 방법 <br>
  <p>
  <img src = "https://user-images.githubusercontent.com/70953813/223693626-2c5fc9b1-34be-4054-88d2-89a913b0da61.PNG">
  </p>
  <hr>
  
  <h3>@PathVariable</h3>
  GET 형식의 요청에서 파라미터를 전달하기 위해 URL에 값을 담아 요청하는 방법 <br>
  아래 방식은 @GetMapping에서 사용된 {변수}의 이름과 메소드의 매개변수와 일치시켜야 함<br>
  <p>
  <img src = "https://user-images.githubusercontent.com/70953813/223694142-6cfab462-da54-445e-9395-3c70b99b6b23.PNG">
  <br>
  변수의 관리의 용이를 위해 사용되는 방식<br>
  variable의 값과 String 변수의 이름을 동일하게 하지 못할때 밑의 방법으로 사용<br>
  PathVariable의 괄호 안에 variable 값을 일치시켜서 사용 <br>
  <p>
  <img src = "https://user-images.githubusercontent.com/70953813/223694842-3399d95e-f7f2-4c71-b4d1-86ce4d36327d.PNG">
  <p>
  
  <hr>
  
  <h3>@RequestParam</h3>
  GET 형식의 요청에서 쿼리 문자열을 전달하기 위해 사용되는 방법 <br>
  '?'를 기준으로 우측에 {키}={값}의 형태로 전달되며, 복수 형태로 전달할 경우 &를 사용함<br>
  <p>
  <img src = "https://user-images.githubusercontent.com/70953813/223698274-c105a7ca-491a-4b18-9471-cef0ab4f40cb.PNG">
  <p>
  <br>
  아래 예시 코드는 어떤 요청 값이 들어올지 모를 경우 사용하는 방식<br>
  <p>
  <img src = "https://user-images.githubusercontent.com/70953813/223699246-5b6a4e59-9c14-4a40-b78a-5438b86900ad.PNG">
  <p>
  <hr>
  
  <h3>DTO 사용</h3>
  GET 형식의 요청에서 쿼리 문자열을 전달하기 위해 사용되는 방법 <br>
  key와 value가 정해져있지만, 받아야할 파라미터가 많을 경우 DTO 객체를 사용한 방식<br>
  <p>
  <img src = "https://user-images.githubusercontent.com/70953813/223699760-3e7fc84e-f2db-434b-b8df-29a6f4d2d8ad.PNG">
  <p>
  <hr>
  
  <h3>Post API</h3>
  리소스를 추가하기 위해 사용되는 API <br>
  @PostMapping : POST API를 제작하기 위해 사용되는 어노테이션, @RequestMapping + POST method의 조합 <br>
  일반적으로 추가하고자 하는 Resource를 http body에 추가하여 서버에 요청 <br>
  그렇기 때문에 @RequestBody를 이용하여 body에 담겨있는 값을 받아야함 <br>
  <p>
    <img src = "https://user-images.githubusercontent.com/70953813/223707927-e4caf518-3df8-4e45-9cb1-f589882891ee.PNG">
  </p>
  
  <hr>
  
  <h3>DTO 사용</h3>
  key와 value가 정해져있지만, 받아야할 파라미터가 많을 경우 DTO 객체를 사용한 방식<br>
  @RequestBody를 안넣을시 Null 값으로 처리됨
  <p>
    <img src = "https://user-images.githubusercontent.com/70953813/223708380-de24b457-9b15-4add-a931-467e898eddff.PNG">
  <hr>
  
  <h3>Swagger란?</h3>
  협업을 위해 필요한 라이브러리 <br>
  서버로 요청되는 API 리스트를 HTML 화면으로 문서화하여 테스트 할 수 있는 라이브러리 <br>
  이 라이브러리는 서버가 가동되면서 @RestController를 읽어 API를 분석하여 HTML 문서를 작성함<br>
  <hr>
  
  <h3>Swagger가 필요한 이유</h3>
  REST API의 스펙을 문서화 하는 것은 매우 중요 <br>
  API를 변경할 때마다 Reference 문서를 계속 바꿔야하는 불편함이 있음<br>
  <hr>
  
  <h3>Swagger 설정 방법</h3>
  @Configuration : 어노테이션 기반의 환경 구성을 돕는 어노테이션, IoC Container에게 해당 클래스를 Bean 구성 Class임을 알려줌<br>
  @Bean : 개발자가 직접 제어가 불가능한 외부 라이브러리 등을 Bean으로 만들 경우에 사용<br>
  링크 : http://localhost:8080/swagger-ui.html
  <hr>
  
  <h3>Put API</h3>
  해당 리소스가 존재하면 갱신하고, 리소스가 없을 경우에는 새로 생성해주는 API <br>
  업데이트를 위한 메소드 <br>
  기본적인 동작 방식은 Post API와 동일 <br>
  <hr>
  
  <h3>Delete API</h3>
  서버를 통해 리소스를 삭제 하기 위해 사용되는 API <br>
  일반적으로 @Pathvariable을 통해 리소스 ID 등을 받아 처리
  <hr>
  
  <h3>ResponseEntity</h3>
  Spring Framework에서 제공하는 클래스 중 HttpEntity라는 클래스를 상속받아 사용하는 클래스<br>
  사용자의 HttpRequest에 대한 응답 데이터를 포함<br>
  포함하는 클래스 <br>
  -HttpStatus <br>
  -HttpHeaders <br>
  -HttpBody <br>
  <hr>
  
  <h3>Lombok이란?</h3>
  반복되는 메소드를 Annotation을 사용하여 자동으로 작성해주는 라이브러리<br>
  일반적으로 VO, DTO, Model, Entity등의 데이터 클래스에서 주로 사용됨 <br>
  대표적으로 많이 사용되는 Annotation <br>
  -@Getter <br>
  -@Setter <br>
  -@NoArgConstructor <br>
  -@AllArgConstuctor <br>
  -@Data <br>
  -@ToString <br>
  <hr>
  
  <h3>Lombok 사용법</h3>
  라이브러리 의존성 설정 <br>
  <p>
    <img src = "https://user-images.githubusercontent.com/70953813/223726213-c327c713-2237-4ba5-a2cb-7c660e5e7eb2.PNG">
  </p>
  <hr>
  
  <h3>Lombok의 대표적인 어노테이션</h3>
  @Getter, @Setter <br>
  해당 클래스에 선언되어 있는 필드를 기반으로 'getField', 'setField'와 같은 식으로 자동으로 메소드를 생성 <br>
  <p>
    <img src = "https://user-images.githubusercontent.com/70953813/223726821-1cdd278b-4f69-4e36-91bd-2d1159b2af02.PNG">
    <img src = "https://user-images.githubusercontent.com/70953813/223726845-79b2c563-8ea9-41d7-b68b-f368129ed8aa.PNG">
  </p>
  <br>
  @NoArgsConstructor // @AllArgsConstructor // @RequiredArgsConstructor <br>
  @NoArgsConstructor : 파라미터가 없는 생성자를 생성<br>
  @AllArgsConstructor : 모든 필드값을 파라미터로 갖는 생성자를 생성<br>
  @RequiredArgsConstructor : 필드값 중 final이나 @NotNull인 값을 갖는 생성자를 생성<br>
  <p>
    <img src = "https://user-images.githubusercontent.com/70953813/223727886-6075c91b-356d-46a7-a5c8-674ae357681d.PNG">
  </p>
  <br>
  @ToString<br>
  toString 메소드를 자동으로 생성해주는 기능 <br>
  @ToString 어노테이션에 exclude 속성을 사용하여 특정 필드를 toString에서 제외시킬 수 있음
  <p>
    <img src="https://user-images.githubusercontent.com/70953813/223728370-c5fd6dc9-a676-4d5a-9bfc-9a733232bef5.PNG">
  </p>
  <br>
  @EqualsAndHashCode <br>
  equals, hashCode 메소드를 자동으로 생성
  equals : 두 객체의 개뇽이 같은지 동등성(equality)를 비교하는 연산자 <br>
  hashCode : 두 객체가 같은 객체인지 동일성(identity)를 비교하는 연산자 <br>
  <br>
  callSuper 속성을 통해 메소드 생성시 부모 클래스의 필드까지 고려할지 여부 설정 가능 <br>
  - callSuper = true -> 부모 클래스 필드 값들도 동일한지 체크 <br>
  <br>
  @Data <br>
  해당 어노테이션을 사용하면, 앞서 나온 기능들을 한번에 추가해줌 <br>
  -@Getter <br>
  -@Setter <br>
  -@RequiredArgsConstructor <br>
  -@ToString <br>
  -EqualsAndHashCode<br>
  <hr>
  
  <h3>Spring Boot 서비스 구조</h3>
  <p>
    <img src="https://user-images.githubusercontent.com/70953813/223731934-12dfb17f-f99c-436c-9aef-6bd701ad138b.PNG">
  </p>
  <br>
  
  <hr>
  
  <h3>Entity(Domain)</h3>
  데이터베이스에 쓰일 컬럼과 여러 엔티티 간의 연관관계를 정의 <br>
  데이터베이스의 테이블을 하나의 엔티티로 생각해도 무방함 <br>
  실제 데이터베이스의 테이블과 1:1로 매핑됨 <br>
  이 클래스의 필드는 각 테이블 내부의 컬럼(Column)을 의미 <br>
  <hr>
  
  <h3>Repository</h3>
  Entity에 의해 생성된 데이터베이스에 접근하는 메소드를 사용하기 위한 인터페이스 <br>
  Service와 DB를 연결하는 고리의 역할을 수행 <br>
  데이터베이스에 적용하고자 하는 CRUD를 정의하는 영역 <br>
  <hr>
  
  <h3>DAO(Data Access Object)</h3>
  데이터베이스에 접근하는 객체를 의미(Persistance Layer)<br>
  Service가 DB에 연결할 수 있게 해주는 역할 <br>
  DB를 사용하여 데이터를 조회하거나 조작하는 기능을 전담 <br>
  <hr>
  
  <h3>DTO(Data Transfer Object)</h3>
  DTO는 VO(Value Object)로 불리기도 하며, 계층간 데이터 교환을 위한 객체를 의미 <br>
  VO의 경우 Read Only의 개념을 가지고 있음 <br>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
  <h3></h3>
  <hr>
  
   
   
