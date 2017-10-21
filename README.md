# 언어

- JavaScript


	1995년 넷스케이프 개발
	Netscape Navigator 2.0 브라우저에 최초 탑재
	웹프로그래밍 개념 창시

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


	<head> 태그 안에 (head태그에 쓰면 html class랑 id 못불러옴)
	<body>  태그 안에
	<html> 태그 안이면 사실 어따 넣어도 상관없음 ㅎ 오류는 책임 안짐 ㅎ
	<script src ="js/index.js"></script> 이런식으로 넘


# 코드 작성

> document.write()는 알겠지


- 경고창 


	alert("hello") = 경고창에 hello라는 말을 띄움
	var data = prompt("hello","") = data라는 변수에 prompt로 입력된 값을 저장
	var data = dialog("") = yes , no 버튼 있음


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

