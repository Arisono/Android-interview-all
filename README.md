![](https://i.loli.net/2020/12/28/hWJbL4ptZUG7anF.png)

> <g-emoji class="g-emoji" alias="fire" fallback-src="https://www.yundashi168.com/154.html">🔥  原文地址：[https://www.yundashi168.com/154.html](https://www.yundashi168.com/154.html "https://www.yundashi168.com/154.html")  🔥
关注原文地址，可以获得最新最全的Android面试知识点更新情况，技术路上你不孤单。</g-emoji>

<g-emoji class="g-emoji">🔥</g-emoji> 个人归纳的中高级Android面试知识点全方面汇总+长期更新+QQ技术群交流(151909524)<g-emoji class="g-emoji">🔥</g-emoji>

# 基础篇

## Java基础

- [静态内部类和非静态内部类有什么区别](https://blog.csdn.net/angle_chen123/article/details/85598585 "静态内部类和非静态内部类有什么区别")
- [静态属性和静态方法是否可以被继承？是否可以被重写？以及原因？](https://blog.csdn.net/qdh186/article/details/79807057)
- [谈谈你对java多态的理解](https://blog.csdn.net/qq_41679818/article/details/90523285 "谈谈你对java多态的理解")+[java方法的多态性理解](https://www.cnblogs.com/liujinhong/p/6003144.html "java方法的多态性理解")
- [java中接口和继承的区别](https://www.cnblogs.com/smuxiaolei/p/9240871.html "java中接口和继承的区别")
- [抽象类和接口的区别（面试题）](https://blog.csdn.net/qq_41933748/article/details/82670072)


### Java集合

- ArrayList
- HashMap (重点)
- LinkedList
- ConcurrentHashMap (重点)
- LinkedHashMap (重点)
- BlockingQueue

ArrayList和LinkedList的区别

> Arraylist
底层是基于动态数组，根据下表随机访问数组元素的效率高，向数组尾部添加元素的效率高；但是，删除数组中的数据以及向数组中间添加数据效率低，因为需要移动数组。例如最坏的情况是删除第一个数组元素，则需要将第2至第n个数组元素各向前移动一位。而之所以称为动态数组，是因为Arraylist在数组元素超过其容量大，Arraylist可以进行扩容（针对JDK1.8? 数组扩容后的容量是扩容前的1.5倍）
> Linkedlist
基于链表的动态数组，数据添加删除效率高，只需要改变指针指向即可，但是访问数据的平均效率低，需要对链表进行遍历。基于链表的动态数组，数据添加删除效率高，只需要改变指针指向即可，但是访问数据的平均效率低，需要对链表进行遍历。



推荐阅读：

- [HashMap中的Hash冲突解决和扩容机制](https://russxia.com/2019/05/06/HashMap%E4%B8%AD%E7%9A%84Hash%E5%86%B2%E7%AA%81%E8%A7%A3%E5%86%B3%E5%92%8C%E6%89%A9%E5%AE%B9%E6%9C%BA%E5%88%B6/ "HashMap中的Hash冲突解决和扩容机制")
- [java1.8源码之ArrayList源码解读](https://blog.csdn.net/u010250240/article/details/89762912 "java1.8源码之ArrayList源码解读")
- [Map 综述（二）：彻头彻尾理解 LinkedHashMap](https://blog.csdn.net/justloveyou_/article/details/71713781 "Map 综述（二）：彻头彻尾理解 LinkedHashMap")
- [超详细LinkedHashMap解析](https://blog.csdn.net/qq_40050586/article/details/105851970 "超详细LinkedHashMap解析")
- [LinkedHashMap详解](https://blog.csdn.net/u012860938/article/details/95613684 "LinkedHashMap详解")
- [你重写过 hashcode 和 equals 么，为什么重写 equals 时必须重写 hashCode ⽅法？](https://blog.csdn.net/qq_41934688/article/details/113796637 "你重写过 hashcode 和 equals 么，为什么重写 equals 时必须重写 hashCode ⽅法？")
 [为什么重写equals()方法时，必须要求重写hashCode()方法？](https://blog.csdn.net/weixin_44259720/article/details/88414828 "为什么重写equals()方法时，必须要求重写hashCode()方法？")
- [ArrayList（int initialCapacity）会不会初始化数组大小？](https://blog.csdn.net/linmengmeng_1314/article/details/106940483 "ArrayList（int initialCapacity）会不会初始化数组大小？")
- **解释Java hashCode（）和equals（）方法**
equals（）方法用于确定两个Java对象的相等性。 当我们有一个自定义类时，我们需要重写equals（）方法并提供一个实现，以便它可以用来找到它的两个实例之间的相等性。 通过Java规范，equals（）和hashCode（）之间有一个契约。 它说，“如果两个对象相等，即obj1.equals（obj2）为true，那么obj1.hashCode（）和obj2.hashCode（）必须返回相同的整数”

  无论何时我们选择重写equals（），我们都必须重写hashCode（）方法。 hashCode（）用于计算位置存储区和key。
- [为什么 Hashtable 和 ConcurrentHashmap 键和值不能为null，而hashmap可以？](https://blog.csdn.net/sinat_40482939/article/details/108014484 "为什么 Hashtable 和 ConcurrentHashmap 键和值不能为null，而hashmap可以？")
- 解释下什么是快速失败(fail-fast机制)和安全失败

###  Java并发

- [JAVA线程间通信的几种方式](http://edisonxu.com/2017/03/02/java-thread-communication.html "JAVA线程间通信的几种方式") 讲解全面而且还有案例展示
- [Java线程间的通信](https://redspider.gitbook.io/concurrent/di-yi-pian-ji-chu-pian/5 "Java线程间的通信")
- [Java并发编程之线程篇之线程间通信(四)](https://juejin.cn/post/6844903919781412877#heading-12 "Java并发编程之线程篇之线程间通信(四)")
- [多线程任务调度(依赖+并发+串行)](https://gitee.com/jd-platform-opensource/asyncTool/blob/master/QuickStart.md "多线程任务调度(依赖+并发+串行)")
- [多线程并发执行任务，取结果归集。终极总结：Future、FutureTask、CompletionService、CompletableFuture](https://www.cnblogs.com/dennyzhangdd/p/7010972.html "多线程并发执行任务，取结果归集。终极总结：Future、FutureTask、CompletionService、CompletableFuture")
- [Java多线程与高并发(四):java.util.concurrent包](https://www.wangtianyi.top/blog/2018/05/01/javagao-bing-fa-xi-lie-si-juc/ "Java多线程与高并发(四):java.util.concurrent包")
- [java多线程设计模式 -- 流水线模式（Pipeline）](https://blog.csdn.net/huzhiqiangCSDN/article/details/56846268 "java多线程设计模式 -- 流水线模式（Pipeline）")
- [深入理解synchronized锁升级过程](https://blog.csdn.net/weixin_40910372/article/details/107726978 "深入理解synchronized锁升级过程")
- [线程池的好处](https://blog.csdn.net/fengye454545/article/details/79536986 "线程池的好处")+[线程池的优点及其原理](https://www.cnblogs.com/allenhhw/p/12101431.html "线程池的优点及其原理")+[线程池的优点](https://blog.csdn.net/hanghangaidoudou/article/details/81628166 "线程池的优点") (重点)
- [为什么不推荐通过Executors直接创建线程池](https://blog.csdn.net/xiaojin21cen/article/details/87269126 "为什么不推荐通过Executors直接创建线程池")
- [不怕难之BlockingQueue及其实现](https://www.jianshu.com/p/7b2f1fa616c6 "不怕难之BlockingQueue及其实现")
- [深入理解ReentrantLock与Condition](https://www.cnblogs.com/superfj/p/7543927.html "深入理解ReentrantLock与Condition")
- [Java多线程：线程间通信之Lock](https://www.cnblogs.com/cielosun/p/6662201.html "Java多线程：线程间通信之Lock")
- [Synchronized 关键字原理](https://blog.csdn.net/weixin_36759405/article/details/83034386 "Synchronized 关键字原理")
- [ReentrantLock原理](https://blog.csdn.net/fuyuwei2015/article/details/83719444 "ReentrantLock原理")
- [浅谈偏向锁、轻量级锁、重量级锁](https://www.jianshu.com/p/36eedeb3f912)

###  Java反射

> 反射是在运行状态中，对于任意一个类，都能够知道这个类的所有属性和方法；对于任意一个对象，都能够调用它的任意一个方法和属性；这种动态获取的信息以及动态调用对象的方法的功能称为 Java 语言的反射机制。

- [java反射原理-重要](https://blog.csdn.net/weixin_42724467/article/details/84311385)
- [什么是反射机制?反射机制的应用场景有哪些?](https://zhuanlan.zhihu.com/p/272002926)

###  Java泛型

###  Java虚拟机

- [深入理解Java对象的创建过程：类的初始化与实例化](https://blog.csdn.net/justloveyou_/article/details/72466416 "深入理解Java对象的创建过程：类的初始化与实例化")

####  JVM常见面试题

- [Java虚拟机(JVM)面试题（2020最新版）](https://blog.csdn.net/ThinkWon/article/details/104390752 "Java虚拟机(JVM)面试题（2020最新版）")
- [JVM 面试题汇总](https://blog.csdn.net/wangming520liwei/article/details/97796772 "JVM 面试题汇总")
- JVM方法区存储内容 是否会动态扩展 是否会出现内存溢出 出现的原因有哪些。
- 如何解决同时存在的对象创建和对象回收问题？
- JVM中最大堆大小有没有限制？
- Java运行时数据区域，导致内存溢出的原因。
- java中一个对象从创建到销毁的过程和 JVM类加载过程
https://blog.csdn.net/m0_37914467/article/details/106441824

####  JVM内存结构

- [JVM内存结构](https://blog.csdn.net/zhaohong_bo/article/details/89392364) 【方法区+虚拟机栈+本地方法栈+程序计数器+堆】
- [JVM原理](https://github.com/xbox1994/Java-Interview/blob/master/MD/Java%E5%9F%BA%E7%A1%80-JVM%E5%8E%9F%E7%90%86.md)
- [Java中的对象一定在堆上分配吗？](https://blog.csdn.net/zhaohong_bo/article/details/89419480 "Java中的对象一定在堆上分配吗？")
- [JAVA的强引用、弱引用、软引用和虚引用，以及用途](https://www.cnblogs.com/mlfz/p/11684185.html)

####  双亲委派模型

- [如何理解双亲委派模型及为什么要使用这种机制](https://blog.csdn.net/weixin_34395205/article/details/86731039 "如何理解双亲委派模型及为什么要使用这种机制")
- [java类加载机制和类加载器以及双亲委派原则解析](https://www.cnblogs.com/iteacat/p/12569008.html "java类加载机制和类加载器以及双亲委派原则解析")

## Android基础

### Activity知识点(必问)

- [Activity启动过程全解析](https://blog.csdn.net/zhaokaiqiang1992/article/details/49428287 "Activity启动过程全解析")
- 启动模式以及使用场景
- onSaveInstanceState以及onRestoreInstanceState使用
- onConfigurationChanged使用以及问题解决

### Fragment知识点

- Fragment生命周期
- Fragment的懒加载
- Fragment之间的通信
- [FragmentPagerAdapter 和FragmentStatePagerAdapter区别](https://juejin.cn/post/6844903726533050381 "FragmentPagerAdapter 和FragmentStatePagerAdapter区别")
- [为什么不建议直接通过使用new Fragment的方式传入数据](https://blog.csdn.net/EthanCo/article/details/50912539 "为什么不建议直接通过使用new Fragment的方式传入数据")
- [为什么官方推荐Fragment.setArguments(Bundle bundle)这种方式来传递参数，而不推荐通过构造方法直接来传递参数呢？](https://blog.csdn.net/asdrt12589wto1/article/details/107961771 "为什么官方推荐Fragment.setArguments(Bundle bundle)这种方式来传递参数，而不推荐通过构造方法直接来传递参数呢？")
- [Androidx 下 Fragment 懒加载的新实现](https://andyjennifer.com/2020/01/19/Androidx%E4%B8%8BFragment%E7%9A%84%E6%87%92%E5%8A%A0%E8%BD%BD/ "Androidx 下 Fragment 懒加载的新实现")


推荐阅读：

1. [Fragment全解析系列（一）：那些年踩过的坑](https://www.jianshu.com/p/d9143a92ad94 "Fragment全解析系列（一）：那些年踩过的坑")
2. Google-Fragment概览
3. Google-与其他Fragment通信


### Service知识点

### Handler知识点(必问)

Handler Looper Message 关系是什么？
Messagequeue 的数据结构是什么？为什么要用这个数据结构？
如何在子线程中创建 Handler?
Handler post方法原理？
Handler消息机制，postDelayed会造成线程阻塞吗？对内存有什么影响？
当访问大量数据出现线程租塞用什么技术解决？
**Handler机制是如何进行线程切换的？**
答：这里先大致解释下，当Looper的loop方法被调用的时候，Looper会从MessageQueue中取出单链表中第一个msg（Message对象），之后会执行msg.target.dispatchMessage(msg)，这个msg中有个target对象，然后target对象里有个dispatchMessage方法，dispatchMessage方法又会调用handleMessage，这时候机智的你肯定意识到了这个target其实就是Handler对象，其实这还不是重点，线程切换的重点在于loop方法是在线程A中执行的，所以即便消息是在线程B产生的，由于loop方法执行在线程A中，所以handleMessage方法也就执行在了线程A中，如果A是主线程，handleMessage方法也就回调在主线程了。


推荐阅读：


- [Handler高频40问](https://mubu.com/doc/4AOg4eG-V2v "Handler高频40问")
- [Android消息机制详解](https://www.zybuluo.com/JeromeLiee/note/1659705#321-%E5%90%8C%E6%AD%A5%E5%B1%8F%E9%9A%9C%E5%92%8C%E5%90%8C%E6%AD%A5%E5%BC%82%E6%AD%A5%E6%B6%88%E6%81%AF) JeromeLiee总结的handler笔记
- [Android主线程阻塞处理及优化](https://blog.csdn.net/weixin_41101173/article/details/79680643 "Android主线程阻塞处理及优化")
- [深入聊聊Android消息机制中的消息队列的设计](https://zhuanlan.zhihu.com/p/82543663 "深入聊聊Android消息机制中的消息队列的设计")
- [深入理解MessageQueue](https://blog.csdn.net/kisty_yao/article/details/71191175 "深入理解MessageQueue")
- [你真的懂Handler.postDelayed()的原理吗?](https://www.cnblogs.com/ldq2016/p/9260783.html "你真的懂Handler.postDelayed()的原理吗?")
- [Handler.postDelayed()是如何精确延迟指定时间的](https://blog.csdn.net/zhangcanyan/article/details/81980166 "Handler.postDelayed()是如何精确延迟指定时间的")
- [Handler延迟消息执行机制，会阻塞吗？](https://blog.csdn.net/u010126792/article/details/85091348 "Handler延迟消息执行机制，会阻塞吗？")
- [Handler之同步屏障机制(sync barrier)+异步消息](https://blog.csdn.net/asdgbc/article/details/79148180 "Handler之同步屏障机制(sync barrier)+异步消息")
- Handler的sendMessage和post的区别
  [Handler 机制中，Message 和 Runnable 的区别？](https://www.jianshu.com/p/43d6cd7b06f1 "Handler 机制中，Message 和 Runnable 的区别？")
- [面试官：“看你简历上写熟悉 Handler 机制，那聊聊 IdleHandler 吧？”  ](https://blog.csdn.net/plokmju88/article/details/104386173/ "面试官：“看你简历上写熟悉 Handler 机制，那聊聊 IdleHandler 吧？”  ")
- [HandlerThread解析](https://zhuanlan.zhihu.com/p/60814560 "HandlerThread解析")

### Intent知识点

- [Android跨进程传递大内存数据](https://blog.csdn.net/qq_29882585/article/details/109498192 "Android跨进程传递大内存数据")

### 数据存储

> 文件和数据库哪个效率高？




# UI控件篇

## 事件分发(重点)

- [Android事件分发机制五：面试官你坐啊](https://bbs.huaweicloud.com/blogs/239940 "Android事件分发机制五：面试官你坐啊")
- [Android事件分发机制 详解攻略，您值得拥有](https://blog.csdn.net/carson_ho/article/details/54136311 "Android事件分发机制 详解攻略，您值得拥有")
- [反思|Android 事件分发机制的设计与实现](https://blog.csdn.net/mq2553299/article/details/100124562 "反思|Android 事件分发机制的设计与实现")
- [View的事件体系(四)View 的事件分发机制](https://www.jianshu.com/p/804eb1a5dd13)

## 自定义View

- [自定义View之自定义View的一般流程](https://www.jianshu.com/p/053d2106a6e0)
- [【带着问题学】关于自定义View你应该知道的知识点](https://juejin.cn/post/6897920522828152839)

## 屏幕适配

- dp+自适应布局+weight比例布局直接适配
- 今日头条适配方式
- 宽高限定符适配方式
- smallestWidth适配

推荐阅读：

- [Android屏幕适配和方案【整理】](https://www.cnblogs.com/whycxb/p/9755012.html "Android屏幕适配和方案【整理】")
- [Android 目前稳定高效的UI适配方案](https://mp.weixin.qq.com/s/X-aL2vb4uEhqnLzU5wjc4Q "Android 目前稳定高效的UI适配方案")



## 主要控件优化

### RecyclerView优化

- [RecyclerView的优化处理](https://juejin.cn/post/6844903930422362119 "RecyclerView的优化处理")
- [RecyclerView 性能优化](https://blankj.com/2018/09/29/optimize-recycler-view/)
- [Android ListView 与 RecyclerView 对比浅析：缓存机制](https://cloud.tencent.com/developer/article/1005658 "Android ListView 与 RecyclerView 对比浅析：缓存机制")
- [RecyclerView与ListView 对比浅析：缓存机制](https://www.cnblogs.com/ganchuanpu/p/8258459.html " RecyclerView与ListView 对比浅析：缓存机制") RecyclerView和ListView的区别(必问)
- [RecyclerView 源码分析](https://conorlee.top/2019/05/31/RecyclerView-source-code/)
- [RecyclerView 预加载机制源码分析](https://conorlee.top/2019/07/17/RecyclerView-pre-initiate/ "RecyclerView 预加载机制源码分析")
- [RecyclerView 中的设计模式](https://conorlee.top/2019/05/30/RecyclerView-Design-Pattern/ "RecyclerView 中的设计模式")
- [Recyclerview 滑动相关功能总结](https://conorlee.top/2020/12/04/RecyclerView_scroll_relatedapi/)

### 嵌套滚动

- [一篇文章让你轻松弄懂NestedScrollingParent & NestedScrollingChild](https://www.jianshu.com/p/8f412c6cb0ef "一篇文章让你轻松弄懂NestedScrollingParent & NestedScrollingChild")


### 动态页面

> 电商类的APP使用居多

- [Android | Tangram动态页面之路](https://blog.csdn.net/weixin_37390872/article/details/106149337 "Android | Tangram动态页面之路")
- [Android动态界面开发框架Tangram使用完整教程](https://blog.csdn.net/u013541140/article/details/89517186 "Android动态界面开发框架Tangram使用完整教程")




# 网络通信篇

## 网络协议

- http与https的区别
- 谈谈你对socket的理解和认识
- TCP和UDP的区别及应用场景
- 对称加密与非对称加密算法
- WebSocket协议原理
- 谈谈MQTT协议

推荐阅读:

- [TCP协议建立连接（三次握手）和断开连接（四次挥手）](https://blog.csdn.net/L_X_Y_HH/article/details/81978528)
- [TCP和UDP的区别及应用场景](https://www.cnblogs.com/liangyc/p/11628208.html)
- [面试官：说说UDP和TCP的区别及应用场景](https://segmentfault.com/a/1190000021815671)
- [ HTTP 与 HTTPS 的区别]()
- [HTTPS的加密过程](https://blog.csdn.net/qq_32998153/article/details/80022489) 对称加密+非对称加密结合
- [网络安全通信（HTTPS）——加密（RSA）和认证(CA)](https://blog.csdn.net/sinat_21026543/article/details/81912427) 这一篇讲解https加密原理通俗易懂。而且非常细致。用非对称加密算法RSA加密 对称算法需要用的主密钥。然后生成会话密钥完成握手协议。之后就可以安全通信了。
- [看完让你彻底理解 WebSocket 原理，附完整的实战代码（包含前端和后端）](https://www.cnblogs.com/nnngu/p/9347635.html "看完让你彻底理解 WebSocket 原理，附完整的实战代码（包含前端和后端）")

## 网络安全


# 架构设计篇

### MVP架构设计

- [高级MVP架构封装演变全过程](https://mp.weixin.qq.com/s?__biz=MzAxMTI4MTkwNQ==&mid=2650824645&idx=1&sn=18fab4a9e35e7656114430f9ecb83ad0&chksm=80b78b5bb7c0024d350962a138e2a84d0a803923b4140ea84a0c6aa18676fb7d40e84c6430f2&mpshare=1&scene=23&srcid=07102utpd9GAgwprZlpCWT2g#rd "高级MVP架构封装演变全过程")
- [Android---我所理解的MVP模式](https://www.jianshu.com/p/a96da61e7f29 "Android---我所理解的MVP模式")


### 组件化架构

> 业务大了代码多了会用到。
为什么要用组件化？
组件之间如何通信？
组件之间如何跳转？

- [ Android为什么要用组件化？](https://blog.csdn.net/guiying712/article/details/55213884 " Android为什么要用组件化？")

### 设计模式

> 1.装饰者模式，代理模式，适配器，桥接模式有什么区别？

- [Android中装饰者模式](https://blog.csdn.net/u014769864/article/details/78439018)
- [适配器模式：代理、适配器、桥接、装饰，这四个模式有何区别？](https://blog.csdn.net/liyf2/article/details/109019285)

# 性能优化篇

> 【面试重点】性能优化：包括启动优化（主要是冷启动）、内存优化、绘制优化、稳定性优化、安装包体积优化等，优化是面试的重中之重。
你在开发中是如何做性能优化的？

- [面试官: 说一下你做过哪些性能优化?](https://www.jianshu.com/p/7cb4ada7a459 "面试官: 说一下你做过哪些性能优化?")

### 启动优化

- [Android App 启动优化全记录](https://androidperformance.com/2019/11/18/Android-App-Lunch-Optimize/#%E5%BA%94%E7%94%A8%E5%90%AF%E5%8A%A8%E6%A6%82%E8%BF%B0 "Android App 启动优化全记录")
- [Activity启动流程](https://blog.csdn.net/zxm317122667/article/details/106660637 "Activity启动流程")
- [Android性能优化--启动优化](https://www.jianshu.com/p/418e34d9d253 "Android性能优化--启动优化")
- [一个更贴近 android 场景的启动框架 | Anchors](https://juejin.cn/post/6854573214380032007 "一个更贴近 android 场景的启动框架 | Anchors")
- [AppLauncher](https://github.com/Ryan-Shz/AppLauncher "AppLauncher")  AppLauncher是一个轻量级的Android App的任务启动器，用来方便、快速的帮助APP处理异步初始化来达到应用启动的最佳性能。
- [SmartStart](https://github.com/conghongjie/SmartStart) Android智能启动框架


### 内存优化

- [Android性能优化：这是一份全面&详细的内存优化指南](https://blog.csdn.net/carson_ho/article/details/79549417 "Android性能优化：这是一份全面&详细的内存优化指南")
- [Android性能优化：手把手带你全面了解 内存泄露 & 解决方案](https://blog.csdn.net/carson_ho/article/details/79407707 "Android性能优化：手把手带你全面了解 内存泄露 & 解决方案")
- [Android内存优化（使用SparseArray和ArrayMap代替HashMap）](https://blog.csdn.net/u010687392/article/details/47809295 "Android内存优化（使用SparseArray和ArrayMap代替HashMap）")

**常见的内存泄露有：**

1.非静态内部类的静态实例
非静态内部类会持有外部类的引用，如果非静态内部类的实例是静态的，就会长期的维持着外部类的引用，组织被系统回收，解决办法是使用静态内部类

2.多线程相关的匿名内部类和非静态内部类
匿名内部类同样会持有外部类的引用，如果在线程中执行耗时操作就有可能发生内存泄漏，导致外部类无法被回收，直到耗时任务结束，解决办法是在页面退出时结束线程中的任务

3.Handler内存泄漏
Handler导致的内存泄漏也可以被归纳为非静态内部类导致的，Handler内部message是被存储在MessageQueue中的，有些message不能马上被处理，存在的时间会很长，导致handler无法被回收，如果handler是非静态的，就会导致它的外部类无法被回收，解决办法是1.使用静态handler，外部类引用使用弱引用处理2.在退出页面时移除消息队列中的消息

4.Context导致内存泄漏
根据场景确定使用Activity的Context还是Application的Context,因为二者生命周期不同，对于不必须使用Activity的Context的场景（Dialog）,一律采用Application的Context,单例模式是最常见的发生此泄漏的场景，比如传入一个Activity的Context被静态类引用，导致无法回收

5.静态View导致泄漏
使用静态View可以避免每次启动Activity都去读取并渲染View，但是静态View会持有Activity的引用，导致无法回收，解决办法是在Activity销毁的时候将静态View设置为null（View一旦被加载到界面中将会持有一个Context对象的引用，在这个例子中，这个context对象是我们的Activity，声明一个静态变量引用这个View，也就引用了activity）

6.WebView导致的内存泄漏
WebView只要使用一次，内存就不会被释放，所以WebView都存在内存泄漏的问题，通常的解决办法是为WebView单开一个进程，使用AIDL进行通信，根据业务需求在合适的时机释放掉

7.资源对象未关闭导致
如Cursor，File等，内部往往都使用了缓冲，会造成内存泄漏，一定要确保关闭它并将引用置为null

8.集合中的对象未清理
集合用于保存对象，如果集合越来越大，不进行合理的清理，尤其是入股集合是静态的

9.Bitmap导致内存泄漏
bitmap是比较占内存的，所以一定要在不使用的时候及时进行清理，避免静态变量持有大的bitmap对象

10.监听器未关闭
很多需要register和unregister的系统服务要在合适的时候进行unregister,手动添加的listener也需要及时移除

而对于内存泄露的检测，常用的工具有LeakCanary、MAT（Memory Analyer Tools）、Android Studio自带的Profiler。



### 绘制优化

> 什么情况下使用 ViewStub、include、merge？
他们的原理是什么？

- [Android性能优化：那些不可忽略的绘制优化](https://www.jianshu.com/p/cbdaeb1bede5 "Android性能优化：那些不可忽略的绘制优化")
- [Android布局优化，全面复盘一波优化思路和优化方案](https://www.jianshu.com/p/eea28f53f846 "Android布局优化，全面复盘一波优化思路和优化方案")

### 安装包优化

- [Android 安装包优化--减小安装包体积](https://www.jianshu.com/p/4c691322aeba?utm_campaign=maleskine&utm_content=note&utm_medium=seo_notes&utm_source=recommendation "Android 安装包优化--减小安装包体积")

### 稳定性优化



# 源码流程篇

## 开源库源码分析

> RxJava的实现原理，它是如何实现线程的控制？
> Retrofit的框架结构是什么？底层是怎么实现的？
> 网络框架是如何搭建？okhttp的底层实现是什么，和Retrofit有什么不同？
> 图片加载框架gilde、Picasso、fresco有什么不同，各自的实现原理是什么？如何搭建一个网络框架？ 

### Glide源码分析

 【面试题】
Glide的优点有哪些？
Glide的缓存原理是什么？

---

Glide的优点主要包括：

- 多种图片格式的缓存，适用于更多的内容表现形式（如Gif、WebP、缩略图、Video）
- 生命周期集成（根据Activity或者Fragment的生命周期管理图片加载请求)Glide可以感知调用页面的生命周期，这就是优势
- 高效处理Bitmap（bitmap的复用和主动回收，减少系统回收压力）
- 高效的缓存策略，灵活（Picasso只会缓存原始尺寸的图片，Glide缓存的是多种规格），加载速度快且内存开销小（默认Bitmap格式的不同，使得内存开销是Picasso的一半）

---

- [Android面试题：Glide](https://blog.csdn.net/songzi1228/article/details/84426165 "Android面试题：Glide")
- [day 20 面试题：Glide面试题](https://blog.csdn.net/xwh_1230/article/details/100006311 "day 20 面试题：Glide面试题")
- [聊一聊关于Glide在面试中的那些事](https://blog.csdn.net/u010302765/article/details/103193470 "聊一聊关于Glide在面试中的那些事")
- [面试官：简历上如果写Glide，请注意以下几点](https://www.cnblogs.com/Android-Alvin/p/12672294.html "面试官：简历上如果写Glide，请注意以下几点")
- [Glide OOM问题解决方法汇总](https://blog.csdn.net/ecjtuhq/article/details/76779931 "Glide OOM问题解决方法汇总")

### LeakCanary源码分析

- [LeakCanary 内存泄漏原理完全解析](https://juejin.cn/post/6844903730190483470#heading-8 "LeakCanary 内存泄漏原理完全解析")


### OkHttp源码分析

【面试问题】

1.如何使用OkHttp进行异步网络请求，并根据请求结果刷新UI？
2.可否介绍一下OkHttp的整个异步请求流程？
3.OkHttp对于网络请求都有哪些优化，如何实现的？
4.OkHttp框架中都用到了哪些设计模式？
5.OKHttp有哪些拦截器，分别起什么作用?
6.OkHttp怎么实现连接池?
7.Okhttp 有哪些优势？


推荐阅读：

- [OkHttp源码解析](https://www.cnblogs.com/huangjialin/p/9469373.html "OkHttp源码解析")
- [Okhttp面试简答](https://blog.csdn.net/songzi1228/article/details/101050603 "Okhttp面试简答")
- [okhttp面试题----拦截器interceptor](https://blog.csdn.net/qiu_suo/article/details/106334570 "okhttp面试题----拦截器interceptor")
- [Okhttp3 总结研究 （面试）](https://blog.csdn.net/u012881042/article/details/79759203 "Okhttp3 总结研究 （面试）")
- [okhttp连接池复用机制](https://blog.csdn.net/tangjiean/article/details/51729371 "okhttp连接池复用机制")
- [okhttp 流程和优化的实现](https://blog.csdn.net/jun_tong/article/details/79808634 "okhttp 流程和优化的实现")
- [一篇让你受用的okhttp分析](https://www.jianshu.com/p/a1b6e71c079d "一篇让你受用的okhttp分析")
- [OkHttp面试之--OkHttp的整个异步请求流程](https://blog.csdn.net/zxm317122667/article/details/53202110 "OkHttp面试之--OkHttp的整个异步请求流程")
- [OkHttp面试之--HttpEngine中的sendRequest方法详解](https://blog.csdn.net/zxm317122667/article/details/53206914 "OkHttp面试之--HttpEngine中的sendRequest方法详解")
- [OkHttp解析大总结](https://blog.csdn.net/zxm317122667/article/details/53217644 "OkHttp解析大总结")
- [Okhttp任务队列工作原理](https://blog.csdn.net/tangjiean/article/details/51736112 "Okhttp任务队列工作原理")
- [Android高频面试专题 - 架构篇（二）okhttp面试必知必会](https://blog.csdn.net/qq41902086/article/details/104562766 "Android高频面试专题 - 架构篇（二）okhttp面试必知必会")
- [Android 网络优化，使用 HTTPDNS 优化 DNS，从原理到 OkHttp 集成](https://www.cnblogs.com/plokmju/p/okhttp_httpdns.html "Android 网络优化，使用 HTTPDNS 优化 DNS，从原理到 OkHttp 集成")

---
Okhttp优势：

1)支持http2，对一台机器的所有请求共享同一个socket
2)内置连接池，支持连接复用，减少延迟
3)支持透明的gzip压缩响应体
4)通过缓存避免重复的请求
5)请求失败时自动重试主机的其他ip，自动重定向
6)丰富的API，可扩展性好



### Retrofit源码分析


- [Android：手把手带你 深入读懂 Retrofit 2.0 源码](https://www.jianshu.com/p/0c055ad46b6c "Android：手把手带你 深入读懂 Retrofit 2.0 源码")



### RxJava源码分析

理解源码之前需要先了解一些RXJava基本知识

- [RxJava操作符之创建操作符(三)](https://www.jianshu.com/p/65bb70007f60 "RxJava操作符之创建操作符(三)")
- [RxJava操作符之转换操作符(四)](https://www.jianshu.com/p/d0d08a518cf6 "RxJava操作符之转换操作符(四)")
- [RxJava操作符之过滤操作符(五)](https://www.jianshu.com/p/66d4dacded9b "RxJava操作符之过滤操作符(五)")
- [RxJava操作符之组合操作符(六)](https://www.jianshu.com/p/aebc8e31f006 "RxJava操作符之组合操作符(六)")

RxJava原理与源码分析

- [RxJava的消息订阅和线程切换原理](https://blog.csdn.net/u011810352/article/details/80518426 "RxJava的消息订阅和线程切换原理")
- [Android：图文解析带你快速了解RxJava原理](https://www.jianshu.com/p/d52ef3ad7460 "Android：图文解析带你快速了解RxJava原理")

RxJava如何进行线程切换的？

- [RxJava 是如何实现线程切换的（上）](https://blog.csdn.net/weixin_33742618/article/details/91863270 "RxJava 是如何实现线程切换的（上）")
- [RxJava 线程切换原理](https://blog.csdn.net/u011060103/article/details/100927415 "RxJava 线程切换原理")
- [RxJava2线程切换原理分析](https://www.cnblogs.com/tony-yang-flutter/p/12331753.html "RxJava2线程切换原理分析")


Rxjava内存泄漏防止方案——RxLifecycle，AutoDispose，RxLife框架

- [Android 使用RxLifecycle解决RxJava内存泄漏](https://www.jianshu.com/p/7fae42861b8d "Android 使用RxLifecycle解决RxJava内存泄漏")
- [解决RxJava内存泄漏（前篇）：RxLifecycle详解及原理分析](https://www.jianshu.com/p/8311410de676 "解决RxJava内存泄漏（前篇）：RxLifecycle详解及原理分析") 理解过滤操作符之takeUntil操作符的使用
- [RxLifecycle详细解析](https://www.jianshu.com/p/e75d320a668c "RxLifecycle详细解析")
- [使用Rxjava2导致的内存泄露问题](https://blog.csdn.net/alex01550/article/details/86496045 "使用Rxjava2导致的内存泄露问题")
- [Rxjava解除订阅②：AutoDispose](https://www.jianshu.com/p/13ba12707068 "Rxjava解除订阅②：AutoDispose")

### Tinker源码分析

- [简单易懂的tinker热修复原理分析](https://juejin.cn/post/6844903651098492942 "简单易懂的tinker热修复原理分析")
- [Tinker源码解析-代码修复和资源修复](https://yutiantina.github.io/2020/04/21/Tinker%E6%BA%90%E7%A0%81%E8%A7%A3%E6%9E%90-%E4%BB%A3%E7%A0%81%E4%BF%AE%E5%A4%8D%E5%92%8C%E8%B5%84%E6%BA%90%E4%BF%AE%E5%A4%8D/ "Tinker源码解析-代码修复和资源修复")



### ARouter源码分析

---
[v_tips] 

<b>路由框架原理：ARouter</b> 【<a href="https://github.com/alibaba/ARouter/blob/master/README_CN.md">官方文档</a>】
【ARouter：现在模块化（组件化）算是比较常见的开发模式了，尤其是在大厂，所以有必要知道ARouter的实现原理，2个模块之间是怎样实现的页面跳转，以及ARouter为了优化性能做了哪些工作】
核心要点：将Route注解中的path地址和Activity.class文件的映射关系保存到它自己生成的java文件的map中
<b>隐式跳转方案</b>,但是一个项目中不可能所有的跳转都是隐式的，这样Manifest文件会有很多过滤配置，而且非常不利于后期维护。
<b>反射跳转方案</b>：需要拿到Activity的类文件，在组件开发的时候，想拿到其他module的类文件是很麻烦的，因为组件开发的时候组件module之间是没有相互引用的，你只能通过找到类的路径去反射拿到这个class。大量的使用反射跳转对性能会有影响。
APT是Annotation Processing Tool的简称,即注解处理工具。apt是在编译期对代码中指定的注解进行解析，然后做一些其他处理（如通过javapoet生成新的Java文件

[/v_tips]



- [ARouter原理剖析及手动实现](https://www.cnblogs.com/ldq2016/p/10504652.html "ARouter原理剖析及手动实现")
- [ARouter组件化框架原理分析](https://blog.csdn.net/lbcwnu/article/details/86249671 "ARouter组件化框架原理分析") 其实ARouter没有用到隐式调转，也没有用到反射技术。而是按需加载路由表类把路由映射关系保存在内存中。
- [Android之ARouter使用和原理解析](https://blog.csdn.net/weixin_37292229/article/details/93375669 "Android之ARouter使用和原理解析")
- [手动实现一个路由框架EasyRouter](https://github.com/Xiasm/EasyRouter/wiki) 仿照ARouter来实现一个简易版的路由框架，实现了组件之间的路由跳转。省略了拦截器等功能
- [Arouter核心思路和源码详解](https://www.cnblogs.com/jymblog/p/11698914.html "Arouter核心思路和源码详解")
- [ARouter源码分析（四）—— 缓存与优化](https://blog.csdn.net/lisdye2/article/details/89517313 "ARouter源码分析（四）—— 缓存与优化")
- [我所理解的Android组件化之通信机制](https://www.sohu.com/a/274178317_611601 "我所理解的Android组件化之通信机制") 
- [ARouter系列三：依赖注入暴露服务](https://www.jianshu.com/p/08029e7e4efc "ARouter系列三：依赖注入暴露服务")
- [ARouter系列一：Activity跳转原理详解](https://www.jianshu.com/p/559cbd9c89e3 "ARouter系列一：Activity跳转原理详解")


## Android框架层源码解析

### Activity启动流程

[![](https://i.loli.net/2021/04/13/6fFx4ehprUEHYD9.jpg)](https://i.loli.net/2021/04/13/6fFx4ehprUEHYD9.jpg)

1. 点击桌面App图标，Launcher进程采用Binder IPC向system_server进程发起startActivity请求；
2. system_server进程接收到请求后，向zygote进程发送创建进程的请求；
3. Zygote进程fork出新的子进程，即App进程；
4. App进程，通过Binder IPC向sytem_server进程发起attachApplication请求；
5. system_server进程在收到请求后，进行一系列准备工作后，再通过binder IPC向App进程发送scheduleLaunchActivity请求；
6. App进程的binder线程（ApplicationThread）在收到请求后，通过handler向主线程发送LAUNCH_ACTIVITY消息；
7. 主线程在收到Message后，通过发射机制创建目标Activity，并回调Activity.onCreate()等方法。

推荐阅读：

- [startActivity启动过程分析](http://gityuan.com/2016/03/12/start-activity/)
- [简述Activity生命周期](http://gityuan.com/2016/03/18/start-activity-cycle/)


### Service启动流程

[![](https://i.loli.net/2021/04/13/RLAGa6ShBVYeQyW.jpg)](https://i.loli.net/2021/04/13/RLAGa6ShBVYeQyW.jpg)

启动流程：

1. Process A进程采用Binder IPC向system_server进程发起startService请求；
2. system_server进程接收到请求后，向zygote进程发送创建进程的请求；
3. zygote进程fork出新的子进程Remote Service进程；
4. Remote Service进程，通过Binder IPC向sytem_server进程发起attachApplication请求；
5. system_server进程在收到请求后，进行一系列准备工作后，再通过binder IPC向remote Service进程发送scheduleCreateService请求；
6. Remote Service进程的binder线程在收到请求后，通过handler向主线程发送CREATE_SERVICE消息；
7. 主线程在收到Message后，通过发射机制创建目标Service，并回调Service.onCreate()方法。

推荐阅读：

- [startService启动过程分析](http://gityuan.com/2016/03/06/start-service/)

### 事件分发机制
[![](https://i.loli.net/2021/04/14/qHsYLBfCXx63SKW.jpg)](https://i.loli.net/2021/04/14/qHsYLBfCXx63SKW.jpg)


1. `onInterceptTouchEvent`返回值true表示事件拦截， `onTouch/onTouchEvent` 返回值true表示事件消费。
2. 触摸事件先交由`Activity.dispatchTouchEvent`。再一层层往下分发，当中间的ViewGroup都不拦截时，进入最底层的`View`后，开始由最底层的`OnTouchEvent`来处理，如果一直不消费，则最后返回到`Activity.OnTouchEvent`。
3. `ViewGroup`才有`onInterceptTouchEvent`拦截方法。在分发过程中，中间任何一层ViewGroup都可以直接拦截，则不再往下分发，而是交由发生拦截操作的ViewGroup的OnTouchEvent来处理。
4. 子View可调用requestDisallowInterceptTouchEvent方法，来设置disallowIntercept=true，从而阻止父ViewGroup的onInterceptTouchEvent拦截操作。
5. OnTouchEvent由下往上冒泡时，当中间任何一层的OnTouchEvent消费该事件，则不再往上传递，表示事件已处理。
6. 如果View没有消费ACTION_DOWN事件，则之后的ACTION_MOVE等事件都不会再接收。
7. 只要View.onTouchEvent是可点击或可长按，则消费该事件.
8. onTouch优先于onTouchEvent执行，上面流程图中省略，onTouch的位置在onTouchEvent前面。当onTouch返回true,则不执行onTouchEvent,否则会执行onTouchEvent。onTouch只有View设置了OnTouchListener，且是enable的才执行该方法。

推荐阅读：

- [Android事件分发机制](http://gityuan.com/2015/09/19/android-touch/)
- [View的事件体系(四)View 的事件分发机制](https://www.jianshu.com/p/804eb1a5dd13)
- [[图片备份]个人理解的Android事件分发机制](https://blog.csdn.net/DayDayPlayPhone/article/details/53223840)

## Java层源码解析

> HashMap底层实现，它和LinkHashMap有什么区别？

# 算法设计

## 理论知识

- [算法的时间与空间复杂度（一看就懂）](https://zhuanlan.zhihu.com/p/50479555)

## 数据结构

- [图解数据结构和算法-网站](https://www.cxyxiaowu.com/7374.html "图解数据结构和算法-网站")
- [浅谈单链表与双链表的区别](https://blog.csdn.net/kangxidagege/article/details/80211225 "浅谈单链表与双链表的区别")

## 刷题资料

-  hello-algorithm | 在线阅读：[hello-algorithm](https://github.com/geekxh/hello-algorithm "https://github.com/geekxh/hello-algorithm") | 「算法面试+算法知识」针对小白的算法训练。小浩算法是一套针对小白的完整的算法训练流程！
-  十大排序算法 | 在线阅读：[bookstack.cn](https://www.bookstack.cn/read/JS-Sorting-Algorithm/1.bubbleSort.md) | 一本关于排序算法的 GitBook 在线书籍 《十大经典排序算法》，使用 JavaScript & Python & Go & Java 实现。 排序算法可以分为内部排序和外部排序，内部排序是数据记录在内存中进行排序，而外部排序是因排序的数据很大，一次不能容纳全部的排序记录，在排序过程中需要访问外存。常见的内部排序算法有：插入排序、希尔排序、选择排序、冒泡排序、归并排序、快速排序、堆排序、基数排序等。
- Leetcode 前 300 题算法题解析（Java） | [bookstack.cn](https://www.bookstack.cn/read/wind-liang-eetcode/65eddf354510804a.md)

# 新技术篇

## Jetpack

[![](https://i.loli.net/2021/08/03/scTDSQU3dZK1YFa.jpg)](https://i.loli.net/2021/08/03/scTDSQU3dZK1YFa.jpg)

- [Android Jetpack从入门到精通（深度好文，值得收藏）
](https://blog.csdn.net/weixin_43901866/article/details/106057755)

### Jetpack架构组件

Android Architecture Components的核心是Lifecycle、LiveData、ViewModel 以及 Room，通过它可以非常优雅的让数据与界面进行交互，并做一些持久化的操作，高度解耦，自动管理生命周期，而且不用担心内存泄漏的问题。

- Room 一个强大的SQLite对象映射库。
- ViewModel 一类对象，它用于为UI组件提供数据，在设备配置发生变更时依旧可以存活。
- LiveData 一个可感知生命周期、可被观察的数据容器，它可以存储数据，还会在数据发生改变时进行提醒。
- Lifecycle 包含LifeCycleOwer和LifecycleObserver，分别是生命周期所有者和生命周期感知者。

Android Architecture Components的特点

- 数据驱动型编程 变化的永远是数据，界面无需更改。
- 感知生命周期，防止内存泄漏。
- 高度解耦 数据，界面高度分离。
- 数据持久化 数据、ViewModel不与UI的生命周期挂钩，不会因为界面的重建而销毁。

推荐阅读:

- [基于LiveData实现事件总线思路和方案](https://yutiantina.github.io/2019/09/20/%E5%9F%BA%E4%BA%8ELiveData%E5%AE%9E%E7%8E%B0%E4%BA%8B%E4%BB%B6%E6%80%BB%E7%BA%BF%E6%80%9D%E8%B7%AF%E5%92%8C%E6%96%B9%E6%A1%88/ "基于LiveData实现事件总线思路和方案")



# 实战问题篇

- [Android工程中方法数超过65536解决方法](https://blog.csdn.net/gongxiaoou/article/details/81281415 "Android工程中方法数超过65536解决方法")

### 权限处理

- [Android运行时权限流程梳理](https://juejin.cn/post/6844904166616203271)

### 主题换肤

- [Android换肤总结](https://blog.csdn.net/shanshui911587154/article/details/104820919)
- [Android夜间模式调研总结](https://blog.csdn.net/u013478336/article/details/52484322)


### Socket粘包半包

- [Socket粘包问题的3种解决方案，最后一种最完美！](https://blog.csdn.net/g6U8W7p06dCO99fQ3/article/details/112342755)

# 面试篇

<g-emoji class="g-emoji">🔥</g-emoji>

### 开源笔记


- [Android-Review(原)](https://github.com/JasonWu1111/Android-Review) <g-emoji class="g-emoji">🔥</g-emoji>Android 复习资料汇总<g-emoji class="g-emoji">🔥</g-emoji>（每周持续更新中~）
- [Android-Review](https://github.com/collectAndroid/Android-Review) Android 复习资料汇总（每周持续更新~）
- [Android-ReadTheFuckingSourceCode](https://github.com/jeanboydev/Android-ReadTheFuckingSourceCode) 记录日常的开发技巧，开发中遇到的技术重点、难点，各个知识点的总结，优质面试题等等。持续更新...
- [LearningNotes](https://github.com/WithLei/LearningNotes)
- [Awesome-Android-Interview](https://github.com/JsonChao/Awesome-Android-Interview/) <g-emoji class="g-emoji">🔥</g-emoji> 随着Android技术发展的成熟，Kotlin、大前端技术Flutter、RN、小程序等一下子就进入了我们的视野内，同时，Android自身的技术栈也正在不断扩展，比如在国外大热的Jetpack。因此，Android开发者们越来越焦虑，越来越迷茫，每个人的时间和精力是有限的，我们到底应该学什么才能有效地提高自身的竞争力呢?其实，首先我们应该优先深入学习工作中用到的技术，其次，关注这2年来Android最新的面试题所涉及的知识点，根据自身的实际情况有选择地进行针对性的学习和提升。只有这样，自身才不会被所谓的 互联网寒冬 吓倒。Awesome-Android-Interview搜集了国内一线及二线互联网公司最常出现的面试题，非常全面，笔者花费了很大的精力和时间，希望得到大家的支持。
- [AndroidGuide](https://leavesc.gitbook.io/androidguide/#androidguide "AndroidGuide") <g-emoji class="g-emoji">🔥</g-emoji> 这是一份 Android 开发从基础入门到进阶的完整（并不是）指南，所有文章都是本人这几年时间里一字一字码出来的，文章的更新方向和更新频率以我的学习计划为导向，会一直持续密集更新下去..... [(gitbook访问不了，可以访问github地址)](https://github.com/leavesC/AndroidGuide) <g-emoji class="g-emoji">🔥</g-emoji>
- [LearningNotes](https://github.com/francistao/LearningNotes "LearningNotes") 
- [Android和Flutter笔记文档](https://blog.yorek.xyz/android/paid/zsxq/week21-mvc%26mvp%26mvvm/) 基于开源文档Mkdocs部署搭建的学习笔记个人网站 
- [android-bookmarks](https://app.gitbook.com/@bookmarks/s/android-bookmarks/android/readme) 以前我自己总结的技术资料，技术笔记。


### 面试文献

Java基础

- [Java-Interview](https://github.com/xbox1994/Java-Interview "Java-Interview") <g-emoji class="g-emoji">🔥</g-emoji> 经历BAT面试后总结的【高级Java后台开发面试指南】，纯净干货无废话，针对高频面试点 

Android

- [Android 高级开发面试题以及答案整理](https://juejin.im/post/6844903797270003719 "Android 高级开发面试题以及答案整理")
- [Android 中高级面试必知必会](https://juejin.im/post/6844904009438855181 "Android 中高级面试必知必会")
- [Android 高级面试高频知识点](https://juejin.im/post/6844904100597858312 "Android 高级面试高频知识点")
- [Android面试重难点高频问题](https://www.jianshu.com/p/74a007b22174 "Android面试重难点高频问题")
- [Android面试题集](https://www.kancloud.cn/aslai/interview-guide/1113658 "Android面试题集")
- [通过三轮面试斩获腾讯offer的Android菜鸟亲述：末流渣本原来也有“春天”](https://www.jianshu.com/p/72794b7bec6f "通过三轮面试斩获腾讯offer的Android菜鸟亲述：末流渣本原来也有“春天”")
- [Android 面试题积累 (高阶)](https://conorlee.top/2018/03/01/IntervieweeQuestions-senior/#32-retrofit%E7%9A%84%E4%BA%86%E8%A7%A3)
- [AndroidOfferKiller](https://github.com/Blankj/AndroidOfferKiller) <g-emoji class="g-emoji">🔥</g-emoji> 安卓 offer 收割基 <g-emoji class="g-emoji">🔥</g-emoji>
- [Android面试文档](https://www.kancloud.cn/smartsean/android/1106138) 看云·Android面试文档


### 个人面经

- [我跳槽了！2020年Android找工作面试，你必须提前知道的一些事](https://www.kaelli.com/43.html "我跳槽了！2020年Android找工作面试，你必须提前知道的一些事")
- [2018已经很冷，2019年Android工作或更难找——面试基础技能罗列](https://www.kaelli.com/28.html "2018已经很冷，2019年Android工作或更难找——面试基础技能罗列")
- [2017年Android面试体验之我一个周面了20多次](https://www.kaelli.com/3.html "2017年Android面试体验之我一个周面了20多次")
- [分享一份非常强势的Android面试题](https://zhuanlan.zhihu.com/p/42740219 "分享一份非常强势的Android面试题")
- [Android 面试题积累 (高阶)](https://conorlee.top/2018/03/01/IntervieweeQuestions-senior/ "Android 面试题积累 (高阶)")
- [Android中高级面试题(看云)](https://www.kancloud.cn/aslai/interview-guide/1126416 "Android中高级面试题(看云)")
- [2019年下半年最接地气的Android面经](https://juejin.cn/post/6844903952085942279 "2019年下半年最接地气的Android面经")
- [热腾腾的腾讯Android岗面经分享||8月6号已入职企鹅FM](https://juejin.cn/post/6858987892195360775 "热腾腾的腾讯Android岗面经分享||8月6号已入职企鹅FM")
- [一位6年老Android面经总结](https://segmentfault.com/a/1190000018827242 "一位6年老Android面经总结")
- [2年Android开发面经分享：跳槽网易个人创业失败后，拿到快手,字节,百度等的Offer之旅](https://cloud.tencent.com/developer/article/1672067 "2年Android开发面经分享：跳槽网易个人创业失败后，拿到快手,字节,百度等的Offer之旅")
- [三年经验Android开发面经总结](http://www.androidchina.net/11772.html)
- [Android面经| 回顾展望](https://withlei.github.io/2019/06/Android%E9%9D%A2%E7%BB%8F-%E5%9B%9E%E9%A1%BE%E5%B1%95%E6%9C%9B/)
- [BAT大厂Android面试知识点，请客官拿好](https://andyjennifer.com/2019/02/23/BAT%E5%A4%A7%E5%8E%82Android%E9%9D%A2%E8%AF%95%E7%9F%A5%E8%AF%86%E7%82%B9%EF%BC%8C%E8%AF%B7%E5%AE%A2%E5%AE%98%E6%8B%BF%E5%A5%BD/) 年年寒冬，年年也挡不住一个安卓程序员追求大厂的决心。想要进入大厂，我们需要掌握哪些知识点呢？这里，我为大家梳理了一个整体的知识架构。整体包括Java、Android、算法、网络等，并且我也在相应知识点下推荐了与该知识点相关的书籍与博客。希望大家阅读之后，能帮助大家完善与整理自己的知识体系。祝大家早日进入自己理想的公司~~


### 面试题目

- [为什么 Android 要采用 Binder 作为 IPC 机制？](https://www.zhihu.com/question/39440766/answer/89210950 "为什么 Android 要采用 Binder 作为 IPC 机制？")

### 跳槽攻略

- [8年Android，6次跳槽，看了15个源代码，最后阿里6面被拒了，HR竟手把手教我跳槽攻略](https://blog.csdn.net/ajsliu1233/article/details/108830306)


# 社区网站篇

- 面圈网：[http://www.mianshigee.com/job/Android/s2/](http://www.mianshigee.com/job/Android/s2/ "http://www.mianshigee.com/job/Android/s2/")
	
	
