#Java 

# 정의
- 객체간 (결합)관계
- 결합관계는 기본적으로 모두 **association**
https://ala-nueva.tistory.com/361

# Has a 상속
## 1.Composition has a
- 일체형
- A객체가 생성될때 B를 포함해서 생성하도록 되어있으므로 A를 생성하기만 하면 사용 가능
![[Pasted image 20231123120423.png]]
- 클래스가 생성될 때 생성자를 통해 객체가 생성된다
- ExamList list = new ExamList(); 와 위의 생성자는 동일. (원래 생성자를 사용해야하지만 자바문법이 나중에 한줄로 쓸 수 있도록 허용해주고 컴파일러가 생성자로 처리함)

## 2.Aggregation has a
- 조립형. setter자리만 마련해놓고 밖에서 객체를 만들어 꽂는다
- 객체를 집합적으로 갖는다

### 사용 이유
- 조립해야 한다는 불편함이 있지만 느슨한 결합력을 유지하여 유지보수가 쉽다
- 다른 객체로 교체하기 쉽다.
- 조립 역할을 스프링이 맡는다

# Dependency Injection
- 두 객체간의 관계를 맺어주는 것.

## 1.Setter Injection
![[Pasted image 20231123114606.png]]
## 2.Construction Injection
![[Pasted image 20231123114621.png]]

# Is a 상속 (Inheritance)
- 자식클래스가 부모클래스의 특징을 상속받아 커스터마이징 하는 것
- extends : 클래스상속, 인터페이스 확장 (implements는 클래스가 인터페이스를 구현할때)
- super: 상속관계에서 부모의 생성자, 속성, 메서드 호출시 사용
- override: 부모의 메서드를 자식에서 구현할때 쓰는 annotation


