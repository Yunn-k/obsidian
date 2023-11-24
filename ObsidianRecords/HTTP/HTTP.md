#Http 

# 1.정의
- hyper text transfer protocol
- hyper text == 링크가 가능한 메세지 (참조를 통해 다른 문서로 접근 가능)
- 서버와 클라이언트 사이에서 어떻게 메세지를 전송할지 정해 놓은 약속

# 2. 웹페이지 렌더링 과정
1. 도메인을 쳐서 접속시 네트워크는 IP주소를 찾으러 DNS(Domain name system)로 감
2. 알맞는 IP주소를 반환받음
3. 해당 서버로 가서 필요한 데이터를 순서대로 받음 (html, css, js)
4. 렌더링시 css는 dom생성을 방해하지 않으나, html은 css 생성을 기다리므로 css 파일이 큰건 좋지 않다
5. js파일이 있다면 dom생성을 멈추고 js를 읽게 되므로 defer, sync옵션을 사용해서 dom 생성을 멈추게 하지 않도록 한다.혹은 js파일을 맨 아래에 두거나!

![[Pasted image 20231123174833.png]]
- 리소스요청 > 토큰화 > 노드 생성 > DOM tree