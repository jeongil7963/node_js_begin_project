# Node.js 프로그래밍 기초

### 노드로 만들 수 있는 대표적인 서버와 용도

-   서버는 왜 필요할까?

        API란 프로그램을 쉽게 제작할 수 있게 미리 만들어 놓은 것들의 모음이다.
        다른 곳에 있는 단말에 데이터를 달라고 요청하는 프로그램을 클라이언트라고 한다.
        다른 곳에서 요청받은 명령을 처리해 주는 프로그램을 서버라고 한다.
        프로토콜이란 데이터를 서로 어떤 형태로 주고받을 것인지를 정한 것으로 간단하게 데이터의 형태라고 생각하면 된다.


-   대표적인 서버 유형은 어떤 것이 있을까?

        채팅 서버
        위치 기반 서비스 서버
        모바일 서버
        JSON-PRC 서버
        웹 서버

-   웹 서버의 기능은 무엇일까?

        웹 문서 조회
        파일 업로드, 다운로드
        로그인, 회원가입

-   채팅 서버의 중요한 기능은 무엇일까?

        친구 목록 보여주기
        일대일 채팅하기
        그룹 채팅하기

-   JSON-RPC 서버의 중요한 기능은 무엇일까?

        서버 쪽에 함수를 만들어 두고 클라이언트에서 함수를 호출하듯이 데이터를 요청하면 응답하는 서버이다.
        JSON은 어떤 형식으로 데이터를 주고 받을지를 정해 노은 표준 데이터 포맷이다.
        RPC 방식으로 데이터를 주고 받는다.
        데이터를 요청하고 응답을 받아 처리하는 데 에이잭스 방식이 아닌 JSON-RPC를 사용하기도 한다.
        > 웹에서 데이터 요청
        > 앱에서 데이터 요청

-   위치 기반 서비스 서버의 중요한 기능은 무엇일까?

        데이터 요청
        가까운 위치 찾기
        영역 내의 위치 찾기

-   모바일 서버의 중요한 기능은 무엇일까

        모바일 웹으로 사이트 열기
        단말 정보관리하기
        공지 메시지 받기

### 노드에 대해 알아보고 개발 도구 설치하기

-   노드란 무엇일까?

        노드는 자바스크립트를 이용해서 서버를 만들 수 있는 개발 도구입니다.
        하나의 요청 처리가 끝날 때까지 기다리지 않고 다른 요청을 동시에 처리할 수 있는 비동기 입출력 방식을 적용했다.
        프로그램에서 해당 파일의 내용을 처리할 수 있는 시점이 되면 콜백함수가 호출된다.
        먼저 메이인이 되는 자바스크립트의 파일의 일부 코드를 떼어 별도의 파일로 만들 수 있는데 이것을 모듈이라고 부른다.

        > 다음과 같은 특징을 갖느다.
        > 모듈과 패키지
        > 비동기 입출력
        > 이벤트 기반 입출력

-   개발 도구 설치하기

        브라켓 설치
        크롬 브라우저 설치
        노드 설치

### 노드 간단하게 살펴보기

- 첫 번재 노드 프로젝트 만들기

        자바스크립트 파일 만들어 실행하기
        브라켓의 확장 기능 설치하고 브라켓에서 노드 프로그램 실행하기
        노드 셸에서 직접 코드 입력하고 실행하기

- 콘솔에 로그 뿌리기

        콘솔 객체는 전역 객체라고 부르며 필요할 때 코드의 어느 부분에서나 사용할 수 있다.
        > console : 콘솔창에서 결과를 보여주는 객체
        > process : 프로세스의 실행에 대한 정보를 다루는 객체
        > exports : 모듈을 다루는 객체

- 프로세스 객체 간단하게 살펴보기

        argv : 프로세스를 실행할 때 전달되는 파라미터 정보
        env : 환경 변수 정보
        exit() : 프로세스를 끝내는 메소드

- 노드에서 모듈 사용하기

        export에는 속성을 추가할 수 있어 여러개의 변수나 함수를 각각의 속성으로추가할 수 있다.
        module.exports는 하나의 변수나 함수 또는 객체를 직접 할당한다.
        다른 사람이 만들어 둔 모듈을 외장 모듈이라고 한다.

- 간단한 내장 모듈 사용하기

        미리 포함되어 있는 모듈을 내장 모듈이라고하며, 개발자가 직접 만들어 올린 모듈을 외장 모듈이라고 한다.
        외장 모듈은 npm으로 설치해야 하지만 내장 모듈은 바로 사용할 수 있다.
        > os 모듈
        >> hostname / totalmem / freemem / cpus / networkinterfaces
        > path 모듈
        >> join / dirname / basename / extname
