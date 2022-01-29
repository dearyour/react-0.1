# 자기주도 프로젝트 플랜/정리 템플릿 🐣
자기주도 프로젝트 명세서를 참고하여 학습 및 과제를 진행하고 배운 내용을 정리하기 위한 템플릿

## 작성자

- 김용희




## 구현 기능

| 기능 분류 | 기능 설명                        | 구현 여부 |
| --------- | -------------------------------- | --------- |
| `필수1`    | 2학기 git 실습      | ✅         |
| `필수2`    | ERD작성실습        | ✅         |
| `필수3`    | create React            | ✅         |
| `필수4`    | 테스트케이스 만들어보기                | ✅         |
| `필수6`    | 알고리즘에 순서도와 의사코드(pseudo-code) 작성    | ✅         |
| `선택1`    | web에서 Rendering 기술 차이 | ✅         |
| `선택4`    | 자바스크립트에서 Firebase 활용하기   | ✅         |
| `선택18`    | node.js와 socket.io를 활용한 채팅 server/client 구현      | ✅         |



# 필수1 2학기 git 실습

쇼핑몰   
-회원가입 , 로그인 ,마이페이지 , 상품등록 , 판매 , 결제모듈, 찜하기, 리뷰 , 상품검색

```
1. 메인 페이지
2. 제품페이지 
3. 제품상세정보 , 리뷰 , 1:1 문의  
4. 마이페이지, 장바구니 
5. 1:1 문의
6. 검색
```
```
1. 메인페이지 - 할인 상품 보여주기
상단에 검색기능, 로그인 회원가입 버튼 
로그인하면 마이페이지,로그아웃 보여주기
좌측에 남자 겉옷,상의,바지,신발,세일 메뉴
여자 겉옷,상의,바지,치마,신발,세일 메뉴

2. 제품 페이지 -  최신등록순서 또는 가격대로 나열   
3. 제품상세정보 -  가격 , 사이즈 , 원단 표기 
	       구매하기와 장바구니 버튼
     밑단에 리뷰, Qna 란

3. 마이페이지 -  구매내역, 반품, 교환 , 
	개인정보 변경 - 비밀번호변경 , 휴대전화, 이메일,  주소지 변경 

4.장바구니 -  제품 결제하기 , 상품수량 늘리기 , 제품 삭제하기  
```

```
1. 메인페이지 
-회원가입 
결제는 회원가입을 해야만 사이트를 이용할수있다
회원가입 아이디는 4글자~ 16글자 (한글 2글자~8글자)로 제한한다.
회원가입시 주소,휴대폰,아이디,비밀번호는 필수로 작성되어야 가능하다
회원가입시 중복된 아이디는 가입할수 없다 
휴대폰을 통한 본인 인증이 되어야만 가입 할 수있다.
Email을통한 ID찾기 pw변경이 가능하다  

-로그인
아이디를 4글자~16글자 이상 작성해야 한다 
로그인과 비밀번호가 기존의 DB에 등록된것과 일치했을때 로그인 성공을하며 
성공시 상단 멘위 마이페이지와 로그아웃이 나타난다.
페이지를 이동해도 로그인상태를 유지한다 . 

-검색
해당 제품명의 일부분만 검색해도 검색되어야 한다.

2. 제품페이지
-등록순서 
최신등록순서를 누르면 등록된 순서를 기준으로 가장최근순서대로 보여준다.
가격대로 나열일 경우 가장 비싼 가격을 최신순서대로 나열하고
다시한번 가격대로를 누르면 가장 싼 가격을 최신순서대로 나열한다.
제품사진아래에 가격이 표기되며 할인된 상품인경우 기존의 가격 숫자 가운데 줄을긋고
할인된 가격을 표기하며 그옆에는 할인된금액을 표기한다
3. 제품 상세정보
제품정보 -
제품사진 오른쪽에 원단과 가격이 표기되며 
할인된 상품인경우 가격 숫자에 가운데줄을 긋고 할인된 금액이 나오며
아래에 할인된 기간을 작성한다 
그 아래에 구매할것인지 장바구니로 보낼것인지 선택한다.

-리뷰 
리뷰에 추천 버튼을 작성해
다른 사용자가 그 리뷰를보고 유용했다면 추천을 누를수있다
월말마다 해당 제품의 리뷰 사진에 1등이 된 사용자에게 적립금을 부여한다. 
-Q&A 
비공개 글을 쓸것인지 공개글을 쓸것인지 선택한다
비공개 글을 쓸경우 관리자만 확인할수 있다.

3.마이페이지 
구매내역을 눌렀을경우 해당 아이디로 구매한 상품내역이 위에서 아래로 최신순서대로 나온다
반품을 눌렀을경우 반품 주소지를 작성후 택배비 차감한 금액에 대한 동의란이 나오고
반품확인을 눌렀을경우 관리자가 확인할수있다.
교환일 경우는 위에서 추가적으로 교환할 사이즈를 작성후 교환확인을 누른다
회원정보 수정 을 할경우 핸드폰번호,주소지,비밀번호를 수정할 수있다.

4. 장바구니에서 상품수량을 늘릴경우 만약 상품의 갯수에 한계가 있다면
상품수량한계를 초과했다는 창과함께 그 이상의 상품수량으로 선택할수 없게된다. 
상품을 삭제하기가 가능하고 상품결제하기를 누르면 결제하기창으로 넘어간다 
import 결제모듈을 사용해서 카드 결제를 하던지 무통장입금으로 결제하기를 한다.

5. 1:1 문의 - 자신이 1:1문의한 내용만 리스트로 보이고 관리자가 답글을 남기면
	    답변완료라는 글이 제목에 보인다.
```

