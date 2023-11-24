#Dao
# 1.정의
- java database connectivity
- 자바에서 데이터베이스에 접속할 수 있도록 하는 자바 [[API]]
- 데이터베이스를 자바를 가지고 select, insert, update, delete 하는 방법을 제공 (쿼리문과 자바의 연결점)
![[Pasted image 20231121174810.png]]

# 2. 탄생배경
- SQL문을 작성할 수 있는 사람들을 위한 쿼리실행도구는 DB client 프로그램. 하지만 SQL문을 작성할 수 없는 사람들을 위한 쿼리실행도구는 업무용 프로그램 ▶ 업무용 프로그램을 위한 쿼리실행도구는 API
- 각 DB업체가 제공하는 api는 통합되어있지 않음 ▶ 통합할 수 있는 API는 JDBC driver *(api를 사용하는 부분을 단일화)*

# 3. 장점
- 자바를 가지고 sql문을 연결하여 데이터를 끌어올 수 있다

# 4. 단점
- 연결을 위해 Connection을 위한 단계를 거쳐야 한다. 
- 구현 코드가 길고 일일히 데이터를 꽂고 만들어내는 과정이 번거로울 수 있다. 
1. DriverManager (드라이버로드) 
2. Connection (연결생성) 
3. Statement (문장실행)
4. ResultSet (결과집합사용)
👉 긴 자바코드를 제거하고 편리하게 쓰기 위해 [[Mybatis]]를 사용한다

# 5. 왜 쓰는가
- 각 DBMS들의 api를 하나로 통합하여 편리하게 사용하기 위함