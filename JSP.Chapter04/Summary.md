## 1. 스크립트 태그

## 1.1 JSP 문법의 기분

#### 태그의 이용

JSP는 태그를 이용하여 고유한 문법을 기술하는 서버 프로그래밍 방식.

JSP의 태그 방식은 
- 스크립트 태그
- 액션 태그
- 커스텀 태그

로 나뉜다.

#### JSP 스크립트 태그 종류
- 지시어 <%@    %> JSP 페이지의 속성을 지정
- 선언 <%! %> 소속변수 선언과 메소드 정의
- 표현식 <%=  %> 변수, 계산식, 함수 호출 결과를 문자열 형태로 출력
- 스크립트릿 <%   %> 자바 코드를 기술
- 주석  <%-- --%> JSP 페이지의 설명 추가

#### 액션 태그

XML 스타일의 태그로 기술한 동작 기능을 수행하는 방식

- <jsp: include page="test.jst"/>  현재 JSP 페이지에서 다른 페이지 포함
- <jsp: forward page="test.jst"/>   현재 JSP 페이지의 제어를 다른 페이지에 전달
- <jsp: plugin type="applet" code="test"/>  자바 애플릿을 플러그인
- <jsp: useBean id = "login" class="LoginBean" />   자바빈을 사용
- <jsp:setProperty name="login" property="pass" />  자바빈의 속성을 지정하는 메소드를 호출
- <jsp:getProperty name="login" property="pass" />  자바빈의 속성을 반환하는 메소드를 호출

#### 커스텀 태그

새로운 태그를 정의하여 이용하는 방법

- <tag:printData dbname="mydb" table="memb" /> 사용자가 직접 정의한 태그를 이용
