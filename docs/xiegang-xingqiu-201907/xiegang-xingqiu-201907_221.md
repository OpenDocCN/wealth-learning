# 20 个 Spring

# 20 个 Spring

小猿 : 20 个 Spring 面试问答(上篇) 1、什么是 Spring 框 架？Spring 框架有哪些主要模块？ Spring 框架是一个为 Java 应 用程序的开发提供了综合、广泛的基础性支持的 Java 平台。 Spring 帮助开发者解决了开发中基础性的问题，使得开发人员 可以专注于应用程序的开发。 Spring 框架本身亦是按照设计 模式精心打造，这使得我们可以在开发环境中安心的集成 Spring 框架，不必担心 Spring 是如何在后台进行工作的。 Spring 框架至今已集成了 20 多个模块。这些模块主要被分如下 图所示的核心容器、数据访问/集成,、Web、AOP（面向切面 编程）、工具、消息和测试模块。 2、使用 Spring 框架能带来 哪些好处？ 下面列举了一些使用 Spring 框架带来的主要好 处： Dependency Injection(DI) 方法使得构造器和 JavaBean properties 文件中的依赖关系一目了然。 与 EJB 容器相比 较，IoC 容器更加趋向于轻量级。这样一来 IoC 容器在有限的 内存和 CPU 资源的情况下进行应用程序的开发和发布就变得 十分有利。 Spring 并没有闭门造车，Spring 利用了已有的技术 比如 ORM 框架、logging 框架、J2EE、Quartz 和 JDK Timer，以 及其他视图技术。 Spring 框架是按照模块的形式来组织的。 由包和类的编号就可以看出其所属的模块，开发者仅仅需要 选用他们需要的模块即可。 要测试一项用 Spring 开发的应用 程序十分简单，因为测试相关的环境代码都已经囊括在框架 中了。更加简单的是，利用 JavaBean 形式的 POJO 类，可以很 方便的利用依赖注入来写入测试数据。 Spring 的 Web 框架亦是 一个精心设计的 Web MVC 框架，为开发者们在 web 框架的选 择上提供了一个除了主流框架比如 Struts、过度设计的、不流 行 web 框架的以外的有力选项。 Spring 提供了一个便捷的事务 管理接口，适用于小型的本地事物处理（比如在单 DB 的环境 下）和复杂的共同事物处理（比如利用 JTA 的复杂 DB 环 境）。 3、什么是控制反转(IOC)？什么是依赖注入？ 控制反

转是应用于软件工程领域中的，在运行时被装配器对象来绑 定耦合对象的一种编程技巧，对象之间耦合关系在编译时通 常是未知的。在传统的编程方式中，业务逻辑的流程是由应 用程序中的早已被设定好关联关系的对象来决定的。 在使用 控制反转的情况下，业务逻辑的流程是由对象关系图来决定 的，该对象关系图由装配器负责实例化，这种实现方式还可 以将对象之间的关联关系的定义抽象化。而绑定的过程是通 过“依赖注入”实现的。 控制反转是一种以给予应用程序中目 标组件更多控制为目的设计范式，并在我们的实际工作中起 到了有效的作用。 依赖注入是在编译阶段尚未知所需的功能 是来自哪个的类的情况下，将其他对象所依赖的功能对象实 例化的模式。这就需要一种机制用来激活相应的组件以提供 特定的功能，所以依赖注入是控制反转的基础。否则如果在 组件不受框架控制的情况下，框架又怎么知道要创建哪个组 件？ 在 Java 中依然注入有以下三种实现方式： 1.构造器注入 2.Setter 方法注入 3.接口注入 4、请解释下 Spring 框架中的 IoC？ Spring 中的 org.springframework.beans 包

和 org.springframework.context 包构成了 Spring 框架 IoC 容器的基 础。 BeanFactory 接口提供了一个先进的配置机制，使得任何 类型的对象的配置成为可能。ApplicationContex 接口对 BeanFactory（是一个子接口）进行了扩展，在 BeanFactory 的 基础上添加了其他功能，比如与 Spring 的 AOP 更容易集成，也 提供了处理 message resource 的机制（用于国际化）、事件传 播以及应用层的特别配置，比如针对 Web 应用的 WebApplicationContext。 org.springframework.beans.factory.BeanFactory 是 Spring IoC 容器 的具体实现，用来包装和管理前面提到的各种 bean。 BeanFactory 接口是 Spring IoC 容器的核心接口。 5、 BeanFactory 和 ApplicationContext 有什么区别？ BeanFactory 可 以理解为含有 bean 集合的工厂类。BeanFactory 包含了种 bean 的定义，以便在接收到客户端请求时将对应的 bean 实例化。 BeanFactory 还能在实例化对象的时生成协作类之间的关系。

