# JSP 공부 내용 정리

## JSP 코드 표기법
| 표현식 | 문 | 설명 |
|------|---|---|
| <%@  %> | 지시문 | 페이지 속성 지정 |
| <%  %> | 스크립트릿 | 자바 코드 블록, 변수(지역) 선언가능 |
| <%!  %> | 선언문 | 전역변수 혹은 메소드 선언 |
| <%=  %> | 표현식 | 웹브라우저에 직접 결과 값을 출력 |
| <%-- --%> | 주석 | 실행에 관여하지않는 문자 | 
## Java API 패키지
| API | 패키지 |
|------|---|
| java.lang | 자바 프로그래밍 기본 기능 제공 (생략가능) | 
| java.util | 프로그램에 유용한 유틸리티
| java.io | 입출력에 관한 기능 제공 |
| java.sql | sql 관련 기능 | 
| java.time | 날짜와 시간 관련 기능 제공 |

# JSP 활용

## 지역변수와 전역변수 차이
### 코드 설명
#### ● 전역 변수는 어느 위치에서든 호출하면 사용이 가능 (함수 밖에 선언하여 클래스 전체에서 사용이 가능한 함수)
#### ● 특정구역({})내에서 생서오디어 그 구역에서만 사용 (함수 속에 선언되어 해당 함수 속에서만 사용이 가능한 변수)


### 출력화면 / 코드부분
![변수차이](https://user-images.githubusercontent.com/93521099/170395359-620d058d-c126-4c3a-b29d-a68cd8981f27.PNG) <br>
### 첫 번째 실행 / 두 번째 실행
![첫실행](https://user-images.githubusercontent.com/93521099/170395363-0be4edae-6c85-4e32-8370-603b6e3beaed.PNG) ![두번째실행](https://user-images.githubusercontent.com/93521099/170395365-3e424ae5-6df8-4ac1-826e-068156710f95.PNG)

## 전역변수 선언문, 지역변수와 연산식 사용
### 출력화면 / 코드부분
![덧셈뺄셈](https://user-images.githubusercontent.com/93521099/170396136-b0dfaae2-98c8-47bf-ab7d-dfe330bb0623.PNG) <br>
### 덧셈 실행  / 뺄셈 실행
![덧셈](https://user-images.githubusercontent.com/93521099/170396147-afc76327-3218-4c34-8b71-bbadc8977519.PNG) ![뺄셈](https://user-images.githubusercontent.com/93521099/170396142-5d2d8038-b9cf-47ef-a7f8-abaacc5b3868.PNG) 

## if ~ else 문 사용
### 출력화면 / 코드부분
![코드](https://user-images.githubusercontent.com/93521099/170401519-b0d2df2b-41be-46e2-852c-2359fda43723.PNG) <br>
### 값이 맞았을 경우 / 틀렸을 경우
![로그인 확인](https://user-images.githubusercontent.com/93521099/170401534-c3289398-46f2-44c0-8725-8465c39480bd.PNG) ![틀림](https://user-images.githubusercontent.com/93521099/170401538-c4075583-e85f-4d92-94e1-ba54716a0a36.PNG)



## 1차원 배열 사용
### 출력화면 / 코드부분
![1차원 배열](https://user-images.githubusercontent.com/93521099/170396982-a7e0030a-d645-480d-82ac-3940c5221cd8.PNG) <br>
![1차원 출력](https://user-images.githubusercontent.com/93521099/170396985-b732b1a5-f42a-4e33-96d1-3c310d109ff8.PNG)

## 2차원 배열 사용
### 코드 설명 (성적처리)
#### ● jumsu에 있는 값을 이중 for문을 이용하여 total배열에 첫 번째 인덱스와 두 번째 인덱스에 더한 값을 넣어줌.
#### ● average배열에 total배열에 있는 값을 이용해 평균을 구함.
#### ● 이중 for문을 이용하여 각 원소의 값을 출력
### 출력화면 / 코드부분
![2차원 배열 for문](https://user-images.githubusercontent.com/93521099/170397062-083492e8-5503-4062-8837-c794579a6c8a.PNG) <br>
![배열출력](https://user-images.githubusercontent.com/93521099/170397066-f78a8484-c260-4d19-a98d-3f4cbab4f420.PNG)

## 클래스 사용
### 코드 설명 (계좌 출금 / 입금)
#### ● balance(잔액)에 deposit(입금) 매소드를 이용하여 돈을 넣어줌.
#### ● balance(잔액)에 payment(출금) 매소드를 이용하여 돈을 뺌.
#### ● balance(잔액)이 출금하려는 값보다 적으면 '잔액부족'이라는 메세지를 출력
### 출력화면 / 코드부분
![클래스](https://user-images.githubusercontent.com/93521099/170397534-afe947b0-58d1-4644-a883-42158c6228dc.PNG) <br>
### 출금 화면 / 잔액 부족 화면
![클래스화면](https://user-images.githubusercontent.com/93521099/170397549-bfb822d9-203f-454c-8431-4a7ce6859322.PNG) ![잔액부족](https://user-images.githubusercontent.com/93521099/170397556-72c5ec6a-f53b-4e70-b6b3-1405b7e48833.PNG)
