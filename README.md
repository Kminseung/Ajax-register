# Ajax-register
Implementing member registration function using ajax (Java, JSP, MySQL 5.7.18, Apache Tomcat 8.5, BootStrap 3.3.7)

1. DAO(Data Access Object) : 실제로 DB에 접근하는 객체  

2. DTO(Data Transfer Object) : 계층간 데이터 교환을 위한 객체. DB에서 꺼낸 데이터를 Entity를 가지고 만드는 일종의 Wrapper라고 볼 수 있는데 Entity를 Controller같은 클라이언트단과 직접 마주하는 계층에 직접 전달하는 대신 DTO를 사용해 데이터를 교환한다.


3. web.xml : WebApplication의 Deployment Descriptor로 XML형식의 파일이다. 모든 WebApplication은 반드시 하나의 web.xml 파일을 가져야 하고 위치는 WEB-INF폴더 아래에 있다. web.xml 파일의 설정들은 WebApplication 시작 시 메모리에 로딩된다. 브라우저가 Java Servlet에 접근하기 위해 WAS에 필요한 정보를 알려줘야 해당하는 Servlet을 호출할 수 있으며 이것을 정하는 곳이 web.xml이다.
