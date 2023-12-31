#Database #면접질문 
# 1.정의
- 자바에서 클래스 안에 하나의 특성을 정의 하듯이, 테이블도 하나의 특성을 행/열을 사용하여 특정 엔티티나 개념을정리해 놓은 것.👉데이터 모델링이 가능해짐
- 이때 중복되는 값이 있으면 [[정규화]]를 통해 나눠 놓고 사용한다
- 테이블의 각 행은 키라는 고유 ID, 테이블의 열에는 데이터의 속성이 들어 있다.
- 각 레코드에는 일반적으로 각 속성에 대한 값이 있으므로 데이터 포인트 간의 관계를 쉽게 설정 가능.

### 데이터 모델링
- 개-논-물
- 주어진 개념으로부터 논리적인 데이터 모델을 구성하는 작업
- 이를 물리적인 데이터베이스 모델로 환원하여 고객의 요구에 따라 특정 정보 시스템의 데이터베이스에 반영하는 작업을 칭한다

# 2.장점
- 정렬된 형태로 다량의 데이터를 조회할 수 있다
- 참조키를 이용하여 테이블간 관계를 설정가능. [[식별관계]]
- 중복된 데이터를 허용하지 않으므로 무결성 보장
- 쿼리를 통해 데이터를 정확하게 검색하고 필요 정보를 추출가능

### 데이터 무결성
- 데이터의 *정확성과 일관성* 유지& 보증
- 데이터베이스, RDBMS 시스템의 중요한 기능

# 3.단점
- 테이블끼리 중복값을 가질 경우 정규화를 통해 나눠주는 작업이 필요하다.
- 단, 정규화를 통해 데이터의 속성을 알아보기 어려워질 수 있으므로 적당한 비정규화가 필요할때도 있다. (속성을 알아보기 쉽게하고 조회성능을 향상시킴)

# 4.사용 이유
- **데이터를 구조화하고, 일관된 형식으로 저장하며, 효과적으로 관리하기 위함.** 
- 관계형 데이터베이스([[RDBMS]])의 핵심 요소로서 데이터베이스 시스템의 핵심