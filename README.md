# Ruby on Rails 학습
- 개인적인 궁금증으로 시작한 실습입니다. ruby에 대한 간단한 문법에 대해 학습하고, 인프런 강의를 따라 간단한 웹페이지를 만드는 것을 목표로 학습하였습니다.
- 구름IDE를 사용하여 학습할 예정(Cloud9 IDE 사용x)

## RUBY
### 데이터의 종류
1. 숫자, 문자열, 배열, 해시
2. 없다는 의미는 nil로 사용함.
3. 배열에는 서로 다른 여러가지의 데이터 종류가 들어갈 수 있음
4. 배열로 할당된 공간보다 더 큰 값을 참조할 때는 nil을 반환
5. 해시 = 키를 값에 매핑할 수 있는 자료구조 {키 => 요소}

### 변수와 상수
- 변수 선언 (ex -> hi = "hello", x = 2) 위와 같이 선언함
- 변수형 선언이 없어도 됨
- 지역변수 전역변수 인스턴스 변수 클래스 변수 네 개로 나뉨
	- 지역변수 : foo = 'foo in top level'
	- 전역변수 : $foo = 'foo in whole'
	- 인스턴스변수 : @foo = 'foo in instance'
	- 클래스변수 : @@foo = 'foo in class'

### 제어구조
- if ~ elseif ~ else end : 만약 ~~라면
- unless else end : 만약 ~~가 아니라면
- for 변수 in 범위 end : 변수에 범위 값이 담겨서 사용 가능
	- for x in 0 .. 10 puts x end 이런 식으로 사용
	- 0 .. 2 의 경우 0 1 2가 출력 0 ... 2 의 경우 0 1 출력
- for 변수 in 배열 end : 변수에 배열의 원소값이 담겨서 사용

### method
- def 이름(매개변수) 
 내용
 return 반환
 end
 
 ## Rails 웹 프레임워크
 - MVC모델 (Spring과 같음)
 
 ### 기본구조
 1. tcp 연결
 - M(model : 데이터베이스의 정보를 가져오는 등 데이터를 다룸)VC패턴
 2. routes.rb => C(controller) => M(model) => C => V(view) 
 