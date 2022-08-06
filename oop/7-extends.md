# 상속 (Extends)

코드의 중복을 방지하기 위해서 상속을 사용하지만 일반적인 경우에서의 상속은 캡슐화를 침해하고 코드의 재사용성을 오히려 떨어뜨립니다. 서브 클레스가 `super`를 통해서 슈퍼클래스를 호출하는 코드를 작성한다면 그 시점에서 슈퍼클래스와 서브클래스가 강하게 결합됩니다.

추가적으로 슈퍼클래스가 수정되면 높은 확률로 해당 슈퍼클래스를 상속받은 서브클래스의 내부 구현도 수정되어야하기 때문에 결합도가 떨어집니다.

**코드 중복을 회피하기 위해서 상속 대신 사용하는 방법**

- 두 메서드가 유사할 경우 차이점을 따로 메서드로 추출해야한다. 
- 슈퍼 클래스의 코드를 하위로 내리지말고 자식 클래스의 코드를 상위로 올려라  