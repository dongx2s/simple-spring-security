关于spring secuirty配置里的建造者模式
有两个重要的基本接口：
(1)SecurityBuilder，提供了一个build方法
(2)SecurityConfigurer，提供了对SecurityBuilder的两项操作：init和configure

先来讨论SecurityConfigurer，它有两个直接抽象子类SecurityConfigurerAdapter，GlobalAuthenticationConfigurerAdapter
和一个直接子接口WebSecurityConfigurer
WebSecurityConfigurer是用户配置spring security的入口
