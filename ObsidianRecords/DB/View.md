#Database #면접질문 
# 1.정의
- 읽기 전용으로 필요한 값을 뽑아서 조회하는 가상테이블

# 2.장점
- 복잡한 쿼리문의 경우 이미 만들어져있으므로 뷰를 읽어오기만 하면 데이터를 확인할 수 있다

# 3.단점
- 뷰를 수정해야 할 경우 뷰 생성문 자체를 수정해야한다
- DBMS내부에 작성되어있으므로 동적쿼리진행이나 동적인 값을 심기 어려울 수 있다.
- insert, update, delete는 개별테이블에서 진행해야 한다

# 4.사용하는 이유
- 변동사항이 없을경우 기본적인 가상테이블이 생성되어있으면 편리하다.
- **여러 테이블에서 데이터를 추출하거나 조인할 때 편리하게 사용할 수 있다. **
- 특히 필요한 데이터의 *부분 집합*을 만들어내는 데 유용하다.