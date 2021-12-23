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

## 브라우저 렌더링 원리 (출처: <https://d2.naver.com/helloworld/59361>)

* 브라우저의 주요 기능

  브라우저의 주요 기능은 사용자가 선택한 자원을 서버에 요청하고 브라우저에 표시하는 것 이다. 자원은 보통 HTML 문서지만 PDF나 이미지 도는 다른 형태일 수 있다.  
  자원의 주소는 URI(Uniform Resource Identifier)에 의해 정해진다.  
  
  브라우저는 HTML과 CSS 명세에 따라 HTML 파일을 해석해서 표시하는데 이 명세는 웹 표준화 기구인 W3C (World Wide Web Constortium)에서 정한다.

  브라우저의 UI는 다음과 같은 요소들이 일반적이다.  
  * URI를 입력할 수 있는 주소 표시줄
  * 이전 버튼과 다음 버튼
  * 북마크
  * 새로고침 버튼과 현재 문서의 로드를 중단할 수 있는 정지 버튼
  * 홈 버튼  
  
* 브라우저의 구조  

  1. 사용자 인터페이스 - 위에 말한 UI 요소들을 보여주는 창을 제외한 나머지 모든 부분
  2. 브라우저 엔진 - 사용자 인터페이스와 렌더링 엔진 사이의 동작을 제어
  3. 렌더링 엔진 - 요청한 콘텐츠를 표시, 예를 들어 HTML을 요청하면 HTML과 CSS를 파싱하여 화면에 표시함
  4. 통신 - HTTP 요청과 같은 네트워크 호출에 사용됨. 이것은 플랫폼 독립적인 인터페이스이고 각 플랫폼 하부에서 실행 됨
  5. UI 백엔드 - 콤보 박스와 창 같은 기본적인 장치를 그림, 플랫폼에서 명시하지 않은 일반적인 인터페이스로서, OS 사용자 인터페이스 체계를 사용
  6. 자바스크립트 해석기 - 자바스크립트 코드를 해석하고 실행
  7. 자료 저장소 - 이 부분은 자료를 저장하는 계층이다. 쿠키를 저장하는 것과 같이 모든 종류의 자원을 하드 디스크에 저장할 필요가 있다.  
  
* 렌더링 엔진들  
  파이어폭스는 모질라에서 직접 만든 게코(Gecko) 엔진을 사용하고, 사파리와 크롬은 웹킷(Webkit) 엔진을 사용한다.
  
* 동작 과정  
  렌더링 엔진은 통신으로부터 요청한 문서의 내용을 얻는 것으로 시작한다.  
  다음은 렌더링 엔진의 기본적인 동작 과정이다.  
![렌더링 과정](/Images/2.png)

**기술면접**

```
렌더링 엔진은 HTML 문서를 파싱하고 "콘텐츠 트리" 내부에서 태그를 DOM 노드로 변환한다.
그 다음 CSS 파일과 함께 포함된 스타일 요소도 파싱한다. (스타일 정보와 HTML 표시 규칙은 '렌더 트리'라고 부르는 또 다른 트리를 생성한다.)
렌더 트리 생성이 끝나면 배치가 시작된다.
```

![동작 과정](/Images/3.png)
<code><pre>
사용자에게 브라우저가 보이는 과정  
1.브라우저가 서버로 URI를 통해 HTML문서를 요청한다.
2.서버에서 HTML 문서를 받으면 렌더링엔진이 DOM 트리를 구축하기 위해 HTML을 파싱한다.
3.DOM 트리를 통해 렌더트리를 구축한다.
4.렌더트리를 위치를 배치한 뒤 그린다.
</pre></code>