此举将 bean 自身与 bean 客户端的配置中解放出来。BeanFactory 还包含了 bean 生命周期的控制，调用客户端的初始化方法

（initialization methods）和销毁方法（destruction methods）。 从表面上看，application context 如同 bean factory 一样具有 bean 定义、bean 关联关系的设置，根据请求分发 bean 的功能。但 application context 在此基础上还提供了其他的功能。 1.提供了 支持国际化的文本消息 2.统一的资源文件读取方式 3.已在监 听器中注册的 bean 的事件 以下是三种较常见

的 ApplicationContext 实现方式： 1、 ClassPathXmlApplicationContext：从 classpath 的 XML 配置文件 中读取上下文，并生成上下文定义。应用程序上下文从程序 环境变量中取得。 ApplicationContext context = new ClassPathXmlApplicationContext(“bean.xml”); 2、 FileSystemXmlApplicationContext ：由文件系统中的 XML 配置 文件读取上下文。 ApplicationContext context = new FileSystemXmlApplicationContext(“bean.xml”); 3、 XmlWebApplicationContext：由 Web 应用的 XML 文件读取上下 文。 6、Spring 有几种配置方式？ 将 Spring 配置到应用开发中 有以下三种方式： 1.基于 XML 的配置 2.基于注解的配置 3.基 于 Java 的配置 7、如何用基于 Java 配置的方式配置 Spring？ Spring 对 Java 配置的支持是由@Configuration 注解和@Bean 注解 来实现的。由@Bean 注解的方法将会实例化、配置和初始化 一个新对象，这个对象将由 Spring 的 IoC 容器来管理。@Bean 声明所起到的作用与 元素类似。被@Configuration 所注解的类 则表示这个类的主要目的是作为 bean 定义的资源。被

@Configuration 声明的类可以通过在同一个类的内部调用

@bean 方法来设置嵌入 bean 的依赖关系。 8、请解释 Spring Bean 的生命周期？ Spring Bean 的生命周期简单易懂。在一个 bean 实例被初始化时，需要执行一系列的初始化操作以达到 可用的状态。同样的，当一个 bean 不在被调用时需要进行相 关的析构操作，并从 bean 容器中移除。 Spring bean factory 负 责管理在 spring 容器中被创建的 bean 的生命周期。Bean 的生命

周期由两组回调（call back）方法组成。 1.初始化之后调用的 回调方法。 2.销毁之前调用的回调方法。 Spring 框架提供了 以下四种方式来管理 bean 的生命周期事件： InitializingBean 和 DisposableBean 回调接口 针对特殊行为的其他 Aware 接口 Bean 配置文件中的 Custom init()方法和 destroy()方法 @PostConstruct 和@PreDestroy 注解方式 9、Spring Bean 的作用域之间有什么 区别？ Spring 容器中的 bean 可以分为 5 个范围。所有范围的名 称都是自说明的，但是为了避免混淆，还是让我们来解释一 下： 1.singleton：这种 bean 范围是默认的，这种范围确保不管 接受到多少个请求，每个容器中只有一个 bean 的实例，单例 的模式由 bean factory 自身来维护。 2.prototype：原形范围与单 例范围相反，为每一个 bean 请求提供一个实例。 3.request：在 请求 bean 范围内会每一个来自客户端的网络请求创建一个实 例，在请求完成以后，bean 会失效并被垃圾回收器回收。 4.Session：与请求范围类似，确保每个 session 中有一个 bean 的 实例，在 session 过期后，bean 会随之失效。 5.global-session： global-session 和 Portlet 应用相关。当你的应用部署在 Portlet 容器 中工作时，它包含很多 portlet。如果你想要声明让所有的 portlet 共用全局的存储变量的话，那么这全局变量需要存储在 global-session 中。 全局作用域与 Servlet 中的 session 作用域效果 相同。 10、Spring 框架中的单例 Beans 是线程安全的么？ Spring 框架并没有对单例 bean 进行任何多线程的封装处理。关 于单例 bean 的线程安全和并发问题需要开发者自行去搞定。 但实际上，大部分的 Spring bean 并没有可变的状态(比如 Serview 类和 DAO 类)，所以在某种程度上说 Spring 的单例 bean 是线程安全的。如果你的 bean 有多种状态的话（比如 View Model 对象），就需要自行保证线程安全。 最浅显的解决办 法就是将多态 bean 的作用域由“singleton”变更为“prototype” 未 完待续 。。。

2018-04-01

评论区：

小猿 : 先起个面试分享带头，大家手头有类似资源，欢迎分享出来，代表星球所有人感激你！[抱拳][抱拳][抱拳]