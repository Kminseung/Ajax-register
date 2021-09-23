# Ajax-register
Implementing member registration function using ajax (Java, JSP, MySQL 5.7.18, Apache Tomcat 8.5, BootStrap 3.3.7)

1. DAO(Data Access Object) : 실제로 DB에 접근하는 객체  

2. DTO(Data Transfer Object) : 계층간 데이터 교환을 위한 객체. DB에서 꺼낸 데이터를 Entity를 가지고 만드는 일종의 Wrapper라고 볼 수 있는데 Entity를 Controller같은 클라이언트단과 직접 마주하는 계층에 직접 전달하는 대신 DTO를 사용해 데이터를 교환한다.


3. web.xml : WebApplication의 Deployment Descriptor로 XML형식의 파일이다. 모든 WebApplication은 반드시 하나의 web.xml 파일을 가져야 하고 위치는 WEB-INF폴더 아래에 있다. web.xml 파일의 설정들은 WebApplication 시작 시 메모리에 로딩된다. 브라우저가 Java Servlet에 접근하기 위해 WAS에 필요한 정보를 알려줘야 해당하는 Servlet을 호출할 수 있으며 이것을 정하는 곳이 web.xml이다.

4. MVC 패턴 : Model, View, Contorller로 구성된 구조이다. 웹페이지를 구성하는 요소들(시각적인 요소, 데이터 담당 요소)들간의 간섭없이 독릭접으로 개발함으로써 큰 효율을 낼 수 있다.
- Model : 데이터를 처리하는 담당. Controller에서 명령을 받고 Database에서의 데이터 CRUD 등의 작업을 수행한다.
- View : 시각적인 부분, 화면을 담당. 화면의 뼈대를 담당하는 html, css, javascript 등을 이용하여 View를 만들어낸다.
- Controller : 사용자가 접근하려는 URL에 따라서 요청사항을 파악한 후 요청에 맞는 Model의 데이터를 의뢰하고 데이터를 View에 반영ㄹ해서 사용자에게 알려준다. 전반적인 제어 담당을 하는 역할이라 할 수 있다.  

예를들어,  
사용자가 웹사이트에 접속 -> Controller는 사용자가 요청한 웹페이지를 제공하기 위해 Model에서 데이터를 호출 -> Model은 데이터베이스나 파일과 같은 데이터 소스를 제어한 후 그 결과를 반환 -> Controller는 Model이 반환한 결과를 View에 반영 -> 데이터가 반영된 View는 사용자에게 보여짐
