# Computer Science

## OOP (Object-oriented programming)

### **객체 지향 프로그래밍**

OOP는 현실 세계를 프로그래밍으로 옮겨와 현실 세계의 사물들을 객체로 보고, 그 객체로부터 개발하고자 하는 특징과 기능을 뽑아와 프로그래밍하는 기법이다.

OOP로 코드를 작성하면 재사용성과 변형가능할 수 있습니다.

### **OOP의 5가지 설계 원칙**

* SRP(Single Responsibillity Principle, 단일 책임 원칙): 클래스는 단 하나의 목적을 가져야 하며, 클래스를 변경하는 이유는 단 하나의 이유여야 한다.
* OCP(Open-Closed Principle, 개방 폐쇄 원칙): 클래스는 확장에는 열려 있고, 변경에는 닫혀 있어야 한다.
* LSP(Liskov Substitution Principle, 리스코프 치환 원칙): 상위 타입의 객체를 하위 타입으로 바꾸어도 프로그램은 일관되게 동작해야 한다.
* ISP(Interface Segregation Principle, 인터페이스 분리 원칙): 클라이언트는 이용하지 않는 메소드에 의존하지 않도록 인터페이스를 분리해야 한다.
* DIP(Dependency Inversion Principle, 의존 역전 법칙): 클라이언트는 추상화(인터페이스)에 의존해야 하며, 구체화(구현된 클래스)에 의존해선 안된다.

### **절차지향 프로그래밍 / 객체지향 프로그래밍**

* 절차지향 프로그래밍
  * 물이 위에서 아래로 흐르는 것 처럼 순차적인 처리를 중요시하는 프로그래밍 기법이다.
  
  * 가장 대표적인 언어 - C

  * 컴퓨터의 처리구조와 유사해 실행속도가 빠르다.
  
  * 코드의 순서가 바뀌면 동일한 결과를 보장하기 힘들다.

* 객체지향 프로그래밍
  * 실제 세계의 사물들을 객체로 모델링하여 개발을 진행하는 프로그래밍 기법

  * 가장 대표적인 언어 - JAVA, C#

  * 캡슐화, 상속, 다형성 등과 같은 기법을 이용할 수 있다.

  * 절차지향 언어보다 실행속도가 느리다.

## 브라우저 렌더링 원리 

* 브라우저의 주요 기능

  브라우저의 주요 기능은 사용자가 선택한 자원을 서버에 요청하고 블아ㅜㅈ에 표시하는 것 이다. 자원은 보통 HTML 문서지만 PDF나 이미지 도는 다른 형태일 수 있다.  
  자원의 주소는 URI(Uniform Resource Identifier)에 의해 정해진다.   
  
  브라우저는 HTML과 CSS 명세에 따라 HTML 파일을 해석해서 표시하는데 이 명세는 웹 표준화 기구인 W3C (World Wide Web Constortium)에서 정한다.

  브라우저의 UI는 다음과 같은 요소들이 일반적이다.  
  * URI를 입력할 수 있는 주소 표시줄
  * 이전 버튼과 다음 버튼
  * 북마크
  * 새로고침 버튼과 현재 문서의 로드를 중단할 수 있는 정지 버튼
  * 홈 버튼
  

