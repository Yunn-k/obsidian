#Dao 
# 1.정의
- MyBatis is a first class persistence framework with support for custom SQL,stored procedures and advanced mappings.
- 사용자 정의 SQL, 저장프로시저, 고급매핑 및 영구적인 *데이터 저장과 사용을 도와주는 프레임워크*
- 객체지향언어인 java와 SQL based인 관계형 데이터베이스(RDBMS) 사이에서 데이터를 다루는 방식의 괴리를 해결하기위해 만들어진 *persistance frmework*의 일종.

# 2.장점
- MyBatis eliminates almost all of the JDBC code and manual setting of parameters and retrieval of results. 
- MyBatis can use simple XML or Annotations for configuration and map primitives, Map interfaces and Java POJOs (Plain Old Java Objects) to database records.
- JDBC에 있는 대부분의 *자바코드 삭제*.
- *mapping*을 위해 단순한 xml파일이나 어노테이션만 설정해주면 된다.
- 데이터베이스 레코드에 매핑하기 위해 map 인터페이스들과 *순수 자바코드(POJO)만 있으면 된다.*
- 간단한 sql문만 가지고도 데이터를 가져올 수 있다.
![[Pasted image 20231121175515.png]]
# 3.단점



# 4.왜 쓰는가?
- *인터페이스와 Mapper.xml을 매핑함으로써 간단하게 sql문을 구현하고 필요한 데이터를 마련할 수 있음.
