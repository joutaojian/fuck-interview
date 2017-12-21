# 知识要点

1.java共有50个关键字，其中两个保留字(不是53个，其中三个是标识符)

2.访问修饰符(关键字)：public, protected, private

3.面向对象(关键字)：class, implements, extends, new, **interface**, **abstract**

4.修饰对象(关键字)：static, **final**, super, this, native, strictfp, synchronized, transient, volatile

5.final修饰的类不能被继承，没有子类

6.顶层类只能用public和default修饰



# 面试要点

- [x] ### interface和abstract的区别


两者都不是实体是一种抽象，根据名字翻译：interface是接口类，abstract是抽象类。

相同点：

* interface类的方法和abstract类的abstract方法**必须被实现**
* 都**不能实例化**


不同点：

* 具体实现不同：interface类是implements，abstract类是extends
* 设计理念不同：interface类表示的是“like-a”关系，abstract类表示的是“is-a”关系


------



- [x] ### Java中4种访问修饰符

如果一个类、类属变量及方法没有用任何修饰符（即没有用public、protected及private中任何一种修饰），则其访问权限为**default/friendly（默认访问权限）**,但是并**不存在default/friendly这样的关键字**。

| **访问级别** |     访问控制修饰符      |  同类  |  同包  |  子类  | 不同的包 |
| :------: | :--------------: | :--: | :--: | :--: | :--: |
|    公开    |      public      |  √   |  √   |  √   |  √   |
|   受保护    |    protected     |  √   |  √   |  √   |  --  |
|    默认    | default、friendly |  √   |  √   |  --  |  --  |
|    私有    |     private      |  √   |  --  |  --  |  --  |

* protected修饰符所修饰的类（这句话中指父类）属成员变量和方法，只可以被子类访问，而不管子类是不是和父类位于同一个包中。
* default修饰符所修饰的类属成员变量和方法，只可被同一个包中的其他类访问，而不管其他类是不是该类的子类。
* protected属于子类限制修饰符，而default属于包限制修饰符。


------



- [x] ### 继承与组合的区别

占坑

------



# 资料

[java中“53”个关键字（含2个保留字）](http://blog.csdn.net/u012506661/article/details/52756452)

[java中的访问修饰符](https://www.cnblogs.com/tjudzj/p/4443066.html)

[Java 中4种访问修饰符 public/protected/default(friendly)/private](http://blog.csdn.net/mingjie1212/article/details/50539188)

[抽象类abstract和接口interface的区别与深入思考](http://blog.csdn.net/wujiaxian/article/details/39991395)

[继承与组合的区别](http://blog.csdn.net/gvinaxu/article/details/51731202)

[详解继承与组合的优缺点](http://blog.csdn.net/calllmq/article/details/7399824)