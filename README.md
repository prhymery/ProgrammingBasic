# ProgrammingBasic

## 객체 지향 프로그래밍(Object Oriented Programming)
## 절차 지향 프로그래밍

## 객체 지향 프로그래밍의 특징
- 추상화(Abstraction)
- 캡슐화(Encapsulation)
  - 객체의 속성(data fields)과 행위(methods)를 하나로 묶음
  - 실제 구현 내용 일부를 내부에 감추어 은닉
- 상속성(Inheritance)
  - 하나의 클래스가 가진 특징(함수 ,데이터)을 다른 클래스가 그대로 물려 받는 것
- 다형성(Polymorphism)
  - 하나의 객체가 여러가지 타입을 가질 수 있는 것
  - 오버로딩(Overloading)
    - 같은 이름의 함수를 여러 개 정의한 후 매개 변수를 다르게 하여 같은 이름을 경우에 따라 호출하여 사용하는 것
  - 오버라이딩(Overriding)
    - 부모클래스의 메소드와 같은 이름을 사용하며 매개변수도 같되 내부 소스를 재정의하는 것
- 동적바인딩(Dynamic Binding)  
  - 함수를 호출하면 동적 바인딩을 통해 파생클래스에 오버라이딩 된 함수가 실행

## 자료구조 상속 구조
## 자료구조
- Set
  - 데이터를 비순차적(unordered)으로 저장할 수 잇는 순열 자료구조(collection)이다
  - 순서가 없다
  - 중복을 혀용하지 않아서 같은 값이 삽입되면 마지막에 삽입한 값 하나만 저장된다
  - 수정이 가능하다
  - 특정갑시 있는지 빠르게 확인하기에 좋다
- Vector
  - ArrayList 와 동일하게 사용가능
- Map
  - key 와 Value 로 나누어서 데이터를 관리한다
  - 순서가 없다
  - key 중복이 불가하다
  - 검색 속도가 빠르다
- List

### Managed Language
- Managed Language
  - 메모리 관리르 언어상에서 알아서 해주는 언어
- Unmanaged Language
  - 하드웨어와 좀 더 가까운 언어로 사용자가 직접적으로 하드웨어 CPU, Memory 를 관리할 수 있다

## Serialize / Deserialize
- 직렬화
  - 개체를 저장하거나 메모리, 데이터베이스, 파일로 전송하기 위해 개체를 바이트 스트림으로 변환하는 프로세스
  - 메모리에 저장되어 있는 추상적인 객체를 물리적으로 네트워크 통신으로 전송 및 디스크에 저장하기 위한 형식으로 변환하는 과정
- 역직렬화는 디스크에 저장한 데이터를 읽거나, 네트워크 통신으로 받은 데이터를 메모리에 쓸 수 있도록 다시 변환하는 과정
- 반대로 텍스트 파일을 오브젝트로 변환하는 것이 역직렬화
- 직렬화 하는 이유
  - 필요할 때 다시 개체로 만들 수 있도록 개체의 상태를 저장하는 것
  - 디스크에 저장하거나 네트워크 통신으로 전송하는 데 참조 타입 데이터는 가능하지 않고 값 타입 데이터만 가능하다
    - 프로세스가 정상적으로 종료될 때 프로세스 내에서 할당된 모든 메모리는 해제되고 프로그램이 새로 실행될 때마다 데이터를 할당하는 메모리 주소가 다르기 때문에 이전에 가지고 있던 주소 값으로는 기존의 데이터를 찾을 수 없다
    - 각 PC 마다 사용하고 있는 메모리 공간 주소가 전혀 다르기 때문)
  - 직렬화 된 데이터들은 언어에 따라서 텍스트 또는 바이너리 형태가 되는데, 이러한 형태가 되었을 때 저장하거나 통신시 파싱이 가능한 유의미한 데이터가 됨
  - string 이 포인터로 구현되어있는 경우, 내부적으로 메모리가 연속적으로 할당 되어있지 않기 때문에 이 메모리 데이터를 직렬화(연속적으로 배치 및 값 타입으로 변조)하는 것이 필요하다

## 값 타입(Value Type) / 참조 타입(Reference Type)
- 값 타입
  - 스택에 메모리가 쌓이고 직접 전근이 가능(int, float, char 등)
- 참조 타입
  - 힙에 메모리가 할당되고 스택에는 이 힙 메모리를 참조하는(힙에 메모리 번지 주소를 가지고 있는) 구조로 되어 있음(Object, 포인터)

## 용어정리
- API()
  - 
- 프레임워크(Framework)
  - 특정 프로그램을 개발하기 위한 여러 요소들과 메뉴얼인 룰을 제공하는 프로그램
  - 소프트웨어 개발에 있어 하나의 뼈대 역할을 함
- 라이브러리(Library)
  - API 를 기반으로 대상 환경(플랫폼)에서 바로 실행될 수 있도록 모듈화된 프로그램 모음
  - 다른 프로그램들과 링크되기 위하여 존재하는 하나 이상의 서브루틴이나 function 들이 저장된 파일들의 모음
  - 링크될 수 있도록 보통 컴파일된 형태(object module)로 존재한다
  - 라이브러리는 코드 재사용을 위해 조직화된 초창기 방법 중 하나이며, 다른 프로그램들이 사용할 수 있도록 운영체제나 소프트웨어 개발 환경 제공자 들에 의해 제공되는 경우가 많다
- 표준 템플릿 라이브러리(STL, Standard Template Library)
  - C++ 을 위한 라이브러리로 알고리즘, 컨테이너, 함수자, 반복자 4가지의 구성요소를 제공한다
    - 컨테이너
      - 데이터를 저장하는 객체들
    - 알고리즘
    - 반복자
    - 함수자
- 매개변수(Parameter) vs 전달인자(Argument)
  - 매개변수(Parameter) - 메서드 선언에서 나열되는 변수 명
  - 전달인자(Argument) - 메서드가 호출할 때 전달하는 실제 값
  ```C#
  int Sum(int A, int B) // 매개변수 A, B
  {
    return A + B;
  }

  Sum(1,2); // 전달인자 1, 2
  ```
- text editor
  - ???
- 컴파일
  - ???
- 컴파일러(Compiler)
  - 고수준 언어로 기술된 프로그램을 기계어 또는 어셈블리 언어 등의 저수준 언어로 번역하는 소프트웨어
  - 일반적으로 구문 해석과 기계어 코드를 발생시킼는 두 부분으로 이루어진다
- 링크
  - ???
  - 





# 3D Graphics
## vertex
- 3D 공간에서의 점
## Edge
- 버텍스 한쌍 사이를 연결한 것
## Polygon
- 3개 이상의 버텍스가 모여서 폴리곤을 형성

## Mesh
- 폴리곤이 모여서 만드렁진 3차원 공간 상의 객체(object)
## Triangle
- 버텍스 3개를 나타냄
## UV