![wire](https://user-images.githubusercontent.com/52556956/147501100-854cecaa-ab48-42f2-ba77-13e1f732b302.png)





# 필수2 ERD작성실습
![ERD다이어그램](https://user-images.githubusercontent.com/52556956/147501283-ad7fcfc3-09ed-4284-9b4b-be4bb2b2ab64.JPG)


# 필수3 create React

### 1. create


![createee](https://user-images.githubusercontent.com/52556956/147504591-da38ad79-d1cd-4776-bd80-cb8c365d070d.JPG)

___
___
___
___

### 2. list

![list](https://user-images.githubusercontent.com/52556956/147504184-6e440e7f-b4f4-48c9-8b86-b6684bf6da05.JPG)
___

### 2.1 list
![분류](https://user-images.githubusercontent.com/52556956/147504161-e5b4d979-933d-49c2-a792-27e2f7b0f00b.JPG)
___
___
___
___

### 3. view

![view](https://user-images.githubusercontent.com/52556956/147504159-075a3a42-7e17-4581-85ac-91729e8a2a7d.JPG)

___
___
___
___
### 4. update

![업데이트](https://user-images.githubusercontent.com/52556956/147504166-06926948-cdbe-441a-be89-92580cbe213a.JPG)
___
___
___
___
### 5. delete

![delete](https://user-images.githubusercontent.com/52556956/147504176-07b9d423-e1ad-461c-a42d-bcfe683d2aab.JPG)
___
![delete2](https://user-images.githubusercontent.com/52556956/147504179-5016d42e-e825-448c-882e-dc0b56e870e6.JPG)
___
___
___
___

# 필수4 테스트케이스 만들어보기 

- 테스트 대상 

![테스트케이스로그인](https://user-images.githubusercontent.com/52556956/147501384-d1274ac6-fb4b-46eb-b0f3-ca1ccf759efe.JPG)

- 제어 흐름도 

![제어흐름도](https://user-images.githubusercontent.com/52556956/147522884-68f4d7ff-0d8e-4e9b-8c9f-b8b31974bd7f.JPG)

- 최종 케이스

![테스트케이스](https://user-images.githubusercontent.com/52556956/147501409-48b960c0-e6cb-41f9-925c-80c627a83188.JPG)

# 필수6 알고리즘에 순서도와 의사코드(pseudo-code) 작성 
```
알고리즘 디자인설계
0. 회원가입 기능이 필요하다.
1. 외부로부터 필요한 데이터값 아이디,비밀번호,이메일,주소 4개를 입력받는다
 1-1 전송방식은 post로 json 타입으로 전해받는다
2. (1)에 데이터 값은 검증 조건이 필요하다
 2-1 아이디는 기존에 있는 아이디와 중복이 불가능하다
 2-2 아이디와 비밀번호는 자릿수가 4자리 이상 12자리 이하여야 한다
 2-3 비밀번호에는 숫자 1개 이상 포함되어야한다
 2-4 비밀번호에는 특수문자중에 1개 이상이 포함되어야한다
 2-5 상기 조건중에 하나라도 해당되지 않으면 에러 (E101)을 리턴 한다
3. (2)에 의해 아이디 중복을 찾기위해 회원테이블을 조회한다
4. 조회된 아이디가 있으면 에러(E102)를 리턴한다.
5. 조회된 아이디가 없으면 해당 정보를 json타입으로 회원테이블에 전달한다
6. 회원가입이 완료가 되면 로그인 페이지로 이동한다 . 
```

- pseudo-code

```
function 문자열의 특수문자를 포함 여부를 검사한다
input 문자열
output 참 또는 거짓

function 문자열의 숫자 포함 여부를 알려준다.
input 문자열
output 참 또는 거짓

start 회원가입 폼
set 외부에서 받아온 데이터값 아이디
set 외부에서 받아온 데이터값 비밀번호
set 외부에서 받아온 데이터값 이메일
set 외부에서 받아온 데이터값 주소
if( 아이디는 특수문자가 포함 안됨
 	and 아이디는 4자리 이상 12자릿수 이하
	and 비밀번호는 4자리 이상 12자릿수 이하
	and 비밀번호에는 숫자가 1개 이상
	and 비밀번호에는 특수문자중에 1개 이상 포함)
else 
	return 에러메시지 E101
set 아이디로 회원정보 테이블을 조회한 객체 
if (해당 아이디를 가진 회원정보 객체 존재하지 않는다면)
else
	return 에러메시지 E102 
return 회원가입 성공  메시지 M100
end 로그인창 으로 이동 
```

- flowchart

![flowchart](https://user-images.githubusercontent.com/52556956/147501512-efd59963-6058-4de3-bdf2-9e196cd61e47.JPG)

# 선택1 web에서 Rendering 기술 차이

-MPA SSR view 바뀔때 패킷생성

![MPA SSR view 바뀔때 패킷생성](https://user-images.githubusercontent.com/52556956/147502838-de362958-70ad-4040-99fc-99da0d1b4086.JPG)

-SPA CSR 최초접속시 js및 static file 다운

![SPA CSR 최초접속시 js및 static file 다운](https://user-images.githubusercontent.com/52556956/147502843-2b9355b2-cd9b-4f93-af11-11bcaa5fc6ed.JPG)

-MPA일때 패킷이 캡처된다

![MPA일때 패킷이 캡처된다](https://user-images.githubusercontent.com/52556956/147502845-7d60922f-c4cf-42a2-b876-7c354823bcd9.JPG)

- csr 단점 
1. 서버에 껍데기만 있는 index.html 을 보내는데 body에는 id root와 app.js 어플리케이션에 필요한 자바스크립트만 보낸다 
2. 처음에 화면을 띄울때 클라이언트는 비어있고 서버에서 app.js 를 받아오기 때문에 느릴 수 있다. 

- csr 장점

1. app.js 를 받아오는 순간 부터 바로 동적으로 사이트가 반응이 가능함 

___ 

- ssr 장점

1. 서버에서 완성된 index.html을 받아오기 때문에 첫번째 페이지 로딩이 빠르다. 

- ssr 단점

1. 매 페이지마다 새로운 html을 받아야하기 때문에 페이지 전환은 csr보다 느리다 

2. index.html을 먼저 받아온 후 동적으로 제어할수있는 js 파일은 받아오기 때문에 js를 아직 못받았을 경우 클릭을해도 반응이 없을 수 있음

___

# 선택4 자바스크립트에서 Firebase 활용하기 

![파이어1](https://user-images.githubusercontent.com/52556956/147502982-fc72b8e5-5e51-48a2-a330-eab722b58131.JPG)

![파이어2](https://user-images.githubusercontent.com/52556956/147502986-22dbd326-a96d-43a3-9634-18080b87e53e.JPG)

![파이어3](https://user-images.githubusercontent.com/52556956/147502989-b0870751-017a-4f83-9c63-d7581f29a9d4.JPG)

![파이어4 1](https://user-images.githubusercontent.com/52556956/147503347-9207f357-773b-4b09-9a70-532a20e78d36.JPG)

![파이어4 2](https://user-images.githubusercontent.com/52556956/147503351-8d73ba08-4d71-400c-ba07-fa4af05de03b.JPG)

- 배포전 빌드를 해준다 

- 그 이유는 동영상,사진을 압축하듯 띄어쓰기,공백을 제거한 파일로 배포를 완료해서 용량을 줄이기 위함

![파이어5](https://user-images.githubusercontent.com/52556956/147503368-c147a08d-84a9-4b16-af6b-1b59860cd991.JPG)


![파이어4](https://user-images.githubusercontent.com/52556956/147502990-834f9987-0e01-469d-af10-78360cf182db.JPG)

# [배포 완료](https://kyh-review.web.app/)

# 선택18 node.js와 socket.io를 활용한 채팅 server/client 구현
개요

## 단방향 통신
![단방향](https://user-images.githubusercontent.com/52556956/147512183-46294ecc-aa6a-461e-ad41-afa2302f9719.JPG)
- 서버는 데이터를 그룹지어서 관련된것을 URL로 클라이언트에게 제공한다  
-클라이언트는 서버에서제공하는 URL중에서 REST API(단방향통신) 는 클라이언트의 요청이 있어야지만 
서버에서 응답을 해서 데이터를 받아옵니다
- REST API는 한번의 요청이 한번의 응답으로 끝남

## 양방향 통신
![양방향](https://user-images.githubusercontent.com/52556956/147512180-04ca5918-78b3-40b9-9977-b6829431507b.JPG)
- socket.io
- 클라이언트와 서버에 데이터를 전송할수있는 채널을 형성후
- 클라이언트의 요청이없이도 서버쪽에서 그 채널로 클라이언트에게 데이터를 제공

![소켓io 작동흐름](https://user-images.githubusercontent.com/52556956/147511199-a527a1d1-10b2-4464-a4a7-8c2ed68e682b.JPG)

1. 웹페이지 접속 
2. 클라이언트 var socket = io();
3. 서버와 연결관계를 맺음
4. 서버에 이벤트로 emit
5. 전체 클라이언트에 메시지 전달 



##
![1socketio설치](https://user-images.githubusercontent.com/52556956/147509986-626d0942-2a79-4324-b1ad-4bb473a96b65.JPG)


## server.js (서버구동)
```js
const app = require('./app.js');
const port = 3000;

const server = app.listen( port, function(){
    console.log('Express listening on port', port);
});

const listen = require('socket.io');  
const io = listen(server);        // localhost:3000에 소켓서버가 붙는다
                                  // 즉 소켓서버를 우리쪽 웹서버에 붙인다 

 io.on('connection', (socket) => {   //접속을 하는순간 소켓을 사용
      socket.on('client message', (data) => {  // 클라이언트에서 emit한 이벤트명과 일치시켜야함, data = message:message.val()
          io.emit('server message', data.message);  // io는 접속한 사용자의 글로벌 변수 
      });
  });
```


## chat.html (사용자)
```js
</style>
<script src="/socket.io/socket.io.js"></script>   // 웹서버에 소켓서버를 붙인후 socket.io 모듈 제공가능
<script>
var socket = io();

socket.on('server message', function(data){
    $('#chatBody').append('<li>' + data + '</li>');
});

$(document).ready(function() {
    $('#sendForm').submit(function(){        // 메시지를 보냈을때
        var message = $('#sendForm input[name=message]');  //메시지값을 저장
        socket.emit('client message', { message : message.val()});   // 소켓가져와서 전송, 이벤트명 , 변수명 : 값
        message.val('');
        return false;
    });
});
</script>
```

## chat에 socket.io 모듈을 가져온다 
```js
<script src="/socket.io/socket.io.js"></script>  
<script>
var socket = io();
```
## server.js에서  socket.io 모듈을 가져와서 emit, 소켓서버로 보낸다

```js
io.on('connection', (socket)=>{  //접속을 하는순간 소켓을 사용
  console.log('소켓서버 접속');
})
``` 
## 소켓서버 접속을 확인한다 

![2 1소켓](https://user-images.githubusercontent.com/52556956/147510228-76dc4818-18a1-48d7-8229-4b4b9b7549f0.JPG)

## chat.html에서 메시지를 보내고 다시 메시지 빈 ''문자열로 만들어준다.
```js
$(document).ready(function()){
 $('#sendForm').submit(function(){        // 메시지를 보냈을때
        var message = $('#sendForm input[name=message]');  //메시지값을 저장
        socket.emit('client message', { message : message.val()});   // 소켓가져와서 전송, 이벤트명 , 변수명 : 값
        message.val('');
        return false;
    });
}
``` 
![3 1](https://user-images.githubusercontent.com/52556956/147510580-c54c02ce-c484-4c31-92c1-026ac9488bac.JPG)

## server.js에서 메시지를 받는다.

```js
io.on('connection', (socket) => {   //접속을 하는순간 소켓을 사용
      socket.on('client message', (data) => {  // 클라이언트에서 emit한 이벤트명과 일치시켜야함, data = message:message.val()
          io.emit('server message', data.message); // io는 접속한 사용자의 글로벌 변수 
      });
  });
```
- 받는쪽(on)의 이벤트명('client message')은 보내는쪽(emit)과 일치시켜줘야한다 

![3](https://user-images.githubusercontent.com/52556956/147510575-9a0fea66-585e-496d-b3d1-1d198edb5b1c.JPG)

## chat을 localhost가 아닌 다른서버면 io()부분에 보내고싶은 주소를 작성한다.
```js
var socket = io('https://www.asdf.com');
```

- socket.on(아이디) 를 지정하면 해당하는 사람에게만 보낸다.


## chat 받은 데이터를 상대에게 갱신한다.
```js
 io.emit('server message', data.message);


socket.on('server message', function(data){   //클라이언트에서 서버에서 온 메시지를 받는다
    $('#chatBody').append('<li>' + data + '</li>');  //클라이언트에서 받은 메시지 갱신 
});
```
![4소켓](https://user-images.githubusercontent.com/52556956/147510989-87776956-a000-44e0-a8ea-7737f75b08b7.JPG)


## 즉 emit으로 보내고 socket.on으로 받는다. 

| 사용자　-> | 서버　-> | 서버　-> | 사용자 | 
| --------- | -------------------------------- | --------- |--------- |
|emit | socket.on | emit | socket.on|
|client Message | client Message | server Message | server Message |




