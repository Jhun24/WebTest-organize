# 언어

- JavaScript


	- 1995년 넷스케이프 개발

	- Netscape Navigator 2.0 브라우저에 최초 탑재

	- 웹프로그래밍 개념 창시

- 특징


	HTML 문서에 내장

	스크립트 언어 (컴파일 필요없음)

	단순하다


- 역할


	동적 제어

	입력 & 계산

	브라우저 제어

	서버 통신

	어플리케이션 제작


- 작성 위치


	HTML 내장 이벤트 리스터 속성 (onclick이벤트 함수 같은거)

	<script> 태그

	.js 파일

	URL에 작성


- 작성 방법


	head 태그 안에 (head태그에 쓰면 html class랑 id 못불러옴)

	body  태그 안에

	html 태그 안이면 사실 어따 넣어도 상관없음 ㅎ 오류는 책임 안짐 ㅎ

	script태그에서 <script src ="js/index.js"></script> 이런식으로 넘

# 코드 작성

> document.write()는 알겠지


- 경고창 


	alert("hello") = 경고창에 hello라는 말을 띄움

	var data = prompt("hello","") = data라는 변수에 prompt로 입력된 값을 저장
	
	var data = dialog("") = yes , no 버튼 있음

# 식별자

- 규칙

	첫글자에는 알파벳 , 언더바( _ ) , 달러($) 이거만 쓸수있음

	두번째 글자부터는 숫자도 쓸수있음

# 변수

- 데이터 타입

	숫자 타입 : 1 2 3 이런거

	논리 타입 : true , false

	문자열 타입 : "abcd" 이런거

	객체 레퍼런스 타입 : var d = new Date(); 이런거

	null : 말그대로 null

- 선언

> Example Code

	var name = "이장훈"

	gender = "남자" : 이런식으로도 되는데 IDE에서 오류 ㅈㄴ 뿜으니까 쓰지말자

> 걍 var만 쓰면됨 개꿀 ㅎㅎ

# 상수

> 선언해서 쓰는 상수는 ES6부터 지원함 ^^

- 문자열 상수

	문자열안에 문자열

# 배열

- 선언

	var arr = new Array();

	var arr = ["1" , "2" , "3"];

- 특징

	처음에 배열 사이즈 설정 안해두됨

	나머지는 c랑 똑같음

# 함수

- 정의
	
	데이터를 받아 처리후 값을 돌려주는 코드

> 걍 그 초딩때 배웠던 값넣으면 다른 값나오는 상자라 생각하삼

- 구성

> Example Code

	function 함수 이름(인자값){
		함수 코드
	}
> 함수 구조

	함수이름();
> 호출방식

- 전역 함수

> Example Code : eval()

	eval("1+2+3") = 6
> 함수안에 있는 식을 계산후 결과 리턴

> Example Code : parseInt()

	parseInt("16") = 16
> 문자열을 10진수로 변환

> Example Code : parseInt(a,b)

	parseInt("A",16) = 10
> 문자열을 b진수로 해석수 10진수 변환

> Example Code : parseFloat()

	parseFloat("1.2") = 1.2
> 문자열을 실수로 변환

> Example Code : isFinite()

	isFinite("16") = true

	isFinite(16) = true

	isFinite("a") = false
> 함수의 인자값이 숫자인지 체크

> Example Code : isNaN()

	isNaN("16") = false

	isNaN(16) = false

	isNaN("a") = true
> 함수의 인자값이 숫자가 아닌지 체크


# 객체


- 정의


	고유한 구성 속성(기능)을 가지고있음


- 종류


> 코어 객체

	언제 어디서나 사용 가능

	표준 객체


- Example


	var arr = new Array();
	var date = new Date();
	var math = new Math();


> DOM 객체


	html 속성 , 태그들을 제어 


> Example 


	document.getElementById()
	document.write()


> 브라우저 객체


	브라우저 제어


> Example


	history : 뒤로가기 그런거

	alert() , prompt() , dialog()

	cookie제어도 가능


- 구조


- proprety(프로퍼티)


	객체의 고유한 값 (멤버 변수)


> Example Code


	var user = {
		name : "이장훈"
	};
	console.log(user.name)


- method(메소드)


	객체의 고유한 함수 (멤버 함수)


> Example Code


	var d = new Date();

	d.getHours();


- 생성 방법


	var testObject = new Object();
	testObject.name = "이장훈" : property(멤버 변수) 생성

	testObject.printName = function(){
		console.log(this.name); 
	} : method(멤버 함수) 생성


- String 객체


	예는 독특해서 설명해줌


> Example


	var objectText = new String("hello");
	var normalText = "hello"
	objectText.length // o
	normalText.length // o
	// 어떤걸로 생성하던 String 객체 method 사용가능
	normalText[0] == h
	// []이거 사용해서 접근가능 개꿀 ㅎㅎ


> 예제들은 느그들이 알아서하자

> Date객체 종류랑 Math객체 종류는 대충보고가삼 

> Date 객체 : http://findfun.tistory.com/464

> Math 객체 : http://findfun.tistory.com/457

> String 객체는 내면 좀 더러운데 낼라나

# 연산자

> 비트 연산자랑 시프트 연산은 프밍에서 했을테니까 패스

> 논리연산도 알지? (&& = and , || = or , ! = not)

> 증감 연산자 (a++ , ++a , a-- , --a) 알꺼고

- String 연산자

> Example Code

	var a = "123";
	var b = "45";

	var c = 123;
	var d = 45

	a + b = "12345"
	a + c = "123123"
	c + d = 168

> 그니까 정수덧셈 빼고는 다 문자열처럼 더해짐 ㅇㅋ?

- 비교연산

> (> , < , >= , <= , != , ==) 이거는 프밍에서 했으니까 다알거고

> 다 똑같은데 다른게 하나있음

> Example Code

	var a = "1"
	var b = 1;

	console.log(a == b)

> true

	console.log(a === b)

> false

> JS는 변수가 var밖에 없어서 형(type)까지 체크할려면 === 써야됨 (== 쓰면 int랑 string이랑 같다고 함 개꿀 ㅎㅎ)

- 대입 연산

> 걍 노답임

> 비트 연산 부분은 참고 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Expressions_and_Operators
