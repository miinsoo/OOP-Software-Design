### 1. 각 클래스로 생성된 개체는 무슨 역활과 책임을 맡을지 설명한다.
* #### Animal  
    Animal 객체의 속성(id, 이름, 종)을 정의, Animal 객체 간의 동등성 재정의.

* #### AnimalCollection  
    Animal 리스트를 저장. 리스트에 Animal 객체를 추가, 삭제, 탐색 기능을 가짐.
* #### Application  
    프로그램의 인터페이스와 작동 프로시저를 정의
* #### Species  
    Species 객체의 속성(값)을 정의, Species 객체 간의 동등성 재정의

### 2. 개체의 상태와 동작은 다른 개체와 어떻게 상호작용하는지 설명한다.
* #### AnimalCollection  
    Animal 객체를 저장
* #### Application  
    사용자의 입력에 따라 AnimalCollection의 동작을 이용
* #### Species  
    Animal 객체가 Species 객체를 가짐

Species -> Animal -> Application -> AnimalCollection

### 3. 개체의 캡슐화가 어떻게 이뤄져 있는지 설명할 수 있어야 한다.
* 필드를 private로 선언, public 속성은 읽기 전용(read-only)
* Animal, Species는 Immutable로 선언해서 다른 클래스에서 함부로 변경하지 못하게 함