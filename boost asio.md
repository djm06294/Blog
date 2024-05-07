# Boost Asio? 개념 잡기

1. socket, endpoint?
**socket이란** 통신의 극점(**endpoint**)을 뜻한다고 한다. 두개의 process가 서로 소통을 하기 위해서는 각 process가 두개씩의 socket을 가지고 있어야 한다. client process가 연결을 요청한다면 host(server) process에서 port번호를 부여한다.
**endpoint**란 ip주소와 port번호의 조합을 의미한다고 생각할 수 있다. 모든 TCP 연결은 2개의 endpoint로 유일하게 식별되어질 수 있다. 

https://3dmpengines.tistory.com/1904

2. resolver?

3. Asio?
Async IO의 줄임말이다. Async란 asynchronous의 앞글자로 비동기적이라는 뜻이다. 비동기 방식으로 소켓 통신을 구현할 때, 리눅스에서는 EPOLL을 사용하고 윈도우에서는 IOCP를 사용한다고 한다. 

https://mutpp.tistory.com/entry/Boost-Asio%EC%97%90-%EB%8C%80%ED%95%B4%EC%84%9C-%EC%95%8C%EC%95%84%EB%B3%B4%EC%9E%90

4. callback함수
asio에서는 socket과 endpoint를 정의한 후에 async_connect() 함수를 통해 비동기 연결 및 callback 함수를 설정할 수 있다. 그런데 나는 이 callback 함수가 main process와 동시에 이루어지는 것인지가 궁금했다. 
