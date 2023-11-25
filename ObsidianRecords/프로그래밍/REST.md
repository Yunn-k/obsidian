# 정의
- representational state transfer
- representation 이란 리소스의 특정 시점의 상태를 반영하는 정보
- http를 통해서 속성을 통해 자원에 접근하는 방법론을 말하며, 이러한 형태로 구현된 메소드를 restful이라 한다
- 자원의 구분과 상태를 url을 통해 이해할 수 있다

# 원칙
1. 명시적으로 HTTP 메서드를 사용할 것.
2. 상태를 저장하지 말 것. (Be stateless)
3. 디렉토리 구조와 유사한 URI 를 사용할 것.
4. XML 혹은 JSON 혹은 두 가지 방법 모두를 사용하여 리소스를 전송할 것.

## URI와 URL의 차이
### URI
- Uniform resource identifier
- 통합 자원 식별자
- naver.com -- 식별자

### URL
- Uniform resource locator
- 웹에서 주어진 고유 리소스 주소
- http://naver.com -- 식별자+위치
 ![[Pasted image 20231125145820.png]]



