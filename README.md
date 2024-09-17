# 프로그램 소개
## 1. 구현 사항
  - 이 채팅 프로그램은 UDP와 TCP를 지원하는 서버/클라이언트를 포함하며, 비동기 소켓 입출력 모델을 사용하여 다자간 채팅 기능과 그림판 기능을 수행한다.
  - 멀티캐스트를 이용해 다자간 채팅 기능을 구현하였으며, 사용자는 자신의 ID를 설정 후 서버에 가입할 수 있고, 그룹에 가입한 후 그룹 탈퇴 기능, 서버 접속 끊기 기능을 통해 자유롭게 소통을 중단할 수 있다.
  - 사용자는 그룹에 가입하여 채팅 및 그림을 실시간으로 전송하고 그룹에 가입되어 있던 사용자는 실시간으로 전송받으며 소통이 가능하다.
  - 또한 사용자는 그룹에 가입 후 보내길 원하는 특정 그룹에만 채팅 및 그림을 전송할 수 있다. 그림판에는 여러 도형 및 색 지정, 선 굵기 조절 등 다양한 그리기 도구를 추가하여 다채로운 표현이 가능하므로 사용자들 간의 이해도가 높아진다.
  - 채팅 내역 삭제 기능을 통해 현재 사용자 자신의 채팅 로그를 삭제할 수 있는 기능을 제공한다. 서버는 브로드 캐스트를 이용해 접속되어 있는 클라이언트에게 공지사항을 전송할 수 있고, 사용자 추방 기능을 통해 사용자 관리가 쉬워진다.

## 2. 주요 기능 설명
  - Select 소켓 입출력 모델을 지원한다.
  - 블로킹 소켓을 사용한다.
  - 고정길이 전송방식을 사용한다.
  - 클라이언트가 보낸 데이터를 해석하지 않는다.
  - AsyncSelect 소켓 입출력 모델을 지원한다.
  - 넌블로킹 소켓을 사용한다.
  - 고정길이 + 가변길이 전송방식을 사용한다.
  - 비트연산을 이용하여 채팅방을 구현한다.
  - 접속한 클라이언트들에게 공지사항을 전달한다.
  - 사용자 목록을 확인 가능하고, 특정 사용자를 추방시킬 수 있다.
