#Spring #면접질문 
# 1. 정의
- Model, View, Controller로 나누어서 각각의 역할을 분담하여 처리하도록 하는 방법론.
- Model을 통해 값을 전달하므로 컨트롤러는 service, repository와만 소통하며 값을 받아 view에 전달만 하면 된다.
- View는 Model을 통해 전달받은 값을 가지고 클라이언트에게 화면을 반환하는 역할만 맡는다.

## MVC Model 1
- 컨트롤러와 뷰가 물리적으로 분리되지 않았다
- 위는 자바코드로 control, 아래는 html로 view를 구분함
## MVC Model2
- 컨트롤러와 뷰가 물리적으로 나누어진 구조. 
- 뷰파일은 사용자 요청이 있을때에만 서블릿으로 만들어짐. 미리 컴파일되어있어서 유지관리가용이
- 컨트롤러(서블릿)에서 뷰(서블릿)로 dispatcher를 통해서 forwarding된다 (*이 부분이 나중에 front controller가 되어 spring의 영역이 됨*)

# 2. Model
- 값을 전달하는 객체.
- Servlet에 담아서 전달하기엔 Servlet이 전역객체이므로, 해당 값만 전달할 수 있는 Model이 생성되었다.

# 3. View
- Model에서 값을 받아 화면에 반환하는 역할.
- [[JSP]]
- [[Thymeleaf]]
# 4. Controller
- 클라이언트 요청에 따라 어느 곳으로 가야할지 선별하는 역할. 
- 원래 어느 컨트롤러를 호출하는지 판별하는 프론트 컨트롤러가 있으나, spring에서는 spring이 역할을 대신 해주므로 프론트 컨트롤러를 별도로 만들 필요가 없어졌다.
-  컨트롤러는 클라이언트 요청을 받아 Service 단과 소통하며 처리된 결과값을 view로 전달하는 중추 역할을 한다

# 5. Service
- 업무로직을 기준으로 하는 파트. 데이터를 가공하여 업무로직에 맞게 처리하는 역할.
- Service를 interface형태로 정의하고, ServiceImp 에서 각 인터페이스를 구현하여 구체적으로 업무처리를 한다.
- 업무로직에 따라 Service가 구성된다.
- Repository객체를 주입해서 사용하는데, 이때 service를 주입해서 서비스 함수끼리 섞이면 안된다.

# 6. Repository
- 데이터베이스를 담당하는 파트.
- DBMS에 접속할 수 있는 DAO를 사용하기도 하며, [[JDBC]]를 사용해서 repository interface를 생성하고 Mapper를 구현하는 방식으로 접근하였다.

# 7. Dao
- Data access object
- DBMS를 사용하기위해 SQL문을 직접 구현하는 대신, 데이터베이스에 접근할 수 있는 object를 통해서 접근하고자 한다
- [[JDBC]]
- [[Mybatis]]
