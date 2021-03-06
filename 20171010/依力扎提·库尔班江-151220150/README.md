# 面向对象编程
依力扎提 151220150
## 面向对象机制
- **继承机制**  
    充分利用extends关键字达到继承基类的效果，这样的好处在于在定义数据类型时可以定义较为抽象的类型，在真正创建时才需要创建具体的类型，且子类可以替代父类，这样有利于代码的重用和多态。  
例如：
```
graph TD
    B[CucurbitBrothers] -->A[Creatures]
    C[Louluo] -->A
    D[Leaders] -->A
    E[CheeringCharactor] -->A
```
- **接口的使用**   
    interface的使用为面向对象中的类提供了对外的接口，实现了接口与实现分离，符合SOLID原则。  
## 设计理念
- **SOLID原则**  
    **单一职责原则**  
当需要修改某个类的时候原因有且只有一个（THERE SHOULD NEVER BE MORE THAN ONE REASON FOR A CLASS TO CHANGE）。换句话说就是让一个类只做一种类型责任，当这个类需要承当其他类型的责任的时候，就需要分解这个类。
``` 
        这样可能会带来类粒度太细的问题，故还要结合实际进行
```  
***
**开放封闭原则**  
软件实体应该是可扩展，而不可修改的。也就是说，对扩展是开放的，而对修改是封闭的。  
***
**里氏替换原则**
当一个子类的实例应该能够替换任何其父类的实例时，它们之间才具有is-A关系 
***
**依赖倒置原则**
1. 高层模块不应该依赖于低层模块，二者都应该依赖于抽象 
2. 抽象不应该依赖于细节，细节应该依赖于抽象
***
**接口分离原则**
不能强迫用户去依赖那些他们不使用的接口。换句话说，使用多个专门的接口比使用单一的总接口总要好。
***