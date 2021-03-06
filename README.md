<!-- TOC -->

- [Python基础](#python基础)
    - [文件操作](#文件操作)
        - [有一个jsonline格式的文件file.txt大小约为10K](#有一个jsonline格式的文件filetxt大小约为10k)
        - [文件路径](#文件路径)
        - [补充缺失的代码](#补充缺失的代码)
    - [模块与包](#模块与包)
        - [列出5个python标准库](#列出5个python标准库)
        - [输入日期， 判断这一天是这一年的第几天？](#输入日期-判断这一天是这一年的第几天)
        - [打乱一个排好序的list对象alist？](#打乱一个排好序的list对象alist)
    - [数据类型](#数据类型)
        - [python常见的列表推导式？](#python常见的列表推导式)
        - [现有字典 d= {'a':24,'g':52,'i':12,'k':33}请按value值进行排序?](#现有字典-d-a24g52i12k33请按value值进行排序)
        - [字典推导式](#字典推导式)
        - [请反转字符串 "aStr"?](#请反转字符串-astr)
        - [将字符串 "k:1|k1:2|k2:3|k3:4"，处理成字典 {k:1,k1:2,...}](#将字符串-k1k12k23k34处理成字典-k1k12)
        - [请按alist中元素的age由大到小排序](#请按alist中元素的age由大到小排序)
        - [下面代码的输出结果将是什么？](#下面代码的输出结果将是什么)
        - [写一个列表生成式，产生一个公差为11的等差数列](#写一个列表生成式产生一个公差为11的等差数列)
        - [给定两个列表，怎么找出他们相同的元素和不同的元素？](#给定两个列表怎么找出他们相同的元素和不同的元素)
        - [请写出一段python代码实现删除list里面的重复元素？](#请写出一段python代码实现删除list里面的重复元素)
        - [Python中生成随机整数、随机小数、0--1之间小数方法](#python中生成随机整数随机小数0--1之间小数方法)
        - [Python中断言方法举例](#python中断言方法举例)
    - [企业面试题](#企业面试题)
        - [python2和python3区别？列举5个](#python2和python3区别列举5个)
        - [python新式类和经典类的区别？](#python新式类和经典类的区别)
        - [python中内置的数据结构有几种？](#python中内置的数据结构有几种)
        - [可变类型和不可变类型](#可变类型和不可变类型)
        - [python如何实现单例模式?请写出两种实现方式?](#python如何实现单例模式请写出两种实现方式)
        - [反转一个整数，例如-123 --> -321](#反转一个整数例如-123-----321)
        - [设计实现遍历目录与子目录，抓取.pyc文件](#设计实现遍历目录与子目录抓取pyc文件)
        - [一行代码实现1-100之和](#一行代码实现1-100之和)
        - [Python-遍历列表时删除元素的正确做法](#python-遍历列表时删除元素的正确做法)
        - [字符串的操作题目](#字符串的操作题目)
        - [is和==有什么区别？](#is和有什么区别)
        - [求出列表所有奇数并构造新列表](#求出列表所有奇数并构造新列表)
        - [用一行python代码写出1+2+3+10248](#用一行python代码写出12310248)
        - [Python中变量的作用域？（变量查找顺序)](#python中变量的作用域变量查找顺序)
        - [字符串 `"123"` 转换成 `123`，不使用内置api，例如 `int()`](#字符串-123-转换成-123不使用内置api例如-int)
        - [给定一个整数数组和一个目标值，找出数组中和为目标值的两个数](#给定一个整数数组和一个目标值找出数组中和为目标值的两个数)
        - [给列表中的字典排序](#给列表中的字典排序)
        - [统计一个文本中单词频次最高的10个单词？](#统计一个文本中单词频次最高的10个单词)
        - [利用collections库的Counter方法统计字符串每个单词出现的次数"kjalfj;ldsjafl;hdsllfdhg;lahfbl;hl;ahlf;h"](#利用collections库的counter方法统计字符串每个单词出现的次数kjalfjldsjaflhdsllfdhglahfblhlahlfh)
        - [请写出一个函数满足以下条件](#请写出一个函数满足以下条件)
        - [使用单一的列表生成式来产生一个新的列表](#使用单一的列表生成式来产生一个新的列表)
        - [用一行代码生成[1,4,9,16,25,36,49,64,81,100]](#用一行代码生成149162536496481100)
        - [输入某年某月某日，判断这一天是这一年的第几天？](#输入某年某月某日判断这一天是这一年的第几天)
        - [两个有序列表，l1、l2对这两个列表进行合并不可使用extend](#两个有序列表l1l2对这两个列表进行合并不可使用extend)
        - [给定一个任意长度数组，实现一个函数](#给定一个任意长度数组实现一个函数)
        - [写一个函数找出一个整数数组中，第二大的数](#写一个函数找出一个整数数组中第二大的数)
        - [阅读一下代码他们的输出结果是什么？](#阅读一下代码他们的输出结果是什么)
        - [统计一段字符串中字符出现的次数](#统计一段字符串中字符出现的次数)
        - [super函数的具体用法和场景](#super函数的具体用法和场景)
- [Python高级](#python高级)
    - [元类](#元类)
        - [Python中类方法、类实例方法、静态方法有何区别？](#python中类方法类实例方法静态方法有何区别)
        - [遍历一个object的所有属性，并print每一个属性名？](#遍历一个object的所有属性并print每一个属性名)
        - [写一个类，并让它尽可能多的支持操作符?](#写一个类并让它尽可能多的支持操作符)
        - [提高python运行效率的方法](#提高python运行效率的方法)
        - [介绍Cython、Pypy、CPython、Numba各有什么缺点](#介绍cythonpypycpythonnumba各有什么缺点)
        - [请描述抽象类和接口类的区别和联系](#请描述抽象类和接口类的区别和联系)
        - [Python中如何动态获取和设置对象的属性？](#python中如何动态获取和设置对象的属性)
    - [内存管理与垃圾回收机制](#内存管理与垃圾回收机制)
        - [哪些操作会导致Python内存溢出，怎么处理？](#哪些操作会导致python内存溢出怎么处理)
        - [关于Python内存管理](#关于python内存管理)
        - [Python的内存管理与垃圾回收机机制及调优手段？](#python的内存管理与垃圾回收机机制及调优手段)
        - [引用计数的优缺点](#引用计数的优缺点)
            - [优点：](#优点)
            - [缺点:](#缺点)
        - [内存泄露是什么？如何避免？](#内存泄露是什么如何避免)
    - [函数](#函数)
        - [简述read、readline、readlines的区别？](#简述readreadlinereadlines的区别)
        - [什么是Hash（散列函数）？](#什么是hash散列函数)
        - [python函数重载机制？](#python函数重载机制)
        - [手写一个判断时间的装饰器](#手写一个判断时间的装饰器)
        - [编写函数的4个原则](#编写函数的4个原则)
        - [函数调用参数的传递方式是值传递还是引用传递？](#函数调用参数的传递方式是值传递还是引用传递)
        - [如何在function里面设置一个全局变量](#如何在function里面设置一个全局变量)
        - [对缺省参数的理解？](#对缺省参数的理解)
        - [带参数的装饰器?](#带参数的装饰器)
        - [为什么函数名字可以当做参数用?](#为什么函数名字可以当做参数用)
        - [Python中pass语句的作用是什么？](#python中pass语句的作用是什么)
        - [map函数和reduce函数？](#map函数和reduce函数)
        - [回调函数，如何通信的?](#回调函数如何通信的)
        - [Python主要的内置数据类型都有哪些？ print(dir("a")) 的输出？](#python主要的内置数据类型都有哪些-printdira-的输出)
        - [hasattr()、getattr()、setattr()函数使用详解？](#hasattrgetattrsetattr函数使用详解)
        - [一句话解决阶乘函数？](#一句话解决阶乘函数)
        - [Python 递归深度默认是多少？递归深度限制的原因是什么？](#python-递归深度默认是多少递归深度限制的原因是什么)
        - [递归函数停止的条件？](#递归函数停止的条件)
        - [什么是lambda函数？它有什么好处？写一个匿名函数求两个数的和](#什么是lambda函数它有什么好处写一个匿名函数求两个数的和)
    - [设计模式](#设计模式)
        - [对设计模式的理解，简述你了解的设计模式？](#对设计模式的理解简述你了解的设计模式)
        - [请手写一个单例模式](#请手写一个单例模式)
        - [单例模式的应用场景有那些？](#单例模式的应用场景有那些)
        - [对装饰器的理解，并写出一个计时器记录方法执行性能的装饰器？](#对装饰器的理解并写出一个计时器记录方法执行性能的装饰器)
        - [解释以下什么是闭包？](#解释以下什么是闭包)
        - [函数装饰器有什么作用？](#函数装饰器有什么作用)
        - [生成器，迭代器的区别？](#生成器迭代器的区别)
        - [简述any()和all()方法](#简述any和all方法)
        - [X是什么类型?](#x是什么类型)
        - [请用一行代码 实现将1-N的整数列表以3为单位分组](#请用一行代码-实现将1-n的整数列表以3为单位分组)
        - [Python中yield的用法?](#python中yield的用法)
    - [面向对象](#面向对象)
        - [Python中的可变对象和不可变对象？](#python中的可变对象和不可变对象)
        - [Python的魔法方法](#python的魔法方法)
        - [简述面向对象中__new__和__init__区别](#简述面向对象中__new__和__init__区别)
        - [面向对象中怎么实现只读属性?](#面向对象中怎么实现只读属性)
        - [谈谈你对面向对象的理解？](#谈谈你对面向对象的理解)
    - [正则表达式](#正则表达式)
        - [字符串a = "not 404 found 张三 99 深圳"，每个词中间是空格，用正则过滤掉英文和数字，最终输出"张三  深圳"](#字符串a--not-404-found-张三-99-深圳每个词中间是空格用正则过滤掉英文和数字最终输出张三--深圳)
        - [请写出一段代码用正则匹配出ip？](#请写出一段代码用正则匹配出ip)
        - [正则匹配，匹配日期2018-03-20](#正则匹配匹配日期2018-03-20)
        - [a = “abbbccc”，用正则匹配为abccc,不管有多少b，就出现一次？](#a--abbbccc用正则匹配为abccc不管有多少b就出现一次)
        - [Python字符串查找和替换？](#python字符串查找和替换)
        - [用Python匹配HTML`<div class="nam">中国</div>`，用正则匹配出标签里面的内容（“中国”），其中class的类名是不确定的，并说明<.> 和 <.*?> 有什么区别](#用python匹配htmldiv-classnam中国div用正则匹配出标签里面的内容中国其中class的类名是不确定的并说明-和--有什么区别)
        - [正则表达式贪婪与非贪婪模式的区别？](#正则表达式贪婪与非贪婪模式的区别)
        - [写出开头匹配字母和下划线，末尾是数字的正则表达式？](#写出开头匹配字母和下划线末尾是数字的正则表达式)
        - [正则表达式操作](#正则表达式操作)
        - [请匹配出变量A中的json字符串。](#请匹配出变量a中的json字符串)
        - [怎么过滤评论中的表情？](#怎么过滤评论中的表情)
        - [正则匹配以163.com结尾的邮箱](#正则匹配以163com结尾的邮箱)
        - [a="张明 98分"，用re.sub，将98替换为100](#a张明-98分用resub将98替换为100)
        - [简述Python里面search和match的区别](#简述python里面search和match的区别)
        - [正则re.complie作用](#正则recomplie作用)
    - [系统编程](#系统编程)
        - [10个Linux常用命令](#10个linux常用命令)
        - [进程总结](#进程总结)
        - [请介绍一下Python的线程同步？](#请介绍一下python的线程同步)
            - [setDaemon(False)](#setdaemonfalse)
            - [setDaemon（True)](#setdaemontrue)
            - [join（线程同步)](#join线程同步)
        - [谈谈你对多进程，多线程，以及协程的理解，项目是否用？](#谈谈你对多进程多线程以及协程的理解项目是否用)
        - [多进程更稳定还是多线程更稳定？为什么？](#多进程更稳定还是多线程更稳定为什么)
        - [多线程的致命缺点是什么？](#多线程的致命缺点是什么)
        - [进程间通信有哪些方式？](#进程间通信有哪些方式)
        - [Python的GIL](#python的gil)
        - [Python异步使用场景有那些？](#python异步使用场景有那些)
        - [多线程共同操作同一个数据互斥锁同步？](#多线程共同操作同一个数据互斥锁同步)
        - [什么是多线程竞争？](#什么是多线程竞争)
        - [解释以下什么是锁，有哪几种锁？](#解释以下什么是锁有哪几种锁)
        - [什么是死锁？](#什么是死锁)
        - [多线程交互访问数据，如果访问到了就不访问了？](#多线程交互访问数据如果访问到了就不访问了)
        - [什么是线程安全，什么是互斥锁？](#什么是线程安全什么是互斥锁)
        - [说说下面几个概念：同步，异步，阻塞，非阻塞？](#说说下面几个概念同步异步阻塞非阻塞)
        - [什么是僵尸进程和孤儿进程？怎么避免僵尸进程？](#什么是僵尸进程和孤儿进程怎么避免僵尸进程)
        - [python中进程与线程的使用场景？](#python中进程与线程的使用场景)
        - [线程是并发还是并行，进程是并发还是并行？](#线程是并发还是并行进程是并发还是并行)
        - [并行(parallel)和并发（concurrency)?](#并行parallel和并发concurrency)
        - [IO密集型和CPU密集型区别？](#io密集型和cpu密集型区别)
        - [python asyncio的原理？](#python-asyncio的原理)
    - [网络编程](#网络编程)
        - [怎么实现强行关闭客户端和服务器之间的连接?](#怎么实现强行关闭客户端和服务器之间的连接)
        - [简述TCP和UDP的区别以及优缺点?](#简述tcp和udp的区别以及优缺点)
            - [区别](#区别)
            - [优缺点](#优缺点)
        - [简述浏览器通过WSGI请求动态资源的过程?](#简述浏览器通过wsgi请求动态资源的过程)
        - [描述用浏览器访问www.baidu.com的过程](#描述用浏览器访问wwwbaiducom的过程)
        - [Post和Get请求的区别?](#post和get请求的区别)
        - [cookie和session的区别？](#cookie和session的区别)
        - [列出你知道的HTTP协议的状态码，说出表示什么意思？](#列出你知道的http协议的状态码说出表示什么意思)
        - [请简单说一下三次握手和四次挥手？](#请简单说一下三次握手和四次挥手)
        - [说一下什么是tcp的2MSL？](#说一下什么是tcp的2msl)
        - [为什么客户端在TIME-WAIT状态必须等待2MSL的时间？](#为什么客户端在time-wait状态必须等待2msl的时间)
        - [说说HTTP和HTTPS区别？](#说说http和https区别)
        - [谈一下HTTP协议以及协议头部中表示数据类型的字段？](#谈一下http协议以及协议头部中表示数据类型的字段)
        - [HTTP请求方法都有什么？](#http请求方法都有什么)
        - [使用Socket套接字需要传入哪些参数 ？](#使用socket套接字需要传入哪些参数-)
        - [HTTP常见请求头？](#http常见请求头)
        - [七层模型？](#七层模型)
        - [url的形式？](#url的形式)
- [Web](#web)
    - [分别从前端、后端、数据库阐述web项目的性能优化](#分别从前端后端数据库阐述web项目的性能优化)
    - [Flask](#flask)
        - [对Flask蓝图(Blueprint)的理解？](#对flask蓝图blueprint的理解)
            - [蓝图的定义](#蓝图的定义)
            - [蓝图的应用场景](#蓝图的应用场景)
            - [蓝图的缺点：](#蓝图的缺点)
            - [使用蓝图的三个步骤](#使用蓝图的三个步骤)
        - [Flask和Django路由映射的区别？](#flask和django路由映射的区别)
    - [Django](#django)
        - [什么是wsgi,uwsgi,uWSGI?](#什么是wsgiuwsgiuwsgi)
        - [Django、Flask、Tornado的对比？](#djangoflasktornado的对比)
            - [Django](#django-1)
            - [Flask](#flask-1)
            - [Tornado](#tornado)
        - [简述同源策略](#简述同源策略)
        - [CORS和CSRF的区别？](#cors和csrf的区别)
        - [Session、Cookie、JWT的理解](#sessioncookiejwt的理解)
        - [简述Django请求生命周期](#简述django请求生命周期)
        - [用的restframework完成api发送时间时区](#用的restframework完成api发送时间时区)
        - [nginx,tomcat,apache都是什么？](#nginxtomcatapache都是什么)
        - [请给出你熟悉关系数据库范式有哪些，有什么作用？](#请给出你熟悉关系数据库范式有哪些有什么作用)
        - [简述QQ登陆过程](#简述qq登陆过程)
        - [项目中日志的作用](#项目中日志的作用)
            - [日志相关概念](#日志相关概念)
            - [日志的作用](#日志的作用)
            - [log日志中，我们需要用时间戳记录error,warning等的发生时间，请用datetime模块打印当前时间戳 “2018-04-01 11:38:54”](#log日志中我们需要用时间戳记录errorwarning等的发生时间请用datetime模块打印当前时间戳-2018-04-01-113854)
        - [异常名称及其意义](#异常名称及其意义)
        - [django中间件的使用？](#django中间件的使用)
        - [谈一下你对uWSGI和nginx的理解？](#谈一下你对uwsgi和nginx的理解)
        - [Python中三大框架各自的应用场景？](#python中三大框架各自的应用场景)
        - [Django中哪里用到了线程？哪里用到了协程？哪里用到了进程？](#django中哪里用到了线程哪里用到了协程哪里用到了进程)
        - [有用过Django REST framework吗？](#有用过django-rest-framework吗)
    - [爬虫](#爬虫)
        - [什么是爬虫，为什么要用爬虫?](#什么是爬虫为什么要用爬虫)
        - [爬虫的基本流程？](#爬虫的基本流程)
        - [如何提高爬取效率？](#如何提高爬取效率)
        - [爬虫协议？](#爬虫协议)
        - [试列出至少三种目前流行的大型数据库](#试列出至少三种目前流行的大型数据库)
        - [列举您使用过的Python网络爬虫所用到的网络数据包?](#列举您使用过的python网络爬虫所用到的网络数据包)
        - [你用过的爬虫框架或者模块有哪些？优缺点？](#你用过的爬虫框架或者模块有哪些优缺点)
            - [框架或者模块](#框架或者模块)
        - [写爬虫是用多进程好？还是多线程好？](#写爬虫是用多进程好还是多线程好)
        - [常见的反爬虫和应对方法？](#常见的反爬虫和应对方法)
        - [解析网页的解析器使用最多的是哪几个?](#解析网页的解析器使用最多的是哪几个)
        - [需要登录的网页，如何解决同时限制ip，cookie, session](#需要登录的网页如何解决同时限制ipcookie-session)
        - [验证码的解决?](#验证码的解决)
        - [使用最多的数据库，对他们的理解？](#使用最多的数据库对他们的理解)
        - [编写过哪些爬虫中间件？](#编写过哪些爬虫中间件)
        - [“极验”滑动验证码如何破解？](#极验滑动验证码如何破解)
        - [爬虫多久爬一次，爬下来的数据使用哪个数据库存储数据，是怎么存储，为什么，部署是你做的吗？怎么部署？](#爬虫多久爬一次爬下来的数据使用哪个数据库存储数据是怎么存储为什么部署是你做的吗怎么部署)
        - [cookie过期的处理问题？](#cookie过期的处理问题)
        - [动态加载又对及时性要求很高怎么处理？](#动态加载又对及时性要求很高怎么处理)
        - [HTTPS有什么优点和缺点？](#https有什么优点和缺点)
        - [HTTPS是如何实现安全传输数据的？](#https是如何实现安全传输数据的)
        - [TTL，MSL，RTT各是什么？](#ttlmslrtt各是什么)
        - [平常怎么使用代理的 ？](#平常怎么使用代理的-)
        - [存放在数据库(redis、mysql等)。](#存放在数据库redismysql等)
        - [怎么监控爬虫的状态?](#怎么监控爬虫的状态)
        - [爬取数据的影响因素？](#爬取数据的影响因素)
        - [scrapy和requests的使用情况？](#scrapy和requests的使用情况)
        - [描述下scrapy框架运行的机制？](#描述下scrapy框架运行的机制)
        - [谈谈你对Scrapy的理解？](#谈谈你对scrapy的理解)
        - [怎么样让scrapy框架发送一个post请求（具体写出来）](#怎么样让scrapy框架发送一个post请求具体写出来)
        - [怎么监控爬虫的状态 ？](#怎么监控爬虫的状态-)
        - [怎么判断网站是否更新？](#怎么判断网站是否更新)
        - [图片、视频爬取怎么绕过防盗连接](#图片视频爬取怎么绕过防盗连接)
        - [你爬出来的数据量大概有多大？大概多长时间爬一次？](#你爬出来的数据量大概有多大大概多长时间爬一次)
        - [增量爬取](#增量爬取)
        - [爬取下来的数据如何去重，说一下scrapy的具体的算法依据。](#爬取下来的数据如何去重说一下scrapy的具体的算法依据)
        - [Scrapy的优缺点?](#scrapy的优缺点)
        - [怎么设置爬取深度？](#怎么设置爬取深度)
        - [scrapy和scrapy-redis有什么区别？为什么选择redis数据库？](#scrapy和scrapy-redis有什么区别为什么选择redis数据库)
            - [区别](#区别-1)
            - [为什么会选择redis数据库？](#为什么会选择redis数据库)
        - [分布式爬虫主要解决什么问题？](#分布式爬虫主要解决什么问题)
        - [什么是分布式存储？](#什么是分布式存储)
        - [你所知道的分布式爬虫方案有哪些？](#你所知道的分布式爬虫方案有哪些)
        - [scrapy-redis，有做过其他的分布式爬虫吗？](#scrapy-redis有做过其他的分布式爬虫吗)
- [数据库](#数据库)
    - [MySQL](#mysql)
        - [主键 超键 候选键 外键](#主键-超键-候选键-外键)
        - [视图的作用，视图可以更改么？](#视图的作用视图可以更改么)
        - [drop,delete与truncate的区别](#dropdelete与truncate的区别)
        - [索引的工作原理及其种类](#索引的工作原理及其种类)
        - [连接的种类](#连接的种类)
        - [数据库优化的思路](#数据库优化的思路)
        - [存储过程与触发器的区别](#存储过程与触发器的区别)
        - [悲观锁和乐观锁是什么？](#悲观锁和乐观锁是什么)
        - [你常用的mysql引擎有哪些?各引擎间有什么区别?](#你常用的mysql引擎有哪些各引擎间有什么区别)
        - [Mysql怎么限制IP访问？](#mysql怎么限制ip访问)
    - [Redis](#redis)
        - [Redis宕机怎么解决?](#redis宕机怎么解决)
        - [redis和mecached的区别，以及使用场景](#redis和mecached的区别以及使用场景)
            - [区别](#区别-2)
            - [使用场景](#使用场景)
        - [Redis支持哪几种持久化方式](#redis支持哪几种持久化方式)
            - [RDB持久化](#rdb持久化)
            - [AOF（append only file）持久化](#aofappend-only-file持久化)
            - [Redis两种持久化方式优缺点？](#redis两种持久化方式优缺点)
        - [如何选择Redis持久化方式策略？](#如何选择redis持久化方式策略)
        - [Redis集群方案该怎么做?都有哪些方案?](#redis集群方案该怎么做都有哪些方案)
        - [Redis如何做内存优化](#redis如何做内存优化)
        - [Redis回收进程是如何工作的](#redis回收进程是如何工作的)
    - [RabbitMQ](#rabbitmq)
    - [MongoDB](#mongodb)
        - [MongoDB中对多条记录做更新操作命令是什么？](#mongodb中对多条记录做更新操作命令是什么)
        - [MongoDB如何才会拓展到多个shard里？](#mongodb如何才会拓展到多个shard里)
    - [测试](#测试)
        - [编写测试计划的目的是](#编写测试计划的目的是)
        - [对关键词触发模块进行测试](#对关键词触发模块进行测试)
        - [其他常用笔试题目网址汇总](#其他常用笔试题目网址汇总)
        - [测试人员在软件开发过程中的任务是什么](#测试人员在软件开发过程中的任务是什么)
        - [一条软件Bug记录都包含了哪些内容？](#一条软件bug记录都包含了哪些内容)
        - [简述黑盒测试和白盒测试的优缺点](#简述黑盒测试和白盒测试的优缺点)
        - [请列出你所知道的软件测试种类，至少5项](#请列出你所知道的软件测试种类至少5项)
        - [Alpha测试与Beta测试的区别是什么？](#alpha测试与beta测试的区别是什么)
        - [举例说明什么是Bug？一个bug report应包含什么关键字？](#举例说明什么是bug一个bug-report应包含什么关键字)
    - [数据结构](#数据结构)
        - [数组中出现次数超过一半的数字-Python版](#数组中出现次数超过一半的数字-python版)
        - [求100以内的质数](#求100以内的质数)
        - [无重复字符的最长子串-Python实现](#无重复字符的最长子串-python实现)
        - [通过2个5和6升得水壶从池塘得到3升水](#通过2个5和6升得水壶从池塘得到3升水)
        - [什么是MD5加密，有什么特点？](#什么是md5加密有什么特点)
        - [什么是对称加密和非对称加密](#什么是对称加密和非对称加密)
        - [冒泡排序的思想？](#冒泡排序的思想)
        - [快速排序的思想？](#快速排序的思想)
        - [如何判断单向链表中是否有环？](#如何判断单向链表中是否有环)
        - [你知道哪些排序算法（一般是通过问题考算法）](#你知道哪些排序算法一般是通过问题考算法)
        - [斐波那契数列](#斐波那契数列)
        - [如何翻转一个单链表？](#如何翻转一个单链表)
        - [青蛙跳台阶问题](#青蛙跳台阶问题)
        - [两数之和Two Sum](#两数之和two-sum)
        - [搜索旋转排序数组(Search in Rotated Sorted Array)](#搜索旋转排序数组search-in-rotated-sorted-array)
        - [Python实现一个Stack的数据结构](#python实现一个stack的数据结构)
        - [写一个二分查找](#写一个二分查找)
        - [set用in时间复杂度是多少，为什么？](#set用in时间复杂度是多少为什么)
        - [列表中有n个正整数范围在[0，1000]，进行排序](#列表中有n个正整数范围在01000进行排序)
        - [面向对象编程中有组合和继承的方法实现新的类](#面向对象编程中有组合和继承的方法实现新的类)
    - [大数据](#大数据)
        - [找出1G的文件中高频词](#找出1g的文件中高频词)
        - [一个大约有一万行的文本文件统计高频词](#一个大约有一万行的文本文件统计高频词)
        - [怎么在海量数据中找出重复次数最多的一个？](#怎么在海量数据中找出重复次数最多的一个)
        - [判断数据是否在大量数据中](#判断数据是否在大量数据中)
        - [事务的ACID](#事务的acid)
    - [机器学习和深度学习](#机器学习和深度学习)

<!-- /TOC -->
# Python基础
## 文件操作
### 有一个jsonline格式的文件file.txt大小约为10K
```python
def get_lines():
    with open('file.txt','rb') as f:
        return f.readlines()

if __name__ == '__main__':
    for e in get_lines():
        process(e) # 处理每一行数据
```
现在要处理一个大小为10G的文件，但是内存只有4G，如果在只修改get_lines 函数而其他代码保持不变的情况下，应该如何实现？需要考虑的问题都有那些？
```python
def get_lines():
    with open('file.txt','rb') as f:
        for i in f:
            yield i
```
Pandaaaa906提供的方法
```python
from mmap import mmap

def get_lines(fp):
    with open(fp, "r+") as f:
        m = mmap(f.fileno(), 0)
        tmp = 0
        for i, char in enumerate(m):
            if char == b"\n":
                yield m[tmp:i+1].decode()
                tmp = i + 1

if __name__=="__main__":
    for i in get_lines("fp_some_huge_file"):
        print(i)
```
要考虑的问题有：内存只有4G无法一次性读入10G文件，需要分批读入分批读入数据要记录每次读入数据的位置。分批每次读取数据的大小，太小会在读取操作花费过多时间。具体可以参考[此处](https://stackoverflow.com/questions/30294146/python-fastest-way-to-process-large-file)

### 文件路径
1. 打印输出当前文件所在目录路径
    ```Python
    import os
    print(os.path.dirname(os.path.abspath(__file__)))
    ```
2. 打印输出当前文件路径
    ```Python
    import os
    print(os.path.abspath(__file__))
    ```
3. 打印输出当前文件上两层文件目录路径
    ```Python
    import os
    print(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
    ```

### 补充缺失的代码
```python
def print_directory_contents(sPath):
"""
这个函数接收文件夹的名称作为输入参数
返回该文件夹中文件的路径
以及其包含文件夹中文件的路径
"""
import os
for s_child in os.listdir(s_path):
    s_child_path = os.path.join(s_path, s_child)
    if os.path.isdir(s_child_path):
        print_directory_contents(s_child_path)
    else:
        print(s_child_path)
```
## 模块与包
### 列出5个python标准库
**os：** 提供了不少与操作系统相关联的函数
**sys:** 通常用于命令行参数
**re:** 正则匹配
**math:** 数学运算
**datetime:** 处理日期时间

### 输入日期， 判断这一天是这一年的第几天？
```python
import datetime
def dayofyear():
    year = input("请输入年份: ")
    month = input("请输入月份: ")
    day = input("请输入天: ")
    date1 = datetime.date(year=int(year), month=int(month), day=int(day))
    date2 = datetime.date(year=int(year), month=1, day=1)
    return (date1 - date2).days + 1
```
### 打乱一个排好序的list对象alist？
```python
import random
alist = [1,2,3,4,5]
random.shuffle(alist)
print(alist)
```
## 数据类型
### python常见的列表推导式？
```Python
d = [val for value in iterable]
```
### 现有字典 d= {'a':24,'g':52,'i':12,'k':33}请按value值进行排序?
```python
sorted(d.items(), key=lambda x:x[1])
```
### 字典推导式
```python
d = {key:value for (key, value) in iterable}
```
### 请反转字符串 "aStr"?
```python
print("aStr"[::-1])
```
### 将字符串 "k:1|k1:2|k2:3|k3:4"，处理成字典 {k:1,k1:2,...}
```python
str1 = "k:1|k1:2|k2:3|k3:4"
def str2dict(str1):
    dict1 = {}
    for iterms in str1.split('|'):
        key,value = iterms.split(':')
        dict1[key] = value
    return dict1
#字典推导式
d = {k:int(v) for t in str1.split("|") for k, v in (t.split(":"), )}
```
### 请按alist中元素的age由大到小排序
```python
alist = [{'name':'a','age':20},{'name':'b','age':30},{'name':'c','age':25}]
def sort_by_age(list1):
    return sorted(alist, key=lambda x:x['age'], reverse=True)
```
### 下面代码的输出结果将是什么？
```python
list = ['a','b','c','d','e']
print(list[10:])
```
代码将输出[],不会产生IndexError错误，就像所期望的那样，尝试用超出成员的个数的index来获取某个列表的成员。例如，尝试获取list[10]和之后的成员，会导致IndexError。然而，尝试获取列表的切片，开始的index超过了成员个数不会产生IndexError，而是仅仅返回一个空列表。这成为特别让人恶心的疑难杂症，因为运行的时候没有错误产生，导致Bug很难被追踪到。
### 写一个列表生成式，产生一个公差为11的等差数列
```python
print([x*11 for x in range(10)])
```
### 给定两个列表，怎么找出他们相同的元素和不同的元素？
```python
list1 = [1,2,3]
list2 = [3,4,5]
set1 = set(list1)
set2 = set(list2)
print(set1 & set2)
print(set1 ^ set2)
```
### 请写出一段python代码实现删除list里面的重复元素？
```python
l1 = ['b','c','d','c','a','a']
l2 = list(set(l1))
print(l2)
```
用list类的sort方法:
```python
l1 = ['b','c','d','c','a','a']
l2 = list(set(l1))
l2.sort(key=l1.index)
print(l2)
```
也可以这样写:
```python
l1 = ['b','c','d','c','a','a']
l2 = sorted(set(l1), key=l1.index)
print(l2)
```
也可以用遍历：
```python
l1 = ['b','c','d','c','a','a']
l2 = []
for i in l1:
    if not i in l2:
        l2.append(i)
print(l2)
```

### Python中生成随机整数、随机小数、0--1之间小数方法
**随机整数：** random.randint(a,b),生成区间内的整数

**随机小数：** 习惯用numpy库，利用np.random.randn(5)生成5个随机小数

**0-1随机小数：** random.random(),括号中不传参

### Python中断言方法举例
**assert()** 方法，断言成功，则程序继续执行，断言失败，则程序报错

## 企业面试题
### python2和python3区别？列举5个
1. Python3中使用`print`必须要以小括号包裹打印内容，比如print('hi')
Python2中既可以使用带小括号的方式，也可以使用一个空格来分隔打印内容，比如print 'hi'
2. python2中range(1,10)返回列表，python3中返回迭代器，节约内存
3. python2中使用ascii编码，python中使用utf-8编码
4. python2中unicode表示字符串序列，str表示字节序列,python3中str表示字符串序列，byte表示字节序列
5. python2中为正常显示中文，引入coding声明，python3中不需要
6. python2中是raw_input()函数，python3中是input()函数

### python新式类和经典类的区别？
1. 在python里凡是继承了object的类，都是新式类
2. Python3里只有新式类
3. Python2里面继承object的是新式类，没有写父类的是经典类
4. 经典类目前在Python里基本没有应用

### python中内置的数据结构有几种？
1. 整型 int、 长整型 long、浮点型 float、 复数 complex
2. 字符串 str、 列表 list、 元组 tuple
3. 字典 dict 、 集合 set
4. Python3 中没有 long，只有无限精度的 int

### 可变类型和不可变类型
1. 可变类型有list,dict.不可变类型有string，number,tuple.
2. 当进行修改操作时，可变类型传递的是内存中的地址，也就是说，直接修改内存中的值，并没有开辟新的内存。
3. 不可变类型被改变时，并没有改变原内存地址中的值，而是开辟一块新的内存，将原地址中的值复制过去，对这块新开辟的内存中的值进行操作。

### python如何实现单例模式?请写出两种实现方式?
第一种方法:使用装饰器
```python
def singleton(cls):
    instances = {}
    def wrapper(*args, **kwargs):
        if cls not in instances:
            instances[cls] = cls(*args, **kwargs)
        return instances[cls]
    return wrapper
    
@singleton
class Foo(object):
    pass
foo1 = Foo()
foo2 = Foo()
print(foo1 is foo2) #True
```
第二种方法：使用基类
**New**是真正创建实例对象的方法，所以重写基类的new方法，以此保证创建对象的时候只生成一个实例
```python
class Singleton(object):
    def __new__(cls, *args, **kwargs):
        if not hasattr(cls, '_instance'):
            cls._instance = super(Singleton, cls).__new__(cls, *args, **kwargs)
        return cls._instance
    
class Foo(Singleton):
    pass

foo1 = Foo()
foo2 = Foo()

print(foo1 is foo2) #True
```
第三种方法：元类
元类是用于创建类对象的类，类对象创建实例对象时一定要调用call方法，因此在调用call时候保证始终只创建一个实例即可，type是python的元类
```python
class Singleton(type):
    def __call__(cls, *args, **kwargs):
        if not hasattr(cls,'_instance'):
            cls._instance = super(Singleton,cls).__call__(*args,**kwargs)
        return cls._instance
```
```python
class Foo(object):
    __metaclass__ = Singleton

foo1 = Foo()
foo2 = Foo()
print(foo1 is foo2) #True

```
### 反转一个整数，例如-123 --> -321 
```python
class Solution(object):
    def reverse(self, x):
        if -10 < x < 10:
            return x
        str_x = str(x)
        if str_x[0] != "-":
            str_x = str_x[::-1]
            x = int(str_x)
        else:
            str_x = str_x[1:][::-1]
            x = int(str_x)
            x = -x
        return x if -2147483648 < x < 2147483647 else 0
if __name__ == '__main__':
    s = Solution()
    reverse_int = s.reverse(-120)
    print(reverse_int)
```
### 设计实现遍历目录与子目录，抓取.pyc文件
第一种方法：
```python
import os

def get_files(dir, suffix):
    res = []
    for root,dirs,files in os.walk(dir):
        for filename in files:
            name,suf = os.path.splitext(filename)
            if suf == suffix:
                res.append(os.path.join(root,filename))
    print(res)

get_files("./",'.pyc')
```
第二种方法：
```python
import os

def pick(obj):
    if ob.endswith(".pyc"):
        print(obj)
    
def scan_path(ph):
    file_list = os.listdir(ph)
    for obj in file_list:
        if os.path.isfile(obj):
            pick(obj)
        elif os.path.isdir(obj):
            scan_path(obj)
    
if __name__=='__main__':
    path = input('输入目录')
    scan_path(path)
```
第三种方法
```python
from glob import iglob

def func(fp, postfix):
    for i in iglob(f"{fp}/**/*{postfix}", recursive=True):
        print(i)

if __name__ == "__main__":
    postfix = ".pyc"
    func("K:\Python_script", postfix)
```
### 一行代码实现1-100之和
```python
count = sum(range(0, 101))
print(count)
```
### Python-遍历列表时删除元素的正确做法
遍历在新在列表操作，删除时在原来的列表操作
```python
a = [1,2,3,4,5,6,7,8]
print(id(a))
print(id(a[:]))
for i in a[:]:
    if i>5:
        pass
    else:
        a.remove(i)
    print(a)
print('-----------')
print(id(a))

```
```python
#filter
a=[1,2,3,4,5,6,7,8]
b = filter(lambda x: x > 5, a)
print(list(b))
```
列表解析
```python
a=[1,2,3,4,5,6,7,8]
b = [i for i in a if i>5]
print(b)
```
倒序删除
因为列表总是‘向前移’，所以可以倒序遍历，即使后面的元素被修改了，还没有被遍历的元素和其坐标还是保持不变的
```python
a=[1,2,3,4,5,6,7,8]
print(id(a))
for i in range(len(a)-1,-1,-1):
    if a[i]>5:
        pass
    else:
        a.remove(a[i])
print(id(a))
print('-----------')
print(a)
```

### 字符串的操作题目
全字母短句 PANGRAM 是包含所有英文字母的句子，比如：A QUICK BROWN FOX JUMPS OVER THE LAZY DOG. 定义并实现一个方法 get_missing_letter, 传入一个字符串采纳数，返回参数字符串变成一个 PANGRAM 中所缺失的字符。应该忽略传入字符串参数中的大小写，返回应该都是小写字符并按字母顺序排序（请忽略所有非 ACSII 字符）

**下面示例是用来解释，双引号不需要考虑:**

(0)输入: "A quick brown for jumps over the lazy dog"

返回： ""

(1)输入: "A slow yellow fox crawls under the proactive dog" 

返回: "bjkmqz"

(2)输入: "Lions, and tigers, and bears, oh my!"

返回: "cfjkpquvwxz" 

(3)输入: ""

返回："abcdefghijklmnopqrstuvwxyz"

```python
def get_missing_letter(a):
    s1 = set("abcdefghijklmnopqrstuvwxyz")
    s2 = set(a)
    ret = "".join(sorted(s1-s2))
    return ret
    
print(get_missing_letter("python"))
```

### is和==有什么区别？
**is：** 比较的是两个对象的id值是否相等，也就是比较俩对象是否为同一个实例对象。是否指向同一个内存地址
**==:** 比较的两个对象的内容/值是否相等，默认会调用对象的eq()方法
### 求出列表所有奇数并构造新列表
```python
a = [1,2,3,4,5,6,7,8,9,10]
res = [ i for i in a if i % 2 == 1]
print(res)
```
### 用一行python代码写出1+2+3+10248
```python
#1.使用sum内置求和函数
num = sum([1,2,3,10248])
print(num)
#2.reduce 函数
from functools import reduce
num1 = reduce(lambda x, y : x + y, [1,2,3,10248])
print(num1)
```
### Python中变量的作用域？（变量查找顺序)
1.什么是LEGB及其函数作用域的LEGB顺序?
**L：** local 函数内部作用域
**E:** enclosing 函数内部与内嵌函数之间
**G:** global 全局作用域
**B：** build-in 内置作用

python在函数里面的查找分为4种，称之为LEGB，也正是按照这是顺序来查找的
### 字符串 `"123"` 转换成 `123`，不使用内置api，例如 `int()`
方法一： 利用 `str` 函数
```python
def atoi(s):
    num = 0
    for v in s:
        for j in range(10):
            if v == str(j):
                num = num * 10 + j
    return num
```
方法二： 利用 `ord` 函数
```python
def atoi(s):
    num = 0
    for v in s:
        num = num * 10 + ord(v) - ord('0')
    return num
```
方法三: 利用 `eval` 函数
```python
def atoi(s):
    num = 0
    for v in s:
        t = "%s * 1" % v
        n = eval(t)
        num = num * 10 + n
    return num
```
方法四: 结合方法二，使用 `reduce`，一行解决
```python
from functools import reduce
def atoi(s):
    return reduce(lambda num, v: num * 10 + ord(v) - ord('0'), s, 0)
```
### 给定一个整数数组和一个目标值，找出数组中和为目标值的两个数
你可以假设每个输入只对应一种答案，且同样的元素不能被重复利用。示例:给定nums = [2,7,11,15],target=9 因为 nums[0]+nums[1] = 2+7 =9,所以返回[0,1]
```python
class Solution:
    def twoSum(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: List[int]
        """
        d = {}
        size = 0
        while size < len(nums):
            if target - nums[size] in d:
                if d[target - nums[size]] < size:
                    return [d[target-nums[size]], size]
                else:
                    d[nums[size]] = size
                size = size + 1
solution = Solution()
list = [2,7,11,15]
target = 9
nums = solution.twoSum(list,target)
print(nums)
```

### 给列表中的字典排序
假设有如下list对象，alist=[{"name":"a","age":20},{"name":"b","age":30},{"name":"c","age":25}],将alist中的元素按照age从大到小排序 alist=[{"name":"a","age":20},{"name":"b","age":30},{"name":"c","age":25}]
```python
alist_sort = sorted(alist, key=lambda e : e.__getitem__('age'), reverse=True)
```

### 统计一个文本中单词频次最高的10个单词？
```python
import re

# 方法一
def test(filepath):
    
    distone = {}
    with open(filepath) as f:
        for line in f:
            line = re.sub("\W+", " ", line)
            lineone = line.split()
            for keyone in lineone:
                if not distone.get(keyone):
                    distone[keyone] = 1
                else:
                    distone[keyone] += 1
    num_ten = sorted(distone.items(), key=lambda x:x[1], reverse=True)[:10]
    num_ten =[x[0] for x in num_ten]
    return num_ten
    
 
# 方法二 
# 使用 built-in 的 Counter 里面的 most_common
import re
from collections import Counter

def test2(filepath):
    with open(filepath) as f:
        return list(map(lambda c: c[0], Counter(re.sub("\W+", " ", f.read()).split()).most_common(10)))
```

### 利用collections库的Counter方法统计字符串每个单词出现的次数"kjalfj;ldsjafl;hdsllfdhg;lahfbl;hl;ahlf;h"
```Python
from collections import Counter
a = "kjalfj;ldsjafl;hdsllfdhg;lahfbl;hl;ahlf;h"
res = Counter(a)
print(res)
```

### 请写出一个函数满足以下条件
该函数的输入是一个仅包含数字的list,输出一个新的list，其中每一个元素要满足以下条件：
1、该元素是偶数
2、该元素在原list中是在偶数的位置(index是偶数)

```python
def num_list(num):
    return [i for i in num if i % 2 == 0 and num.index(i) % 2 == 0]

num = [0,1,2,3,4,5,6,7,8,9,10]
result = num_list(num)
print(result)
```
### 使用单一的列表生成式来产生一个新的列表
该列表只包含满足以下条件的值，元素为原始列表中偶数切片
```python
list_data = [1,2,5,8,10,3,18,6,20]
res = [x for x in list_data[::2] if x % 2 == 0]
print(res)
```
### 用一行代码生成[1,4,9,16,25,36,49,64,81,100]
```python
[x * x for x in range(1, 11)]
```
### 输入某年某月某日，判断这一天是这一年的第几天？
```python
import datetime

y = int(input("请输入4位数字的年份:"))
m = int(input("请输入月份:"))
d = int(input("请输入是哪一天"))

targetDay = datetime.date(y, m, d)
dayCount = targetDay - datetime.date(targetDay.year - 1, 12, 31)
print("%s是 %s年的第%s天。"%(targetDay, y, dayCount.days))
```
### 两个有序列表，l1、l2对这两个列表进行合并不可使用extend
```python
def loop_merge_sort(l1, l2):
    tmp = list()
    while len(l1) > 0 and len(l2) > 0:
        if l1[0] < l2[0]:
            tmp.append(l1[0])
            del l1[0]
        else:
            tmp.append(l2[0])
            del l2[0]
    
    if len(l1) > 0:
        while len(l1):
            tmp.append(l1[0])
            del l1[0]

    if len(l2) > 0:
        while len(l2) > 0:
            tmp.append(l2[0])
            del l2[0]
    return tmp
```
### 给定一个任意长度数组，实现一个函数
让所有奇数都在偶数前面，而且奇数升序排列，偶数降序排序，如字符串'1982376455',变成'1355798642'
```python
# 方法一
def func1(l):
    if isinstance(l, str):
        l = [int(i) for i in l]

    l.sort(reverse=True)

    for i in range(len(l)):
        if l[i] % 2 > 0:
            l.insert(0, l.pop(i))
    print(''.join(str(e) for e in l))

# 方法二
def func2(l):
    print("".join(sorted(l, key=lambda x: int(x) % 2 == 0 and 20 - int(x) or int(x))))
```
### 写一个函数找出一个整数数组中，第二大的数
```python
def find_second_large_num(num_list):
    """
    找出数组第2大的数字
    """
    # 方法一
    # 直接排序，输出倒数第二个数即可
    tmp_list = sorted(num_list)
    print("方法一\nSecond_large_num is :", tmp_list[-2])
    
    # 方法二
    # 设置两个标志位一个存储最大数一个存储次大数
    # two 存储次大值，one 存储最大值，遍历一次数组即可，先判断是否大于 one，若大于将 one 的值给 two，将 num_list[i] 的值给 one，否则比较是否大于two，若大于直接将 num_list[i] 的值给two，否则pass
    one = num_list[0]
    two = num_list[0]
    for i in range(1, len(num_list)):
        if num_list[i] > one:
            two = one
            one = num_list[i]
        elif num_list[i] > two:
            two = num_list[i]
    print("方法二\nSecond_large_num is :", two)
    
    # 方法三
    # 用 reduce 与逻辑符号 (and, or)
    # 基本思路与方法二一样，但是不需要用 if 进行判断。
    from functools import reduce
    num = reduce(lambda ot, x : ot[1] < x and (ot[1], x) or ot[0] < x and (x, ot[1]) or ot, num_list, (0, 0))[0]
    print("方法三\nSecond_large_num is :", num)
    
if __name__ == '__main___':
    num_list = [34, 11, 23, 56, 78, 0, 9, 12, 3, 7, 5]
    find_second_large_num(num_list)
```
### 阅读一下代码他们的输出结果是什么？
```python
def multi():
    return [lambda x : i * x for i in range(4)]
print([m(3) for m in multi()])
```
正确答案是[9,9,9,9]，而不是[0,3,6,9]产生的原因是Python的闭包的后期绑定导致的，这意味着在闭包中的变量是在内部函数被调用的时候被查找的，因为，最后函数被调用的时候，for循环已经完成, i 的值最后是3,因此每一个返回值的i都是3,所以最后的结果是[9,9,9,9]
### 统计一段字符串中字符出现的次数
```python
# 方法一
def count_str(str_data):
    """定义一个字符出现次数的函数"""
    dict_str = dict()
    for i in str_data:
        dict_str[i] = dict_str.get(i, 0) + 1
    return dict_str
dict_str = count_str("AAABBCCAC")
str_count_data = ""
for k, v in dict_str.items():
    str_count_data += k + str(v)
print(str_count_data)

# 方法二
from collections import Counter
print("".join(map(lambda x: x[0] + str(x[1]), Counter("AAABBCCAC").most_common())))
```
### super函数的具体用法和场景
1. 为了调用父类(超类)的一个方法，可以使用super()函数
2. super()函数的一个常见用法是在 `__init__()`方法中确保父类被正确的初始化
3. super()的另外一个常见用法出现在覆盖Python特殊方法的代码中
具体详见[调用父类方法](https://python3-cookbook.readthedocs.io/zh_CN/latest/c08/p07_calling_method_on_parent_class.html)
# Python高级
## 元类
### Python中类方法、类实例方法、静态方法有何区别？
* 类方法: 是类对象的方法，在定义时需要在上方使用`@classmethod`进行装饰,形参为cls，表示类对象，类对象和实例对象都可调用
* 类实例方法: 是类实例化对象的方法,只有实例对象可以调用，形参为self,指代对象本身;
* 静态方法: 是一个任意函数，在其上方使用`@staticmethod`进行装饰，可以用对象直接调用，静态方法实际上跟该类没有太大关系
### 遍历一个object的所有属性，并print每一个属性名？
```python
class Car:
    def __init__(self, name, loss): # loss [价格，油耗，公里数]
        self.name = name
        self.loss = loss
    
    def get_name(self):
        return self.name
    
    def get_price(self):
        # 获取汽车价格
        return self.loss[0]
    
    def get_loss(self):
        # 获取汽车损耗值
        return self.loss[1] * self.loss[2]

Bmw = Car("宝马", [60,9,500]) # 实例化一个宝马车对象
print(getattr(Bmw,"name")) # 使用getattr()传入对象名字,属性值。
print(dir(Bmw)) # 获Bmw所有的属性和方法
```
### 写一个类，并让它尽可能多的支持操作符?
```python
class Array:
    __list = []
    
    def __init__(self):
        print "constructor"
    
    def __del__(self):
        print "destruct"
    
    def __str__(self):
        return "this self-defined array class"

    def __getitem__(self,key):
        return self.__list[key]
    
    def __len__(self):
        return len(self.__list)

    def Add(self, value):
        self.__list.append(value)
    
    def Remove(self, index):
        del self.__list[index]
    
    def DisplayItems(self):
        print "show all items---"
        for item in self.__list:
            print item
```
### 提高python运行效率的方法
1. 使用生成器，因为可以节约大量内存
2. 循环代码优化，避免过多重复代码的执行
3. 核心模块用Cython、PyPy等，提高效率
4. 多进程、多线程、协程
5. 多个if elif条件判断，可以把最有可能先发生的条件放到前面写，这样可以减少程序判断的次数，提高效率

### 介绍Cython、Pypy、CPython、Numba各有什么缺点
python程序性能优化的套路一般有两种：1）jit， 即just in time compiler， 即时编译器，在运行时将某些函数编译成二进程代码，使用这种方式的有：numba 和pypy；2）将python代码转换成c++/c代码，然后编译执行，这种方式有：cython和nuitka。总而言之，转换成c++/c代码以后编译成二进制文件执行的效率比用numba和pypy即时编译执行的效率要高
1. Cython
    Cython（Python的C语言扩展）是Python的超集，它能把Python代码编译成C代码，并与C和C++进行交互。它可以作为Python项目的扩展使用（重新性能要求高的部分），或者单独使用，不涉及传统的Python代码。缺点是你写的不是Python，所以需要手动迁移，缺乏可移植性。
    
    据说，Cython提供了一些特性来让代码更高效，比如变量类型化，这本质上是C要求的。一些科学计算的包，如scikit-learn依赖Cython的一些特性来保持操作简洁快速。

2. Pypy
    在CPython的替代品中，PyPy是最显眼的那一个（比如Quora就在生产环境中使用它）。它也最有机会成为默认解释器，它和现存Python代码高度兼容。

    PyPy使用适时编译来加速Python，这项技术Google也在使用，Google在V8引擎中使用它加速Javascript。最近的版本PyPy2.5增加了一些提升性能的特性，其中有一项很受欢迎，它集成了Numpy，Numpy之前也一直被用来加速Python的运行。

    使用Python3的代码需要对应地使用PyPy3。PyPy目前只支持到Python3.2.5，对Python3.3的支持正在进行中。

3. CPython
    CPython是特指C语言实现的Python，就是原汁原味的Python。
    
    之所以使用CPython这个词，是因为Python还有一些其它的实现，比如Jython，就是Java版的Python，还有烧脑的PyPy，使用Python再把Python实现了一遍。
    
    如下是官方对CPython的说明：
    CPython is Guido van Rossum’s reference version of the Python computing language. It’s most often called simply “Python”; speakers say “CPython” generally to distinguish it explicitly from other implementations.
    
4. Numba
    Numba接合了上面几个项目的想法。学习了Cython，Numba也采用了部分加速的策略，只加速CPU密集型的任务；同时它又学习了PyPy和Pyston，通过LLVM运行Python。你可以用一个装饰器指定你要用Numba编译的函数，Numba继承Numpy来加速函数的执行，Numba不做适时编译，它的代码是预先编译的。

Python之父说大部分觉得Python慢的应用都是没有正确地使用Python。对于CPU密集型的任务有多种方法来提升性能--使用Numpy来做计算，调用外部C代码，以及尽量避免GIL锁。由于GIL锁目前还无法被替代，所以有很多项目开始尝试一些短期可行的替代方案，当然这些方案也可能转变为长期的可选项。

### 请描述抽象类和接口类的区别和联系
使用`abc`模块可以很轻松的定义抽象基类：
抽象类的一个特点是它不能直接被实例化
抽象类的目的就是让别的类继承它并实现特定的抽象方法
抽象基类的一个主要用途是在代码中检查某些类是否为特定类型，实现了特定接口
除了继承这种方式外，还可以通过注册方式来让某个类实现抽象基类
```python
import abc
```
具体请看[此处](https://python3-cookbook.readthedocs.io/zh_CN/latest/c08/p12_define_interface_or_abstract_base_class.html)

### Python中如何动态获取和设置对象的属性？
dir([obj]):调用这个方法将返回包含obj大多数属性名的列表（会有一些特殊的属性不包含在内）。obj的默认值是当前的模块对象。
hasattr(obj, attr): 这个方法用于检查obj是否有一个名为attr的值的属性，返回一个布尔值。
getattr(obj, attr): 调用这个方法将返回obj中名为attr值的属性的值，例如如果attr为’bar’，则返回obj.bar。
setattr(obj, attr, val):调用这个方法将给obj的名为attr的值的属性赋值为val。例如如果attr为’bar’，则相当于obj.bar = val。

## 内存管理与垃圾回收机制
### 哪些操作会导致Python内存溢出，怎么处理？
内存溢出:你申请了10个字节的内存,但写入了大于10个字节的数据会导致内存溢出

**内存溢出原因：**
1. 内存中加载的数据量过于庞大，如一次从数据库取出过多数据；
2. 集合类中有对对象的引用，使用完后未清空，产生了堆积，使得JVM不能回收；
3. 代码中存在死循环或循环产生过多重复的对象实体；
4. 使用的第三方软件中的BUG；
5. 启动参数内存值设定的过小
**内存溢出的解决方案：** 
1. 修改JVM启动参数，直接增加内存。(-Xms，-Xmx参数一定不要忘记加。)
2. 检查错误日志，查看“OutOfMemory”错误前是否有其 它异常或错误。
3. 对代码进行走查和分析，找出可能发生内存溢出的位置。

### 关于Python内存管理
**内存管理**包括:
* 变量无须事先声明
* 变量无须指定类型
* 不用关心内存管理
* 变量名会被"回收"
* del语句能够直接释放资源
**变量定义**
python中, 变量在第一次被赋值时自动声明, 和其它语言一样, 变量只有被创建和赋值后才能被使用
**动态类型**
变量名无须事先声明, 也无须类型声明
对象的类型和内存占用都是运行时确定的
**内存分配**
python解释器会自动进行内存管理, 不用开发人员去关心
**引用计数**
* 要保持追踪内存中的状态, python使用了引用计数, 就是python内部记录着所有使用中的对象各有多少引用.
* 一个内部跟踪变量, 称为一个引用计数器, 至于每个对象各有多少引用, 简称引用计数, 当对象被创建时, 就创建了一个引用计数, 当这个对象不再需要时, 也就是说, 这个对象的引用计数变为0时, 它被垃圾回收
**增加引用计数**
* 当对象被创建赋值给变量时, 该对象的引用计数就被设置为1
* 当同一个对象又被赋值给其他变量时, 或作为参数传递给函数, 方法或类实例时, 或者被赋值为一个窗口对象的成员时, 该对象的一个新的引用, 或者作为别名, 就被创建.
**减少引用计数**
当对象的引用被销毁时, 引用计数会减少, 明显的例子就是当引用离开其作用范围时, 这种情况最经常出现在函数运行结束时, 所有局部变量都被自动销毁, 对象的引用计数也就减少
**垃圾收集**
不再被使用的内存会被一种称为垃圾收集的机制释放
注: 解释器跟踪对象的引用计数, 垃圾回收机制负责释放内存, 垃圾收集器是一块独立代码, 它用来寻找引用计数为0的对象, 它也负责检查虽然引用计数大于0但是也应该被销毁的对象
引用语义: python中在变量里保存值(对象)的引用, 采用这种方式, 变量所需的存储空间大小一致, 因为其只需要保存一个引用
值语义变量的值直接保存在变量的存储区里, 这样一个整数类型的变量就需要保存一个整数所需的空间, 一个浮点数变量就需要足够的空间存储一个浮点数. C中就是值语义

### Python的内存管理与垃圾回收机机制及调优手段？
1. 内存管理机制：引用计数、垃圾回收、内存池。 
    **引用计数：** 引用计数是一种非常高效的内存管理手段，当一个python对象被引用时，它的引用计数增加1，当它不再被一个变量引用时则引用计数减1，当它的引用计数等于0时对象被删除
    **垃圾回收：** 当Python的某个对象的引用计数降为0时，说明没有任何引用指向该对象，该对象就成为要被回收的垃圾。比如某个新建对象，被分配给某个引用，对象的引用计数变为1。如果引用被删除，对象的引用计数为0，那么该对象就可以被垃圾回收。
    **内存池：** Python 的内存机制呈现金字塔形状，-1，-2 层主要有操作系统进行操作；
    * 第 0 层是 C 中的 malloc，free 等内存分配和释放函数进行操作；
    * 第 1 层和第 2 层是内存池，有 Python 的接口函数 PyMem_Malloc 函数实现，当对象小于256K 时有该层直接分配内存；
    * 第 3 层是最上层，也就是我们对 Python 对象的直接操作；

    Python 在运行期间会大量地执行 malloc 和 free 的操作，频繁地在用户态和核心态之间进行切换，这将严重影响 Python 的执行效率。为了加速 Python 的执行效率，Python 引入了一个内存池机制，用于管理对小块内存的申请和释放。

    Python 内部默认的小块内存与大块内存的分界点定在 256 个字节，当申请的内存小于 256 字节时，PyObject_Malloc 会在内存池中申请内存；当申请的内存大于 256 字节时，PyObject_Malloc 的行为将蜕化为 malloc 的行为。当然，通过修改 Python 源代码，我们可以改变这个默认值，从而改变 Python 的默认内存管理行为。

2. 调优手段：
    * 手动垃圾回收
    * 调高垃圾回收阈值
    * 避免循环引用(手动解循环引用和使用弱引用)

### 引用计数的优缺点
#### 优点：
1. 高效
2. 运行期没有停顿：一旦没有引用，内存就直接释放了。不用像其他机制等到特定时机。实时性还带来一个好处：处理回收内存的时间分摊到了平时。
3. 对象有确定的生命周期
4. 易于实现

#### 缺点:
1. 维护引用计数消耗资源，维护引用计数的次数和引用赋值成正比，而不像mark and sweep等基本与回收的内存数量有关。
2. 无法解决循环引用的问题。A和B相互引用而再没有外部引用A与B中的任何一个，它们的引用计数都为1，但显然应该被回收。

### 内存泄露是什么？如何避免？
内存泄露指由于疏忽或错误造成程序未能释放已经不再使用内存的情况。内存泄露并非指内存在物理上的消失，而是应用程序分配某段内存后，由于设计错误，失去了对该段内存的控制，因而造成了内存的浪费，导致运行速度缓慢甚至系统崩溃等严重后果。

**如何避免**
有_del_()函数的对象间的循环引用是导致内存泄露的主凶。
* 不使用一个对象式用del object来删除一个对象的引用计数就可以有效防止内存泄露问题。
* 通过Python扩展模块gc来查看不能回收的对象的详细信息
* 可以通过sys.getrefcount(obj)来获取对象的引用计数，并根据返回值是否为0来判断是否内存泄露

## 函数
### 简述read、readline、readlines的区别？
**read()：** 一次性读取整个文件内容。推荐使用read(size)方法，size越大运行时间越长
**readline()：** 每次读取一行内容。内存不够时使用，一般不太用
**readlines()：** 一次性读取整个文件内容，并按行返回到list，方便我们遍历
一般小文件我们都采用read()，不确定大小你就定个size，大文件就用readlines()

### 什么是Hash（散列函数）？
哈希函数（Hash Function），也称为散列函数，给定一个输入x，它会算出相应的输出H(x)。哈希函数的主要特征是：
* 输入x可以是任意长度的字符串
* 输出结果即H(x)的长度是固定的
* 计算H(x)的过程是高效的（对于长度为n的字符串x, 计算出H(x)的时间复杂度应为O(n)）

1. 免碰撞：即不会出现输入x≠y，但是H(x)=H(y) 的情况，其实这个特点在理论上并不成立，比如目前比特币使用的 SHA256 算法，会有 2^256 种输出，如果我们进行 2^256 + 1 次输入，那么必然会产生一次碰撞，事实上，通过 理论证明 ，通过 2^130 次输入就会有99%的可能性发生一次碰撞，不过即使如此，即便是人类制造的所有计算机自宇宙诞生开始一直运算到今天，发生一次碰撞的几率也是极其微小的。
2. 隐匿性：也就是说，对于一个给定的输出结果 H(x) ，想要逆推出输入 x ，在计算上是不可能的。如果想要得到 H(x) 的可能的原输入，不存在比穷举更好的方法。
hash 算法的原理是试图将一个空间的数据集映射到另外一个空间（通常比原空间要小），并利用质数将数据集能够均匀的映射。目前主流的 hash 算法有：md4、md5、sha系列。

### python函数重载机制？
通常不需要在Python中重载函数。Python是动态类型的，并支持函数的可选参数。

### 手写一个判断时间的装饰器
函数可以作为参数传递的语言，可以使用装饰器
```python
import datetime
class TimeException(Exception):
    def __init__(self, exception_info):
        super().__init__()
        self.info = exception_info

    def __str__(self):
        return self.info

def timecheck(func):
    def wrapper(*args, **kwargs):
        if datetime.datetime.now().year == 2019:
            func(*args, **kwargs)
        else:
            raise TimeException("函数已过时")

    return wrapper

@timecheck
def test(name):
    print("Hello {}, 2019 Happy".format(name))


if __name__ == "__main__":
    test("backbp")
```
### 编写函数的4个原则
1. 函数设计要尽量短小，嵌套层次不宜过深。避免过长函数，嵌套最好能控制在3层之内。
2. 函数申明应该合理，简单，易于使用。除函数名能够够正确反映其大体功能外，参数的设计也应该简洁明了，参数个数不宜太多。
3. 函数参数设计应该考虑向下兼容。可以通过加入默认参数来避免退化。
4. 一个函数只做一件事，就要尽量保证抽象层级的一致性，所有语句尽量在一个粒度上。若在一个函数中处理多件事，不利于代码的重用。
Python中函数设计的好习惯还包括，不要在函数中定义可变对象作为默认值，使用异常替换返回错误，保证通过单元测试等。

### 函数调用参数的传递方式是值传递还是引用传递？
Python中函数参数是引用传递（注意不是值传递）。对于不可变类型（数值型、字符串、元组），因变量不能修改，所以运算不会影响到变量自身；而对于可变类型（列表、字典）来说，函数体运算可能会更改传入的参数变量。

### 如何在function里面设置一个全局变量
函数内部global声明 修改全局变量

### 对缺省参数的理解？
缺省参数指在调用函数的时候没有传入参数的情况下，调用默认的参数，在调用函数的同时赋值时， 所传入的参数会替代默认参数。
**args**是不定长参数，他可以表示输入参数是不确定的，可以是任意多个。
**kwargs**是关键字参数，赋值的时候是以`key=value`的方式，参数是可以任意多对在定义函数的时候不确定会有多少参数会传入时，就可以使用两个参数。

### 带参数的装饰器?
函数可以作为参数传递的语言，可以使用装饰器

### 为什么函数名字可以当做参数用?
在实际使用中，我们有时希望将函数作为参数传递给另一个方法使用。
比如装饰器实际就是函数调用函数

如果要调用的方法的入参个数不确定，可以使用`*args`或`**args`。但是一定要把`*args`放到最后面

### Python中pass语句的作用是什么？
pass语句什么也不做，一般作为占位符或者创建占位程序，pass语句不会执行任何操作

### map函数和reduce函数？
**map()** 函数接收两个参数，一个是函数，一个是Iterable（可迭代对象），map将传入的函数依次作用到序列的每个元素，并把结果作为新的Iterator（迭代器）返回。 
**reduce()** 把一个函数作用在一个序列上，这个函数必须接收两个参数，reduce把结果继续和序列的下一个元素做累积计算

### 回调函数，如何通信的?
在计算机程序设计中，回调函数，或简称回调（Callback），是指通过函数参数传递到其它代码的，某一块可执行代码的引用。这一设计允许了底层代码调用在高层定义的子程序。

有两种类型的回调函数：即blocking callbacks (also known as synchronous callbacks or just callbacks) and deferred callbacks (also known as asynchronous callbacks).

那么，在python中如何实现回调函数呢，看代码
```Python
def my_callback(input):
    print "function my_callback was called with %s input" % (input,)
 
def caller(input, func):
    func(input)
 
for i in range(5):
    caller(i, my_callback)
```
来自[https://www.cnblogs.com/berlin-sun/p/callbackinpython.html](https://www.cnblogs.com/berlin-sun/p/callbackinpython.html)

### Python主要的内置数据类型都有哪些？ print(dir("a")) 的输出？
int:整型;
bool:布尔;
str:字符串;
list:列表;
tuple:元组;
dict:字典;
float 浮点型小数

输出字符串"a"的内建方法。

### hasattr()、getattr()、setattr()函数使用详解？
**hasattr(object, name)函数：** 判断一个对象里面是否有name 属性或者name 方法，返回bool 值，有name 属性(方法)返回True， 否则返回 False。
**getattr(object, name[,default]) 函数：** 获取对象 object 的属性或者方法，如果存在则打印出来，如果不存在，打印默认值，默认值可选。注意：如果返回的是对象的方法，则打印结果是：方法的内存地址，如果需要运行这个方法，可以在后面添加括号()。
**setattr(object,name,values)函数：** 给对象的属性赋值，若属性不存在，先创建再赋值

### 一句话解决阶乘函数？
```Python
def factorial(num):
    j = 1
    for i in range(1, num + 1):
        j = j * i
    print(j)

num = int(input("请输入阶乘数字："))
factorial(num)
reduce(lambda x, i : x * i, range(1, 100))
```

### Python 递归深度默认是多少？递归深度限制的原因是什么？
Python 递归深度可以用内置函数库中的`sys.getrecursionlimit()`查看。
因为无限递归会导致的C堆栈溢出和Python崩溃。

### 递归函数停止的条件？
递归的终止条件一般定义在递归函数内部，在递归调用前要做一个条件判断，根据判断的结果选择是继续调用自身，还是return; 返回终止递归。
**终止的条件：**
* 判断递归的次数是否达到某一限定值
* 判断运算的结果是否达到某个范围等，根据设计的目的来选择

### 什么是lambda函数？它有什么好处？写一个匿名函数求两个数的和
lambda函数是一个可以接收任意多个参数(包括可选参数)并且返回单个表达式值的匿名函数
**好处：**
1. lambda 函数比较轻便，即用即删除，很适合需要完成一项功能，但是此功能只在此一处使用，连名字都很随意的情况下；
2. 匿名函数，一般用来给filter、map这样的函数式编程服务;
3. 作为回调函数，传递给某些应用，比如消息处理

```python
from functools import reduce
reduce(lambda x, y : x + y, [2, 3])
```

## 设计模式
### 对设计模式的理解，简述你了解的设计模式？
设计模式是经过总结，优化的，对我们经常会碰到的一些编程问题的可重用解决方案。一个设计模式并不像一个类或一个库那样能够直接作用于我们的代码，反之，设计模式更为高级，它是一种必须在特定情形下实现的一种方法模板。
常见的是工厂模式和单例模式

### 请手写一个单例模式
[python如何实现单例模式?请写出两种实现方式?](#python如何实现单例模式请写出两种实现方式)

### 单例模式的应用场景有那些？
单例模式应用的场景一般发现在以下条件下：
* 资源共享的情况下，避免由于资源操作时导致的性能或损耗等，如日志文件，应用配置。
* 控制资源的情况下，方便资源之间的互相通信。如线程池等，1,网站的计数器 2,应用配置 3.多线程池 4数据库配置 数据库连接池 5.应用程序的日志应用...

### 对装饰器的理解，并写出一个计时器记录方法执行性能的装饰器？
装饰器本质上是一个callable object，它可以让其他函数在不需要做任何代码变动的前提下增加额外功能，装饰器的返回值也是一个函数对象。

```python
import time
from functools import wraps

def timeit(func):
    @wraps(func)
    def wrapper(*args, **kwargs):
        start = time.clock()
        ret = func(*args, **kwargs)
        end = time.clock()
        print('used:',end-start)
        return ret
    
    return wrapper
@timeit
def foo():
    print('in foo()' foo())
```
### 解释以下什么是闭包？
在函数内部再定义一个函数，并且这个函数用到了外边函数的变量，那么将这个函数以及用到的一些变量称之为闭包。

### 函数装饰器有什么作用？
装饰器本质上是一个callable object，它可以在让其他函数在不需要做任何代码的变动的前提下增加额外的功能。装饰器的返回值也是一个函数的对象，它经常用于有切面需求的场景。比如：插入日志，性能测试，事务处理，缓存。权限的校验等场景，有了装饰器就可以抽离出大量的与函数功能本身无关的雷同代码并发并继续使用。
详细参考：https://manjusaka.itscoder.com/2018/02/23/something-about-decorator/

### 生成器，迭代器的区别？
**迭代器**是遵循迭代协议的对象。用户可以使用`iter()`以从任何序列得到迭代器（如list、tuple、dictionary、set等）。另一个方法则是创建一个另一种形式的迭代器——generator。要获取下一个元素，则使用成员函数`next()`。当没有元素时，则引发`StopIteration`此例外。若要实现自己的迭代器，则只要实现 `__next__`。

**生成器(Generator)**，只是在需要返回数据的时候使用yield语句。每次`next()`被调用时，生成器会返回它脱离的位置（它记忆语句最后一次执行的位置和所有的数据值）

**区别：** 生成器能做到迭代器能做的所有事，而且因为自动创建`iter()`和`next()`方法，生成器显得特别简洁，而且生成器也是高效的，使用生成器表达式取代列表解析可以同时节省内存。除了创建和保存程序状态的自动方法，当发生器终结时，还会自动抛出`StopIteration`异常。

官方介绍：https://docs.python.org/3/tutorial/classes.html#iterators

### 简述any()和all()方法
**any():** 只要迭代器中有一个元素为真就为真
**all():** 迭代器中所有的判断项返回都是真，结果才为真
python中什么元素为假？`（0，空字符串，空列表、空字典、空元组、None, False）`

### X是什么类型?
X= (i for i in range(10))
X是**generator**类型

### 请用一行代码 实现将1-N的整数列表以3为单位分组
```python
N =100
print([[x for x in range(1, 100)][i:i + 3] for i in range(0, 100, 3)])
```
### Python中yield的用法?
**yield**就是保存当前程序执行状态。你用for循环的时候，每次取一个元素的时候就会计算一次。用yield的函数叫generator,和iterator一样，它的好处是不用一次计算所有元素，而是用一次算一次，可以节省很多空间，generator每次计算需要上一次计算结果，所以用yield,否则一return，上次计算结果就没了

## 面向对象
### Python中的可变对象和不可变对象？
**不可变对象：** 数值型、字符串、元组
**可变对象：** 列表、字典

### Python的魔法方法
`__init__`:对象初始化方法
`__new__`:创建对象时候执行的方法，单列模式会用到
`__str__`:当使用print输出对象的时候，只要自己定义了__str__(self)方法，那么就会打印从在这个方法中return的数据
`__del__`:删除对象执行的方法

### 简述面向对象中__new__和__init__区别
1. __init__是初始化方法，创建对象后，就立刻被默认调用了，可接收参数
2. __new__至少要有一个参数cls，代表当前类，此参数在实例化时由Python解释器自动识别
3. __new__必须要有返回值，返回实例化出来的实例，这点在自己实现__new__时要特别注意，可以return父类（通过super(当前类名, cls)）__new__出来的实例，或者直接是object的__new__出来的实例
4. __init__有一个参数self，就是这个__new__返回的实例，__init__在__new__的基础上可以完成一些其它初始化的动作，__init__不需要返回值
5. 如果__new__创建的是当前类的实例，会自动调用__init__函数，通过return语句里面调用的__new__函数的第一个参数是cls来保证是当前类实例，如果是其他类的类名，；那么实际创建返回的就是其他类的实例，其实就不会调用当前类的__init__函数，也不会调用其他类的__init__函数。

### 面向对象中怎么实现只读属性?
property装饰器把方法变成了类的属性
```python
class Demo():
    __name = "test"

    @property
    def name(self):
        return self.__name
```

### 谈谈你对面向对象的理解？
**面向对象**是相对于面向过程而言的。面向过程语言是一种基于功能分析的、以算法为中心的程序设计方法；而面向对象是一种基于结构分析的、以数据为中心的程序设计思想。在面向对象语言中有一个有很重要东西，叫做类。

面向对象有三大特性：**封装、继承、多态。** 

## 正则表达式
### 字符串a = "not 404 found 张三 99 深圳"，每个词中间是空格，用正则过滤掉英文和数字，最终输出"张三  深圳"
```Python
import re
a = "not 404 found 张三 99 深圳"

lists = a.split(' ')
print(lists)

res = re.findall('\d+|[a-zA-Z]+', a)
for i in res:
    if i in lists:
        lists.remove(i)
new_str = " ".join(res)
print(res)
print(new_str)
```

### 请写出一段代码用正则匹配出ip？
```python
import re
pattern = r'\\b(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\b'
regex = re.compile(pattern, re)
result = regex.findall(testString)
```

### 正则匹配，匹配日期2018-03-20
url=r'https://sycm.taobao.com/bda/tradinganaly/overview/get_summary.json?dateRange=2018-03-20%7C2018-03-20&dateType=recent1&device=1&token=ff25b109b&_=1521595613462'
```Python
import re
url=r'https://sycm.taobao.com/bda/tradinganaly/overview/get_summary.json?dateRange=2018-03-20%7C2018-03-20&dateType=recent1&device=1&token=ff25b109b&_=1521595613462'
res = re.findall(r'dateRange(.*?)%7C(.*?)&', url)
print(res)
```
### a = “abbbccc”，用正则匹配为abccc,不管有多少b，就出现一次？
### Python字符串查找和替换？
### 用Python匹配HTML`<div class="nam">中国</div>`，用正则匹配出标签里面的内容（“中国”），其中class的类名是不确定的，并说明<.> 和 <.*?> 有什么区别
```Python
import re
strs = <div class="nam">中国</div>
res = re.findall(r'<idv class=".">(.*?)</div>', strs)
print(res)
```
`.`: 代表可有可无
`*`: 代表任意字符
`(.*?)`: 提取文本
`（.*）`: 是贪婪匹配，会把满足正则的尽可能多的往后匹配
`（.*?）`: 是非贪婪匹配，会把满足正则的尽可能少匹配

### 正则表达式贪婪与非贪婪模式的区别？
### 写出开头匹配字母和下划线，末尾是数字的正则表达式？
### 正则表达式操作
### 请匹配出变量A中的json字符串。
### 怎么过滤评论中的表情？

### 正则匹配以163.com结尾的邮箱

### a="张明 98分"，用re.sub，将98替换为100
```Python
import re
a = "张明 98分"
res = re.sub(r'\d+', '100', a)
print(res)
```

### 简述Python里面search和match的区别
**re.match:** 只匹配字符串的开始，如果字符串开始不符合正则表达式，则匹配失败，函数返回None
**re.search:** 匹配整个字符串，直到找到一个匹配。

### 正则re.complie作用
**re.compile** 是将正则表达式编译成一个对象，加快速度，并重复使用

## 系统编程
### 10个Linux常用命令
[Linux与Windows命令的比较
](https://javyxu.cn/linux/linux_win_command/)

### 进程总结
**进程：** 程序运行在操作系统上的一个实例，就称之为进程。进程需要相应的系统资源：内存、时间片、pid。
1. 创建进程：
首先要导入multiprocessing中的Process：
创建一个Process对象;
创建Process对象时，可以传递参数;
    ```python
    p = Process(target=XXX, args=(tuple,), kwargs={key:value})
    # target = XXX 指定的任务函数，不用加(),
    # args=(tuple,) kwargs={key:value}给任务函数传递的参数
    ```
2. 使用start()启动进程
3. 结束进程
给子进程指定函数传递参数Demo
    ```python
    import os
    from mulitprocessing import Process
    import time

    def pro_func(name,age,**kwargs):
        for i in range(5):
            print("子进程正在运行中，name=%s,age=%d,pid=%d"%(name,age,os.getpid()))
            print(kwargs)
            time.sleep(0.2)
    if __name__ =="__main__":
        #创建Process对象
        p = Process(target=pro_func,args=('小明',18),kwargs={'m':20})
        #启动进程
        p.start()
        time.sleep(1)
        #1秒钟之后，立刻结束子进程
        p.terminate()
        p.join()
    ```
    注意：进程间不共享全局变量

**进程之间的通信-Queue**
1. 在初始化Queue()对象时（例如q=Queue(),若在括号中没有指定最大可接受的消息数量，获数量为负值时，那么就代表可接受的消息数量没有上限一直到内存尽头）
    * Queue.qsize():返回当前队列包含的消息数量
    * Queue.empty():如果队列为空，返回True，反之False
    * Queue.full():如果队列满了，返回True,反之False
    * Queue.get([block[,timeout]]):获取队列中的一条消息，然后将其从队列中移除，
    block默认值为True。如果block使用默认值，且没有设置timeout（单位秒),消息队列如果为空，此时程序将被阻塞（停在读中状态），直到消息队列读到消息为止，如果设置了timeout，则会等待timeout秒，若还没读取到任何消息，则抛出“Queue.Empty"异常：
    * Queue.get_nowait()相当于Queue.get(False)
    * Queue.put(item,[block[,timeout]]):将item消息写入队列，block默认值为True;如果block使用默认值，且没有设置timeout（单位秒），消息队列如果已经没有空间可写入，此时程序将被阻塞（停在写入状态），直到从消息队列腾出空间为止，如果设置了timeout，则会等待timeout秒，若还没空间，则抛出”Queue.Full"异常,如果block值为False，消息队列如果没有空间可写入，则会立刻抛出"Queue.Full"异常;
    * Queue.put_nowait(item):相当Queue.put(item,False)

**进程间通信Demo:**
```python
from multiprocessing import Process.Queue
import os,time,random
#写数据进程执行的代码：
def write(q):
    for value in ['A','B','C']:
        print("Put %s to queue...",%value)
        q.put(value)
        time.sleep(random.random())
#读数据进程执行的代码
def read(q):
    while True:
        if not q.empty():
            value = q.get(True)
            print("Get %s from queue.",%value)
            time.sleep(random.random())
        else:
            break
if __name__=='__main__':
    #父进程创建Queue，并传给各个子进程
    q = Queue()
    pw = Process(target=write,args=(q,))
    pr = Process(target=read,args=(q,))
    #启动子进程pw ，写入：
    pw.start()
    #等待pw结束
    pw.join()
    #启动子进程pr，读取：
    pr.start()
    pr.join()
    #pr 进程里是死循环，无法等待其结束，只能强行终止:
    print('')
    print('所有数据都写入并且读完')
```
**进程池Pool Demo**
```python
#coding:utf-8
from multiprocessing import Pool
import os,time,random

def worker(msg):
    t_start = time.time()
    print("%s 开始执行，进程号为%d"%(msg,os.getpid()))
    # random.random()随机生成0-1之间的浮点数
    time.sleep(random.random()*2)
    t_stop = time.time()
    print(msg,"执行完毕，耗时%0.2f”%（t_stop-t_start))

po = Pool(3)#定义一个进程池，最大进程数3
for i in range(0,10):
    po.apply_async(worker,(i,))
print("---start----")
po.close()
po.join()
print("----end----")
```
**进程池中使用Queue Demo**
如果要使用Pool创建进程，就需要使用multiprocessing.Manager()中的Queue(),而不是multiprocessing.Queue(),否则会得到如下的错误信息：
RuntimeError：Queue objects should only be shared between processs through inheritance
```python
from multiprocessing import Manager, Pool
import os,time,random
def reader(q):
    print("reader 启动(%s),父进程为（%s)"%(os.getpid(),os.getpid()))
    for i in range(q.qsize()):
        print("reader 从Queue获取到消息:%s"%q.get(True))

def writer(q):
    print("writer 启动（%s), 父进程为(%s)"%(os.getpid(),os.getpid()))
    for i ini "itcast":
        q.put(i)
if __name__ == "__main__":
    print("(%s)start"%os.getpid())
    q = Manager().Queue()#使用Manager中的Queue
    po = Pool()
    po.apply_async(wrtier,(q,))
    time.sleep(1)
    po.apply_async(reader,(q,))
    po.close()
    po.join()
    print("(%s)End"%os.getpid())
```

### 请介绍一下Python的线程同步？
#### setDaemon(False)
当一个进程启动之后，会默认产生一个主线程，因为线程是程序执行的最小单位，当设置多线程时，主线程会创建多个子线程，在Python中，默认情况下就是setDaemon(False),主线程执行完自己的任务以后，就退出了，此时子线程会继续执行自己的任务，直到自己的任务结束。
**例子:**
```python
import threading 
import time

def thread():
    time.sleep(2)
    print('---子线程结束---')

def main():
    t1 = threading.Thread(target=thread)
    t1.start()
    print('---主线程--结束')

if __name__ =='__main__':
    main()
#执行结果
---主线程--结束
---子线程结束---
```
#### setDaemon（True)
当我们使用setDaemon(True)时，这是子线程为守护线程，主线程一旦执行结束，则全部子线程被强制终止
**例子:**
```python
import threading
import time
def thread():
    time.sleep(2)
    print('---子线程结束---')
def main():
    t1 = threading.Thread(target=thread)
    t1.setDaemon(True)#设置子线程守护主线程
    t1.start()
    print('---主线程结束---')

if __name__ =='__main__':
    main()
#执行结果
---主线程结束--- #只有主线程结束，子线程来不及执行就被强制结束
```
#### join（线程同步)
join所完成的工作就是线程同步，即主线程任务结束以后，进入堵塞状态，一直等待所有的子线程结束以后，主线程再终止。
当设置守护线程时，含义是主线程对于子线程等待timeout的时间将会杀死该子线程，最后退出程序，所以说，如果有10个子线程，全部的等待时间就是每个timeout的累加和，简单的来说，就是给每个子线程一个timeou的时间，让他去执行，时间一到，不管任务有没有完成，直接杀死。
没有设置守护线程时，主线程将会等待timeout的累加和这样的一段时间，时间一到，主线程结束，但是并没有杀死子线程，子线程依然可以继续执行，直到子线程全部结束，程序退出。
**例子:**
```python
import threading
import time

def thread():
    time.sleep(2)
    print('---子线程结束---')

def main():
    t1 = threading.Thread(target=thread)
    t1.setDaemon(True)
    t1.start()
    t1.join(timeout=1)#1 线程同步，主线程堵塞1s 然后主线程结束，子线程继续执行
                        #2 如果不设置timeout参数就等子线程结束主线程再结束
                        #3 如果设置了setDaemon=True和timeout=1主线程等待1s后会强制杀死子线程，然后主线程结束
    print('---主线程结束---')

if __name__=='__main___':
    main()
```

### 谈谈你对多进程，多线程，以及协程的理解，项目是否用？
这个问题被问的概念相当之大，
**进程：** 一个运行的程序（代码）就是一个进程，没有运行的代码叫程序，进程是系统资源分配的最小单位，进程拥有自己独立的内存空间，所有进程间数据不共享，开销大。稳定性好，如果一个进程崩溃，不影响其他进程，但是进程消耗资源大，开启的进程数量有限制
**线程:** cpu调度执行的最小单位，也叫执行路径，不能独立存在，依赖进程存在，一个进程至少有一个线程，叫主线程，而多个线程共享内存（数据共享，共享全局变量),从而极大地提高了程序的运行效率。如果IO操作密集，则可以多线程运行效率高，缺点是如果一个线程崩溃，都会造成进程的崩溃
**协程:** 是一种用户态的轻量级线程，协程的调度完全由用户控制。协程拥有自己的寄存器上下文和栈。协程调度时，将寄存器上下文和栈保存到其他地方，在切回来的时候，恢复先前保存的寄存器上下文和栈，直接操中栈则基本没有内核切换的开销，可以不加锁的访问全局变量，所以上下文的切换非常快。
**应用:** 
* IO密集的用多线程，在用户输入，sleep 时候，可以切换到其他线程执行，减少等待的时间
* CPU密集的用多进程，因为假如IO操作少，用多线程的话，因为线程共享一个全局解释器锁，当前运行的线程会霸占GIL，其他线程没有GIL，就不能充分利用多核CPU的优势

### 多进程更稳定还是多线程更稳定？为什么？
多进程更稳定，它们是独立运行的，不会因为一个崩溃而影响其他进程

### 多线程的致命缺点是什么？
因为所有线程共享进程的内存，所以任何一个线程挂掉都可能直接造成整个进程崩溃。

### 进程间通信有哪些方式？
共享变量、队列、管道。

### Python的GIL
GIL 是python的全局解释器锁，同一进程中假如有多个线程运行，一个线程在运行python程序的时候会霸占python解释器（加了一把锁即GIL），使该进程内的其他线程无法运行，等该线程运行完后其他线程才能运行。如果线程运行过程中遇到耗时操作，则解释器锁解开，使其他线程运行。所以在多线程中，线程的运行仍是有先后顺序的，并不是同时进行。

多进程中因为每个进程都能被系统分配资源，相当于每个进程有了一个python解释器，所以多进程可以实现多个进程的同时运行，缺点是进程系统资源开销大

### Python异步使用场景有那些？
异步的使用场景:
1. 不涉及共享资源，获对共享资源只读，即非互斥操作
2. 没有时序上的严格关系
3. 不需要原子操作，或可以通过其他方式控制原子性
4. 常用于IO操作等耗时操作，因为比较影响客户体验和使用性能
5. 不影响主线程逻辑

### 多线程共同操作同一个数据互斥锁同步？
```python
import threading
import time
class MyThread(threading.Thread):
    def run(self):
        global num
        time.sleep(1)
    
        if mutex.acquire(1):
            num +=1
            msg = self.name + 'set num to ' +str(num)
            print msg
            mutex.release()
num = 0
mutex = threading.Lock()
def test():
    for i in range(5):
        t = MyThread()
        t.start()
if __name__=="__main__":
    test()
```

### 什么是多线程竞争？
线程是非独立的，同一个进程里线程是数据共享的，当各个线程访问数据资源时会出现竞争状态即：数据几乎同步会被多个线程占用，造成数据混乱，即所谓的线程不安全
那么怎么解决多线程竞争问题？---锁
**锁的好处:** 确保了某段关键代码（共享数据资源）只能由一个线程从头到尾完整地执行能解决多线程资源竞争下的原子操作问题。
**锁的坏处:** 阻止了多线程并发执行，包含锁的某段代码实际上只能以单线程模式执行，效率就大大地下降了
**锁的致命问题:** 死锁

### 解释以下什么是锁，有哪几种锁？
锁(Lock)是python提供的对线程控制的对象。有互斥锁，可重入锁，死锁。

### 什么是死锁？
若干子线程在系统资源竞争时，都在等待对方对某部分资源解除占用状态，结果是谁也不愿先解锁，互相干等着，程序无法执行下去，这就是死锁。
**GIL锁** 全局解释器锁（只在cython里才有）
**作用:** 限制多线程同时执行，保证同一时间只有一个线程执行，所以cython里的多线程其实是伪多线程！

所以python里常常使用协程技术来代替多线程，协程是一种更轻量级的线程。
进程和线程的切换时由系统决定，而协程由我们程序员自己决定，而模块gevent下切换是遇到了耗时操作时才会切换

三者的关系：进程里有线程，线程里有协程。

### 多线程交互访问数据，如果访问到了就不访问了？
怎么避免重读？
创建一个已访问数据列表，用于存储已经访问过的数据，并加上互斥锁，在多线程访问数据的时候先查看数据是否在已访问的列表中，若已存在就直接跳过。

### 什么是线程安全，什么是互斥锁？
每个对象都对应于一个可称为’互斥锁‘的标记，这个标记用来保证在任一时刻，只能有一个线程访问该对象。

同一进程中的多线程之间是共享系统资源的，多个线程同时对一个对象进行操作，一个线程操作尚未结束，另一线程已经对其进行操作，导致最终结果出现错误，此时需要对被操作对象添加互斥锁，保证每个线程对该对象的操作都得到正确的结果。

### 说说下面几个概念：同步，异步，阻塞，非阻塞？
**同步：** 多个任务之间有先后顺序执行，一个执行完下个才能执行。
**异步：** 多个任务之间没有先后顺序，可以同时执行，有时候一个任务可能要在必要的时候获取另一个同时执行的任务的结果，这个就叫回调！
**阻塞：** 如果卡住了调用者，调用者不能继续往下执行，就是说调用者阻塞了。
**非阻塞：** 如果不会卡住，可以继续执行，就是说非阻塞的。
同步异步相对于多任务而言，阻塞非阻塞相对于代码执行而言。

### 什么是僵尸进程和孤儿进程？怎么避免僵尸进程？
**孤儿进程：** 父进程退出，子进程还在运行的这些子进程都是孤儿进程，孤儿进程将被init 进程（进程号为1）所收养，并由init 进程对他们完成状态收集工作。
**僵尸进程：** 进程使用fork创建子进程，如果子进程退出，而父进程并没有调用wait 获waitpid 获取子进程的状态信息，那么子进程的进程描述符仍然保存在系统中的这些进程是僵尸进程。

避免僵尸进程的方法：
1. **fork** 两次用孙子进程去完成子进程的任务
2. 用**wait()** 函数使父进程阻塞
3. 使用信号量，在signal handler中调用waitpid,这样父进程不用阻塞

### python中进程与线程的使用场景？
多进程适合在CPU密集操作（cpu操作指令比较多，如位多的的浮点运算）。
多线程适合在IO密性型操作（读写数据操作比多的的，比如爬虫）

### 线程是并发还是并行，进程是并发还是并行？
线程是并发，进程是并行;
进程之间互相独立，是系统分配资源的最小单位，同一个线程中的所有线程共享资源。

### 并行(parallel)和并发（concurrency)?
**并行：** 同一时刻多个任务同时在运行不会在同一时刻同时运行，存在交替执行的情况。

实现并行的库有：**multiprocessing**
实现并发的库有: **threading**

程序需要执行较多的读写、请求和回复任务的需要大量的IO操作，IO密集型操作使用**并发**更好。

CPU运算量大的程序，使用**并行**会更好

### IO密集型和CPU密集型区别？
**IO密集型：** 系统运行，大部分的状况是CPU在等I/O（硬盘/内存）的读/写
**CPU密集型：** 大部分时间用来做计算，逻辑判断等CPU动作的程序称之CPU密集型。

### python asyncio的原理？
asyncio这个库就是使用python的yield这个可以打断保存当前函数的上下文的机制，封装好了selector摆脱掉了复杂的回调关系

## 网络编程
### 怎么实现强行关闭客户端和服务器之间的连接?
### 简述TCP和UDP的区别以及优缺点?
#### 区别
1. 基于连接与无连接
2. TCP要求系统资源较多，UDP较少； 
3. UDP程序结构较简单 
4. 流模式（TCP）与数据报模式(UDP); 
5. TCP保证数据正确性，UDP可能丢包 
6. TCP保证数据顺序，UDP不保证 
#### 优缺点
**TCP** 是面向连接的通讯协议，通过三次握手建立连接，通讯完成时四次挥手
**优点：** TCP在数据传递时，有确认、窗口、重传、阻塞等控制机制，能保证数据正确性，较为可靠。
**缺点：** TCP相对于UDP速度慢一点，要求系统资源较多。

**UDP** 是面向无连接的通讯协议，UDP数据包括目的端口号和源端口号信息。
**优点：** UDP速度快、操作简单、要求系统资源较少，由于通讯不需要连接，可以实现广播发送
**缺点：** UDP传送数据前并不与对方建立连接，对接收到的数据也不发送确认信号，发送端不知道数据是否会正确接收，也不重复发送，不可靠。

### 简述浏览器通过WSGI请求动态资源的过程?
### 描述用浏览器访问www.baidu.com的过程
### Post和Get请求的区别?
1. GET重点在从服务器上获取资源，POST重点在向服务器发送数据；
2. GET传输数据是通过URL请求，以field（字段）= value的形式，置于URL后，并用”?”连接，多个请求数据间用”&”连接如http://127.0.0.1/Test/login.action?name=admin&password=admin ，这个过程用户是可见的；POST传输数据通过HTTP的post机制，将字段与对应值封存在请求实体中发送给服务器，这个过程对用户是不可见的；
3. GET传输的数据量小，因为受URL长度限制，但效率较高；POST可以传输大量数据，所以上传文件时只能用post方式；
4. GET是不安全的，因为URL是可见的，可能会泄露私密信息，如密码等；POST较GET安全性较高；
5. GET方式只能支持ASCII字符，向服务器传的中文字符可能会乱码;POST支持标准字符集，可以正确传递中文字符。

### cookie和session的区别？
[Session、Cookie、JWT的理解](#sessioncookiejwt的理解)

### 列出你知道的HTTP协议的状态码，说出表示什么意思？
|状态码| 说明 | 意义 |
| --- | ---- | --- |
| 200 | OK | 请求正常处理完毕 |
| 204 | No Content | 请求成功处理，没有实体的主体返回 |
| 206 | Partial Content | GET范围请求已成功处理 |
| 301 | Moved Permanently | 永久重定向，资源已永久分配新URI |
| 302 | Found | 临时重定向，资源已临时分配新URI |
| 303 | See Other | 临时重定向，期望使用GET定向获取 |
| 304 | Not Modified | 发送的附带条件请求未满足 |
| 307 | Temporary Redirect | 临时重定向，POST不会变成GET |
| 400 | Bad Request | 请求报文语法错误或参数错误 |
| 401 | Unauthorized | 需要通过HTTP认证，或认证失败 |
| 403 | Forbidden | 请求资源被拒绝 |
| 404 | Not Found | 无法找到请求资源（服务器无理由拒绝）|
| 500 | Internal Server Error | 服务器故障或Web应用故障 |
| 503 | Service Unavailable | 服务器超负载或停机维护 |

### 请简单说一下三次握手和四次挥手？
### 说一下什么是tcp的2MSL？
### 为什么客户端在TIME-WAIT状态必须等待2MSL的时间？
### 说说HTTP和HTTPS区别？
**HTTP：** 是互联网上应用最为广泛的一种网络协议，是一个客户端和服务器端请求和应答的标准（TCP），用于从WWW服务器传输超文本到本地浏览器的传输协议，它可以使浏览器更加高效，使网络传输减少。
**HTTPS：** 是以安全为目标的HTTP通道，简单讲是HTTP的安全版，即HTTP下加入SSL层，HTTPS的安全基础是SSL，因此加密的详细内容就需要SSL。
HTTPS协议的主要作用可以分为两种：一种是建立一个信息安全通道，来保证数据传输的安全；另一种就是确认网站的真实性。

HTTPS和HTTP的区别主要如下：
1. https协议需要到ca申请证书，一般免费证书较少，因而需要一定费用。
2. http是超文本传输协议，信息是明文传输，https则是具有安全性的ssl加密传输协议。
3. http和https使用的是完全不同的连接方式，用的端口也不一样，前者是80，后者是443。
4. ttp的连接很简单，是无状态的；HTTPS协议是由SSL+HTTP协议构建的可进行加密传输、身份认证的网络协议，比http协议安全。
### 谈一下HTTP协议以及协议头部中表示数据类型的字段？
### HTTP请求方法都有什么？
### 使用Socket套接字需要传入哪些参数 ？
### HTTP常见请求头？
### 七层模型？
### url的形式？

# Web
## 分别从前端、后端、数据库阐述web项目的性能优化
**前端优化：**
1. 减少http请求、例如制作精灵图
2. html和CSS放在页面上部，javascript放在页面下面，因为js加载比HTML和Css加载慢，所以要优先加载html和css,以防页面显示不全，性能差，也影响用户体验差

**后端优化：**
1. 缓存存储读写次数高，变化少的数据，比如网站首页的信息、商品的信息等。应用程序读取数据时，一般是先从缓存中读取，如果读取不到或数据已失效，再访问磁盘数据库，并将数据再次写入缓存。
2. 异步方式，如果有耗时操作，可以采用异步，比如celery
3. 代码优化，避免循环和判断次数太多，如果多个if else判断，优先判断最有可能先发生的情况

**数据库优化：**
1. 如有条件，数据可以存放于redis，读取速度快
2. 建立索引、外键等

## Flask
### 对Flask蓝图(Blueprint)的理解？
#### 蓝图的定义
**蓝图(Blueprint)** 是Flask应用程序组件化的方法，可以在一个应用内或跨越多个项目共用蓝图。使用蓝图可以极大简化大型应用的开发难度，也为Flask扩展提供了一种在应用中注册服务的集中式机制。

#### 蓝图的应用场景
把一个应用分解为一个蓝图的集合。这对大型应用是理想的。一个项目可以实例化一个应用对象，初始化几个扩展，并注册一集合的蓝图。
以URL前缀和/或子域名，在应用上注册一个蓝图。URL前缀/子域名中的参数即成为这个蓝图下的所有视图函数的共同的视图参数（默认情况下）
在一个应用中用不同的URL规则多次注册一个蓝图。
通过蓝图提供模板过滤器、静态文件、模板和其他功能。一个蓝图不一定要实现应用或视图函数。
初始化一个Flask扩展时，在这些情况中注册一个蓝图。

#### 蓝图的缺点：
不能在应用创建后撤销注册一个蓝图而不销毁整个应用对象。

#### 使用蓝图的三个步骤
1. 创建一个蓝图对象
    ```python
    blue = Blueprint("blue",__name__)
    ```
2. 在这个蓝图对象上进行操作，例如注册路由、指定静态文件夹、注册模板过滤器...
    ```python
    @blue.route('/')
    def blue_index():
        return "Welcome to my blueprint"
    ```
3. 在应用对象上注册这个蓝图对象
    ```python
    app.register_blueprint(blue, url_prefix="/blue")
    ```

### Flask和Django路由映射的区别？
1. 在django中，路由是浏览器访问服务器时，先访问的项目中的url，再由项目中的url找到应用中url，这些url是放在一个列表里，遵从从前往后匹配的规则。
2. 在flask中，路由是通过装饰器给每个视图函数提供的，而且根据请求方式的不同可以一个url用于不同的作用。

## Django
### 什么是wsgi,uwsgi,uWSGI?
**WSGI:** web服务器网关接口，是一套协议。用于接收用户请求并将请求进行初次封装，然后将请求交给web框架。
**实现wsgi协议的模块：** wsgiref,本质上就是编写一socket服务端，用于接收用户请求（django)
**werkzeug**, 本质上就是编写一个socket服务端，用于接收用户请求(flask)

**uwsgi:** 与WSGI一样是一种通信协议，它是uWSGI服务器的独占协议，用于定义传输信息的类型。
**uWSGI:** 是一个web服务器，实现了WSGI的协议，uWSGI协议，http协议

### Django、Flask、Tornado的对比？
#### Django
1. Django走的大而全的方向，开发效率高。它的MTV框架，自带的ORM,admin后台管理,自带的sqlite数据库和开发测试用的服务器，给开发者提高了超高的开发效率。重量级web框架，功能齐全，提供一站式解决的思路，能让开发者不用在选择上花费大量时间。
2. 自带ORM和模板引擎，支持jinja等非官方模板引擎。
3. 自带ORM使Django和关系型数据库耦合度高，如果要使用非关系型数据库，需要使用第三方库
4. 自带数据库管理app
5. 成熟，稳定，开发效率高，相对于Flask，Django的整体封闭性比较好，适合做企业级网站的开发。python web框架的先驱，第三方库丰富

#### Flask
1. Flask是轻量级的框架，自由，灵活，可扩展性强，核心基于Werkzeug WSGI工具和jinja2模板引擎
2. 适用于做小网站以及web服务的API,开发大型网站无压力，但架构需要自己设计
3. 与关系型数据库的结合不弱于Django，而与非关系型数据库的结合远远优于Django

#### Tornado
1. Tornado走的是少而精的方向，性能优越，它最出名的异步非阻塞的设计方式
2. Tornado的两大核心模块：
* **iostraem:** 对非阻塞的socket进行简单的封装
* **ioloop:** 对I/O多路复用的封装,它实现一个单例

### 简述同源策略
同源策略需要同时满足以下三点要求： 
1. 协议相同 
2. 域名相同 
3. 端口相同 
    http:www.test.com与https:www.test.com 不同源——协议不同 http:www.test.com与http:www.admin.com 不同源——域名不同 http:www.test.com与http:www.test.com:8081 不同源——端口不同
    
只要不满足其中任意一个要求，就不符合同源策略，就会出现“跨域”

### CORS和CSRF的区别？
**什么是CORS？**
CORS是一个W3C标准,全称是“跨域资源共享"(Cross-origin resoure sharing).
它允许浏览器向跨源服务器，发出XMLHttpRequest请求，从而克服了AJAX只能同源使用的限制。

**什么是CSRF？**
CSRF主流防御方式是在后端生成表单的时候生成一串随机token,内置到表单里成为一个字段，同时，将此串token置入session中。每次表单提交到后端时都会检查这两个值是否一致，以此来判断此次表单提交是否是可信的，提交过一次之后，如果这个页面没有生成CSRF token,那么token将会被清空,如果有新的需求，那么token会被更新。
攻击者可以伪造POST表单提交，但是他没有后端生成的内置于表单的token，session中没有token都无济于事。

### Session、Cookie、JWT的理解
1. 为什么要使用会话管理
众所周知，HTTP协议是一个无状态的协议，也就是说每个请求都是一个独立的请求，请求与请求之间并无关系。但在实际的应用场景，这种方式并不能满足我们的需求。举个大家都喜欢用的例子，把商品加入购物车，单独考虑这个请求，服务端并不知道这个商品是谁的，应该加入谁的购物车？因此这个请求的上下文环境实际上应该包含用户的相关信息，在每次用户发出请求时把这一小部分额外信息，也做为请求的一部分，这样服务端就可以根据上下文中的信息，针对具体的用户进行操作。所以这几种技术的出现都是对HTTP协议的一个补充，使得我们可以用HTTP协议+状态管理构建一个的面向用户的WEB应用。

2. Session和Cookie的区别
    * session 在服务器端，cookie 在客户端（浏览器）
    * session 的运行依赖 session id，而 session id 是存在 cookie 中的，也就是说，如果浏览器禁用了 cookie ，同时 session 也会失效，存储Session时，键与Cookie中的sessionid相同，值是开发人员设置的键值对信息，进行了base64编码，过期时间由开发人员设置
    * cookie安全性比session差
    * 个人认为session与cookies最核心区别在于额外信息由谁来维护。利用cookies来实现会话管理时，用户的相关信息或者其他我们想要保持在每个请求中的信息，都是放在cookies中,而cookies是由客户端来保存，每当客户端发出新请求时，就会稍带上cookies,服务端会根据其中的信息进行操作。当利用session来进行会话管理时，客户端实际上只存了一个由服务端发送的session_id,而由这个session_id,可以在服务端还原出所需要的所有状态信息，从这里可以看出这部分信息是由服务端来维护的。
  
3. 除此以外，session与cookies都有一些自己的缺点：   
cookies的安全性不好，攻击者可以通过获取本地cookies进行欺骗或者利用cookies进行CSRF攻击。使用cookies时,在多个域名下，会存在跨域问题。
session 在一定的时间里，需要存放在服务端，因此当拥有大量用户时，也会大幅度降低服务端的性能，当有多台机器时，如何共享session也会是一个问题.(redis集群)也就是说，用户第一个访问的时候是服务器A，而第二个请求被转发给了服务器B，那服务器B如何得知其状态。实际上，session与cookies是有联系的，比如我们可以把session_id存放在cookies中的。

4. JWT是如何工作的
首先用户发出登录请求，服务端根据用户的登录请求进行匹配，如果匹配成功，将相关的信息放入payload中，利用算法，加上服务端的密钥生成token，这里需要注意的是secret_key很重要，如果这个泄露的话，客户端就可以随机篡改发送的额外信息，它是信息完整性的保证。生成token后服务端将其返回给客户端，客户端可以在下次请求时，将token一起交给服务端，一般是说我们可以将其放在Authorization首部中，这样也就可以避免跨域问题。

### 简述Django请求生命周期
一般是用户通过浏览器向我们的服务器发起一个请求(request),这个请求会去访问视图函数，如果不涉及到数据调用，那么这个时候视图函数返回一个模板也就是一个网页给用户）
视图函数调用模型毛模型去数据库查找数据，然后逐级返回，视图函数把返回的数据填充到模板中空格中，最后返回网页给用户。
xs
1. wsgi, 请求封装后交给web框架（Flask，Django)
2. 中间件，对请求进行校验或在请求对象中添加其他相关数据，例如：csrf,request.session
3. 路由匹配 根据浏览器发送的不同url去匹配不同的视图函数
4. 视图函数，在视图函数中进行业务逻辑的处理，可能涉及到：orm，templates 
5. 中间件，对响应的数据进行处理
6. wsgi，将响应的内容发送给浏览器

### 用的restframework完成api发送时间时区
当前的问题是用django的rest framework模块做一个get请求的发送时间以及时区信息的api
```python
class getCurrenttime(APIView):
    def get(self,request):
        local_time = time.localtime()
        time_zone =settings.TIME_ZONE
        temp = {'localtime':local_time,'timezone':time_zone}
        return Response(temp)
```

### nginx,tomcat,apache都是什么？
**Nginx（engine x)** 是一个高性能的HTTP和反向代理服务器，也是一个IMAP/POP3/SMTP服务器，工作在OSI七层，负载的实现方式：轮询，IP_HASH,fair,session_sticky.
**Apache HTTP Server** 是一个模块化的服务器，源于NCSAhttpd服务器
**Tomcat** 服务器是一个免费的开放源代码的Web应用服务器，属于轻量级应用服务器，是开发和调试JSP程序的首选。

### 请给出你熟悉关系数据库范式有哪些，有什么作用？
在进行数据库的设计时，所遵循的一些规范，只要按照设计规范进行设计，就能设计出没有数据冗余和数据维护异常的数据库结构。

数据库的设计的规范有很多，通常来说我们在设是数据库时只要达到其中一些规范就可以了，这些规范又称之为数据库的三范式，一共有三条，也存在着其他范式，我们只要做到满足前三个范式的要求，就能设陈出符合我们的数据库了，我们也不能全部来按照范式的要求来做，还要考虑实际的业务使用情况，所以有时候也需要做一些违反范式的要求。
1. 数据库设计的第一范式(最基本)，基本上所有数据库的范式都是符合第一范式的，符合第一范式的表具有以下几个特点：
数据库表中的所有字段都只具有单一属性，单一属性的列是由基本的数据类型（整型，浮点型，字符型等）所构成的设计出来的表都是简单的二比表
2. 数据库设计的第二范式(是在第一范式的基础上设计的)，要求一个表中只具有一个业务主键，也就是说符合第二范式的表中不能存在非主键列对只对部分主键的依赖关系
3. 数据库设计的第三范式，指每一个非主属性既不部分依赖与也不传递依赖于业务主键，也就是第二范式的基础上消除了非主属性对主键的传递依赖

### 简述QQ登陆过程
qq登录，在我们的项目中分为了三个接口:
1. 第一个接口是请求qq服务器返回一个qq登录的界面;
2. 第二个接口是通过扫码或账号登陆进行验证，qq服务器返回给浏览器一个code和state,利用这个code通过本地服务器去向qq服务器获取access_token覆返回给本地服务器，凭借access_token再向qq服务器获取用户的openid(openid用户的唯一标识)
3. 第三个接口是判断用户是否是第一次qq登录，如果不是的话直接登录返回的jwt-token给用户，对没有绑定过本网站的用户，对openid进行加密生成token进行绑定

### 项目中日志的作用
#### 日志相关概念
1. 日志是一种可以追踪某些软件运行时所发生事件的方法
2. 软件开发人员可以向他们的代码中调用日志记录相关的方法来表明发生了某些事情
3. 一个事件可以用一个包含可选变量数据的消息来描述
4. 此外，事件也有重要性的概念，这个重要性也可以被成为严重性级别(level)

#### 日志的作用
1. 通过log的分析，可以方便用户了解系统或软件、应用的运行情况;
2. 如果你的应用log足够丰富，可以分析以往用户的操作行为、类型喜好，地域分布或其他更多信息;
3. 如果一个应用的log同时也分了多个级别，那么可以很轻易地分析得到该应用的健康状况，及时发现问题并快速定位、解决问题，补救损失。
4. 简单来讲就是我们通过记录和分析日志可以了解一个系统或软件程序运行情况是否正常，也可以在应用程序出现故障时快速定位问题。不仅在开发中，在运维中日志也很重要，日志的作用也可以简单。总结为以下几点：
    * 程序调试
    * 了解软件程序运行情况，是否正常
    * 软件程序运行故障分析与问题定位
    * 如果应用的日志信息足够详细和丰富，还可以用来做用户行为分析

#### log日志中，我们需要用时间戳记录error,warning等的发生时间，请用datetime模块打印当前时间戳 “2018-04-01 11:38:54”
```Python
import datetime
a = str(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')) + ' 星期 ' + str(datetime.datetime.now().isoweekday())
print(a)
```

### 异常名称及其意义
| 名称 | 意义 |
| --- | ---- |
| IOError | 输入输出异常 |
| AttributeError | 试图访问一个对象没有的属性 |
| ImportError | 无法引入模块或包，基本是路径问题 |
| IndentationError | 语法错误，代码没有正确的对齐 |
| IndexError | 下标索引超出序列边界 |
| KeyError | 试图访问你字典里不存在的键 |
| SyntaxError | Python代码逻辑语法出错，不能执行 |
| NameError | 使用一个还未赋予对象的变量 |

### django中间件的使用？
Django在中间件中预置了六个方法，这六个方法的区别在于不同的阶段执行，对输入或输出进行干预，方法如下：
1. 初始化：无需任何参数，服务器响应第一个请求的时候调用一次，用于确定是否启用当前中间件
    ```python
    def __init__():
        pass
    ```
2. 处理请求前：在每个请求上调用，返回None或HttpResponse对象。
    ```python
    def process_request(request):
        pass
    ```
3. 处理视图前:在每个请求上调用，返回None或HttpResponse对象。
    ```python
    def process_view(request,view_func,view_args,view_kwargs):
        pass
    ```
4. 处理模板响应前：在每个请求上调用，返回实现了render方法的响应对象。
    ```python
    def process_template_response(request,response):
        pass
    ```
5. 处理响应后：所有响应返回浏览器之前被调用，在每个请求上调用，返回HttpResponse对象。
    ```python
    def process_response(request,response):
        pass
    ```
6. 异常处理：当视图抛出异常时调用，在每个请求上调用，返回一个HttpResponse对象。
    ```python
    def process_exception(request,exception):
        pass
    ```

### 谈一下你对uWSGI和nginx的理解？
**uWSGI** 是一个Web服务器，它实现了WSGI协议、uwsgi、http等协议。Nginx中HttpUwsgiModule的作用是与uWSGI服务器进行交换。WSGI是一种Web服务器网关接口。它是一个Web服务器（如nginx，uWSGI等服务器）与web应用（如用Flask框架写的程序）通信的一种规范。

要注意WSGI/uwsgi/uWSGI这三个概念的区分。
* WSGI是一种通信协议。
* uwsgi是一种线路协议而不是通信协议，在此常用于在uWSGI服务器与其他网络服务器的数据通信。
* uWSGI是实现了uwsgi和WSGI两种协议的Web服务器。

**nginx** 是一个开源的高性能的HTTP服务器和反向代理：
1. 作为web服务器，它处理静态文件和索引文件效果非常高
2. 它的设计非常注重效率，最大支持5万个并发连接，但只占用很少的内存空间
3. 稳定性高，配置简洁。
4. 强大的反向代理和负载均衡功能，平衡集群中各个服务器的负载压力应用

### Python中三大框架各自的应用场景？
**django:** 主要是用来搞快速开发的，他的亮点就是快速开发，节约成本，,如果要实现高并发的话，就要对django进行二次开发，比如把整个笨重的框架给拆掉自己写socket实现http的通信,底层用纯c,c++写提升效率，ORM框架给干掉，自己编写封装与数据库交互的框架,ORM虽然面向对象来操作数据库，但是它的效率很低，使用外键来联系表与表之间的查询;
**flask:** 轻量级，主要是用来写接口的一个框架，实现前后端分离，提考开发效率，Flask本身相当于一个内核，其他几乎所有的功能都要用到扩展(邮件扩展Flask-Mail，用户认证Flask-Login),都需要用第三方的扩展来实现。比如可以用Flask-extension加入ORM、文件上传、身份验证等。Flask没有默认使用的数据库，你可以选择MySQL，也可以用NoSQL。其WSGI工具箱用Werkzeug(路由模块)，模板引擎则使用Jinja2,这两个也是Flask框架的核心。
**Tornado：** Tornado是一种Web服务器软件的开源版本。Tornado和现在的主流Web服务器框架（包括大多数Python的框架）有着明显的区别：它是非阻塞式服务器，而且速度相当快。得利于其非阻塞的方式和对epoll的运用，Tornado每秒可以处理数以千计的连接因此Tornado是实时Web服务的一个理想框架

### Django中哪里用到了线程？哪里用到了协程？哪里用到了进程？
1. Django中耗时的任务用一个进程或者线程来执行，比如发邮件，使用celery.
2. 部署django项目是时候，配置文件中设置了进程和协程的相关配置。

### 有用过Django REST framework吗？
Django REST framework是一个强大而灵活的Web API工具。使用RESTframework的理由有：
* Web browsable API对开发者有极大的好处
* 包括OAuth1a和OAuth2的认证策略
* 支持ORM和非ORM数据资源的序列化

全程自定义开发--如果不想使用更加强大的功能，可仅仅使用常规的function-based views额外的文档和强大的社区支持

## 爬虫
### 什么是爬虫，为什么要用爬虫?    
**爬虫：** 用于在网络上采集数据的程序，可以用任何语言开发，python更加方便快捷高效一些。
**爬虫的目的：** 采集一些需要的数据。 
**为什么python更适合写爬虫程序？** python中封装了很多爬虫库，如urllib、re、bs、scrapy等，开发效率更高

### 爬虫的基本流程？        
1. 浏览器发起请求，可能包含请求头等信息，等待服务器相应
2. 获取服务器响应内容，可能是网页文本（html、json代码），图片二进制、视频二进制等
3. 解析内容（正则、xpath、json解析等 ）
4. 保存数据（本地文件、数据库等）

### 如何提高爬取效率？
爬虫下载慢主要原因是阻塞等待发往网站的请求和网站返回
1. 采用异步与多线程，扩大电脑的cpu利用率
2. 用消息队列模式
3. 提高带宽

### 爬虫协议？
**Robots协议**（也称为爬虫协议、爬虫规则、机器人协议等）也就是robots.txt，网站通过robots协议告诉搜索引擎哪些页面可以抓取，哪些页面不能抓取。
**Robots协议** 是网站国际互联网界通行的道德规范，其目的是保护网站数据和敏感信息、确保用户个人信息和隐私不被侵犯。因其不是命令，故需要搜索引擎自觉遵守。

### 试列出至少三种目前流行的大型数据库
* Oracle
* PostgreSQL
* MySQL
* HBase

### 列举您使用过的Python网络爬虫所用到的网络数据包?
* urllib
* urllib2
* requests
* httplib2

### 你用过的爬虫框架或者模块有哪些？优缺点？
#### 框架或者模块
**Python自带：** urllib，urllib2
urllib和urllib2模块都做与请求URL相关的操作，但他们提供不同的功能。
urllib2.：urllib2.urlopen可以接受一个Request对象或者url，（在接受Request对象时候，并以此可以来设置一个URL 的headers），urllib.urlopen只接收一个urlurllib 有urlencode,urllib2没有，因此总是urllib，urllib2常会一起使用的原因scrapy是封装起来的框架，他包含了下载器，解析器，日志及异常处理，基于多线程， twisted的方式处理，对于固定单个网站的爬取开发，有优势，但是对于多网站爬取 100个网站，并发及分布式处理方面，不够灵活，不便调整与括展。
**第三方：** requests
request 是一个HTTP库， 它只是用来，进行请求，对于HTTP请求，他是一个强大的库，下载，解析全部自己处理，灵活性更高，高并发与分布式部署也非常灵活，对于功能可以更好实现.
**框架：** Scrapy

**优点：** 采取可读性更强的xpath代替正则 强大的统计和log系统 同时在不同的url上爬行 支持shell方式，方便独立调试 写middleware,方便写一些统一的过滤器 通过管道的方式存入数据库
**缺点：** 基于python爬虫框架，扩展性比较差，基于twisted框架，运行中exception是不会干掉reactor，并且异步框架出错后是不会停掉其他任务的，数据出错后难以察觉

### 写爬虫是用多进程好？还是多线程好？
IO密集型代码(文件处理、网络爬虫等)，多线程能够有效提升效率(单线程下有IO操作会进行IO等待，造成不必要的时间浪费，而开启多线程能在线程A等待时，自动切换到线程B，可以不浪费CPU的资源，从而能提升程序执行效率)。在实际的数据采集过程中，既考虑网速和响应的问题，也需要考虑自身机器的硬件情况，来设置多进程或多线程

### 常见的反爬虫和应对方法？
1. 基于用户行为，同一个ip段时间多次访问同一页面，利用代理ip，构建ip池
2. 请求头里的user-agent，构建user-agent池（操作系统、浏览器不同，模拟不同用户）
3. 动态加载（抓到的数据和浏览器显示的不一样），js渲染，模拟ajax请求，返回json形式的数据 
4. selenium/webdriver模拟浏览器加载
5. 对抓到的数据进行分析
6. 加密参数字段、会话跟踪[cookie]、防盗链设置[Referer]

### 解析网页的解析器使用最多的是哪几个?
1. BeautifulSoup
2. pyquery
3. Xpath
4. lxml

### 需要登录的网页，如何解决同时限制ip，cookie, session

### 验证码的解决?
HTTP请求的basic认证
客户端将输入的用户名密码用Base64进行编码后，采用非加密的明文方式传送给服务器。
Authorization: Basic xxxxxxxxxx.

### 使用最多的数据库，对他们的理解？

### 编写过哪些爬虫中间件？

### “极验”滑动验证码如何破解？

### 爬虫多久爬一次，爬下来的数据使用哪个数据库存储数据，是怎么存储，为什么，部署是你做的吗？怎么部署？
PostgreSQL
Sqlite

### cookie过期的处理问题？
自动更新cookie呢？这里会用到selenium。
1. 采用selenium自动登录获取cookie，保存到文件;
2. 读取cookie，比较cookie的有效期，若过期则再次执行步骤1；
3. 在请求其他网页时，填入cookie，实现登录状态的保持。

### 动态加载又对及时性要求很高怎么处理？

### HTTPS有什么优点和缺点？
**HTTPS的优点：**
1. HTTPS具有更好的加密性能，避免用户信息泄露；
2. HTTPS复杂的传输方式，降低网站被劫持的风险；
3. 搜索引擎已经全面支持HTTPS抓取、收录，并且会优先展示HTTPS结果；
4. HTTPS绿锁表示可以提升用户对网站信任程度；
5. 可以有效防止山寨、镜像网站等

**HTTPS的缺点：**
1. 繁重的计算和多次交互自然的影响了访问速度
2. 网站改用HTTPS以后，由HTTP跳转到HTTPS的方式增加了用户访问耗时
3. HTTPS涉及到的安全算法会消耗CPU资源，需要增加服务器资源（https访问过程需要加解密）但是还是建议安装SSL证书实现HTTPS.

### HTTPS是如何实现安全传输数据的？
对安全或密码学基础有了解的同学，应该知道常见的加密手段。一般来说，加密分为对称加密、非对称加密（也叫公开密钥加密）。

**对称加密**对称加密的意思就是，加密数据用的密钥，跟解密数据用的密钥是一样的。
**优点** 在于加密、解密效率通常比较高。
**缺点** 在于，数据发送方、数据接收方需要协商、共享同一把密钥，并确保密钥不泄露给其他人。此外，对于多个有数据交换需求的个体，两两之间需要分配并维护一把密钥，这个带来的成本基本是不可接受的。

**非对称加密**非对称加密的意思就是，加密数据用的密钥（公钥），跟解密数据用的密钥（私钥）是不一样的。
**什么叫做公钥呢？** 其实就是字面上的意思——公开的密钥，谁都可以查到。因此非对称加密也叫做公开密钥加密。相对应的，私钥就是非公开的密钥，一般是由网站的管理员持有。

**公钥、私钥两个有什么联系呢？**
简单的说就是，通过公钥加密的数据，只能通过私钥解开。通过私钥加密的数据，只能通过公钥解开。
很多同学都知道用私钥能解开公钥加密的数据，但忽略了一点，私钥加密的数据，同样可以用公钥解密出来。而这点对于理解HTTPS的整套加密、授权体系非常关键。

### TTL，MSL，RTT各是什么？
1. MSL是Maximum Segment Lifetime英文的缩写，中文可以译为“报文最大生存时间”，他是任何报文在网络上存在的最长时间，超过这个时间报文将被丢弃。TCP报文 （segment）是ip数据报（datagram）的数据部分，具体称谓请参见《数据在网络各层中的称呼》一文；
2. ip头中有一个TTL域，TTL是 time to live的缩写，中文可以译为“生存时间”，这个生存时间是由源主机设置初始值但不是存的具体时间，而是存储了一个ip数据报可以经过的最大路由数，每经 过一个处理他的路由器此值就减1，当此值为0则数据报将被丢弃，同时发送ICMP报文通知源主机。RFC 793中规定MSL为2分钟，实际应用中常用的是30秒，1分钟和2分钟等。
    `TTL与MSL是有关系的但不是简单的相等的关系，MSL要大于等于TTL。`
3. RTT是客户到服务器往返所花时间（round-trip time，简称RTT），TCP含有动态估算RTT的算法。TCP还持续估算一个给定连接的RTT，这是因为RTT受网络传输拥塞程序的变化而变化。
表示从发送端发送数据开始，到发送端收到来自接收端的确认（接收端收到数据后便立即发送确认），总共经历的时延。 
一般认为单向时延=传输时延t1+传播时延t2+排队时延t3 
t1是数据从进入节点到传输媒体所需要的时间，通常等于数据块长度/信道带宽 
t2是信号在信道中需要传播一定距离而花费的时间，等于信道长度/传播速率（光纤中电磁波的传播速率约为2*10^5 km/s，铜缆中2.3*10^5 km/s） 
t3可笼统归纳为随机噪声，由途径的每一跳设备及收发两端负荷情况及吞吐排队情况决定(包含互联网设备和传输设备时延)
4. 2MSL即两倍的MSL，TCP的TIME_WAIT状态也称为2MSL等待状态，当TCP的一端发起主动关闭，在发出最后一个ACK包后，即第3次握 手完成后发送了第四次握手的ACK包后就进入了TIME_WAIT状态，必须在此状态上停留两倍的MSL时间，等待2MSL时间主要目的是怕最后一个 ACK包对方没收到，那么对方在超时后将重发第三次握手的FIN包，主动关闭端接到重发的FIN包后可以再发一个ACK应答包。在TIME_WAIT状态 时两端的端口不能使用，要等到2MSL时间结束才可继续使用。当连接处于2MSL等待阶段时任何迟到的报文段都将被丢弃。不过在实际应用中可以通过设置 SO_REUSEADDR选项达到不必等待2MSL时间结束再使用此端口

### 平常怎么使用代理的 ？
1. 为什么会用到代理将真是IP隐藏起来（请求过于太频繁的话，ip可能会被禁止）
2. 代理怎么使用（具体代码，请求在什么时候添加的代理）
proxy_handler = ProxyHandler({'http': 'http://183.159.89.204:18118'})# 构建一个Opener对象proxy_opener = build_opener(proxy_handler)# 使用自定义opener访问服务器数据，得到相应response = proxy_opener.open(request)

### 存放在数据库(redis、mysql等)。

### 怎么监控爬虫的状态?

### 爬取数据的影响因素？    
影响因素：机器的性能及带宽，代码质量，爬取时的反爬机制

### scrapy和requests的使用情况？
**requests** 是polling方式的，会被网络阻塞，不适合爬取大量数据
**scapy** 底层是异步框架twisted，并发是最大优势

### 描述下scrapy框架运行的机制？
1. 从start_urls里面获取第一批url发送请求，请求由请求引擎给调度器入请求对列，
2. 获取完毕后，调度器将请求对列交给下载器去获取请求对应的响应资源，并将响应交给自己编写的解析方法做提取处理，
3. 如果提取出需要的数据，则交给管道处理，如果提取出url，则继续执行之前的步骤，直到多列里没有请求，程序结束。

### 谈谈你对Scrapy的理解？

### 怎么样让scrapy框架发送一个post请求（具体写出来）

### 怎么监控爬虫的状态 ？

### 怎么判断网站是否更新？

### 图片、视频爬取怎么绕过防盗连接

### 你爬出来的数据量大概有多大？大概多长时间爬一次？

### 增量爬取

### 爬取下来的数据如何去重，说一下scrapy的具体的算法依据。

### Scrapy的优缺点?
**优点：** 
1. 采取可读性更强的xpath代替正则、强大的统计和log系统 同时在不同的url上爬行 
2. 支持shell方式，方便独立调试 
3. 写middleware,方便写一些统一的过滤器 
4. 通过管道的方式存入数据库

**缺点：**
1. 基于python爬虫框架，扩展性比较差；
2. 基于twisted框架，运行中exception是不会干掉reactor，并且异步框架出错后是不会停掉其他任务的，数据出错后难以察觉

### 怎么设置爬取深度？

### scrapy和scrapy-redis有什么区别？为什么选择redis数据库？
#### 区别
**scrapy** 是一个爬虫通用框架，但不支持分布式，
**scrapy-redis** 是为了更方便的实现scrapy分布式爬虫，而提供了一些以redis为基础的组件    
#### 为什么会选择redis数据库？   
1. 因为redis支持主从同步，而且数据都是缓存在内存中，所以基于redis的分布式爬虫，对请求和数据的高频读取效率非常高
2. 什么是主从同步？
在Redis中，用户可以通过执行SLAVEOF命令或者设置slaveof选项，让一个服务器去复制（replicate）另一个服务器，我们称呼被复制的服务器为主服务器（master），而对主服务器进行复制的服务器则被称为从服务器（slave），当客户端向从服务器发送SLAVEOF命令，要求从服务器复制主服务器时，从服务器首先需要执行同步操作，也即是，将从服务器的数据库状态更新至主服务器当前所处的数据库状态

### 分布式爬虫主要解决什么问题？
面对海量待抓取网页，只有采用分布式架构，才有可能在较短时间内完成一轮抓取工作。它的开发效率是比较快而且简单的。

### 什么是分布式存储？
**分布式存储系统**，是将数据分散存储在多台独立的设备上。传统的网络存储系统采用集中的存储服务器存放所有数据，存储服务器成为系统性能的瓶颈，也是可靠性和安全性的焦点，不能满足大规模存储应用的需要。分布式网络存储系统采用可扩展的系统结构，利用多台存储服务器分担存储负荷，利用位置服务器定位存储信息，它不但提高了系统的可靠性、可用性和存取效率，还易于扩展。

### 你所知道的分布式爬虫方案有哪些？

### scrapy-redis，有做过其他的分布式爬虫吗？

# 数据库
## MySQL
### 主键 超键 候选键 外键
### 视图的作用，视图可以更改么？
### drop,delete与truncate的区别
### 索引的工作原理及其种类
### 连接的种类
### 数据库优化的思路
1. 如有条件，数据可以存放于redis，读取速度快
2. 建立外键、索引、联合查询、选择特定字段等等

### 存储过程与触发器的区别
### 悲观锁和乐观锁是什么？
### 你常用的mysql引擎有哪些?各引擎间有什么区别?
### Mysql怎么限制IP访问？

## Redis
### Redis宕机怎么解决?
非常危险的动作：重新启动主库。
要知道这样一来，最坏情况数据将全部丢失。因为主库没有配置持久化，所以主库的data目录只有从库连接主库请求resync的时候做快照留下来的dump.rdb文件。如果重启主库，主库会按照data目录下的dump.rdb来恢复数据。因此，如果从库是从最开始就配置好了的而且没有发生过再次请求resync，那么此时的dump.rdb将是空的。主库按照空的dump.rdb恢复数据，自然数据全无，从库发现主库能够连接上时会自动请求resync,从库也将拷贝一份空白的数据。

正确做法：连上从库，做save操作。将会在从库的data目录保存一份从库最新的dump.rdb文件。将这份dump.rdb文件拷贝到主库的data目录下。再重启主库
### redis和mecached的区别，以及使用场景
#### 区别
1. 存储方式：Memcache把数据全部存在内存之中，断电后会挂掉，数据不能超过内存大小。Redis支持数据的持久化，可以将内存中的数据保存在磁盘中，重启时可以再次加载进行使用。（RDB快照和AOF日志两 种持久化方式）。
2. Redis支持数据的备份，及master-slave模式的数据备份。
3. 数据支持类型：Redis在数据支持上要比Memcache多得多。
4. 使用底层模型不同：新版本的Redis直接自己构建了VM机制，因为一般的系统调用系统函数的话，会浪费一定的时间去移动和请求。
5. redis有一个致命缺陷 当内存满了时dump数据cpu占用100%。
#### 使用场景
如果需要缓存的数据只是key-value这样简单的结构时，采用Memcache，足够稳定可靠。如果有持久化需求、存储、排序等一系列复制操作时，或者对数据结构和处理有高级要求的应用，选择Redis。
* memcache使用场景
1、在动态系统中减少数据库负载，提升性能，做缓存，适合多读少写，大数据量的情况（如人人网大量查询用户信息、好友信息、文章信息等）。它的一个总原则是将经常需要从数据库读取的数据缓存在memcached中，这些数据也分为几类：（1）经常被读取并且实时性要求不强可以等到自动过期的数据。例如网站首页最新文章列表、某某排行等数据。也就是虽然新数据产生了，但对用户体验不会产生任何影响的场景。这类数据就使用典型的缓存策略，设置一过合理的过期时间，当数据过期以后再从数据库中读取。当然你得制定一个缓存清除策略，便于编辑或者其它人员能马上看到效果。（2）经常被读取并且实时性要求强的数据。比如用户的好友列表，用户文章列表，用户阅读记录等。这类数据首先被载入到memcached中，当发生更改（添加、修改、删除）时就清除缓存。在缓存的时候，我将查询的SQL语句md5（）得到它的 hash值作为key,结果数组作为值写入memcached，并且将该SQL涉及的table_name以及hash值配对存入memcached中。 当更改了这个表时，我就将与此表相配对的key的缓存全部删除。2、秒杀功能：一个人下单，要牵涉数据库读取，写入订单，更改库存，及事务要求， 对于传统型数据库来说，压力是巨大的。可以利用 memcached 的 incr/decr 功能， 在内存存储 count 库存量， 秒杀 1000 台每人抢单主要在内存操作，速度非常快，抢到 count < =1000 的号人，得一个订单号，这时再去另一个页面慢慢支付。
* 不适用memcached的业务场景： 
1、缓存对象的大小大于1MB；
2、key的长度大于250字符（所以我们把一些key先md5再存储）；
3、应用运行在不安全的环境中Memcached为提供任何安全策略，仅仅通过telnet就可以访问到memcached。如果应用运行在共享的系统上，需要着重考虑安全问题；
4、业务本身需要的是持久化数据。
* Redis场景：适用于对读写效率要求都很高，数据处理业务复杂和对安全性要求较高的系统（如新浪微博的计数和微博发布部分系统，对数据安全性、读写要求都很高）、Pub/Sub构建实时消息系统、统计。
### Redis支持哪几种持久化方式
#### RDB持久化
原理是将Redis在内存中的数据记录定时dump到磁盘上的RDB文件
指定的时间间隔内将内存中的数据集快照写入磁盘，实际操作过程是fork一个子进程，先将数据集写入临时文件，写入成功后，再替换之前的文件，用二进制压缩存储。
#### AOF（append only file）持久化
原理是将Redis的操作日志以追加的方式写入文件。
以日志的形式记录服务器所处理的每一个写、删除操作，查询操作不会记录，以文本的方式记录，可以打开文件看到详细的操作记录。当服务器重启的时候会重新执行这些命令来恢复原始的数据。AOF命令以Reids协议追加保存每次写的操作到文件末尾。Redis还能对AOF文件进行后台重写，使得AOF文件的体积不至于过大。
#### Redis两种持久化方式优缺点？
* RDB持久化
优点：RDB文件紧凑，体积小，网络传输快，适合全量复制；恢复速度比AOF快很多。当然，与AOF相比，RDB最重要的优点之一是对性能的影响相对较小
缺点：RDB文件的致命缺点在与其数据快照的持久化方式决定了必然做不到实时持久化，而在数据越来越重要的今天，数据的大量丢失很多时候是无法接受的，因此AOF持久化称为主流。此外，RDB文件需要满足特定格式，兼容性差。
* AOF持久化
与RDB持久化相对应,AOF的优点在于支持秒级持久化、兼容性好，缺点是文件大，恢复速度慢，对性能影响大
### 如何选择Redis持久化方式策略？
在介绍持久化策略之前，首先要明白无论是RDB还是AOF，持久化的开启都是要付出性能方面的代价的。对比RDB持久化，一方面是bdsave在进行fork操作时Redis主进程会阻塞，另一方面，子进程向硬盘写数据也会带来IO压力；对于AOF持久化，向硬盘写数据的频率大大提高（everysec策略下为秒级），IO压力更大，设置可能造成AOF追加阻塞文件。此外，AOF文件的重写与RDB的basave类似，会有fork时的阻塞和子进程的IO压力问题。相对来说，由于AOF向硬盘中写数据的频率更高，因此对Redis主进程性能的影响会更大。

在实际生产环境中，根据数据量、应用对数据的安全要求、预算限制等不同情况，会有各种各样的持久化策略；如完全不使用任何持久化，使用RDB或AOF一种，或同事开启RDB和AOF持久化等。此外，持久化的选择必须与Redis的主从策略一起考虑，因为主从复制与持久化同样具有数据备份的功能，而且主机master和从机slave可以独立的选择持久化方案。
### Redis集群方案该怎么做?都有哪些方案?

### Redis如何做内存优化
尽可能使用散列表（hashes），散列表（是说列表里面存储的数少）使用的内存非常小，所以你应该尽可能的将你的数据模型抽象到一个散列表里面，比如你的web系统中有一个用户对象，不要为这个用户的名称，姓氏，邮箱，密码设置单独的key，而是应该把这个用户所有信息存储到一张散列表中
### Redis回收进程是如何工作的
一个Client运行了新的命令，添加了新的数据，Redis会检查内存使用情况，如果大于maxmemory的限制，则根据设定好的策略进行回收

## RabbitMQ 

## MongoDB
### MongoDB中对多条记录做更新操作命令是什么？
1. 只更新第一条记录
```
db.swxx.update({"ZJHM":"xxxxxxxxxxxxxxxxxx"},{"ZJHM":"23060419730523301X"})
```
2. 更新多条的第四个参数，这时候需要用$set操作才能更新多条
```
db.swxx.update({"ZJHM":"xxxxxxxxxxxxxxxxxx"},{$set:{"ZJHM":"23060419730523301X"}},false,true)
```
* 参数1：筛选条件
* 参数2：更新哪些字段
* 参数3：如果没有筛选到符合条件的记录，是否需要将参数2插入到集合中，默认false，不插入
* 参数4：默认false，一次更新一条；true一次更新多条，此时参数2需要使用$set操作

### MongoDB如何才会拓展到多个shard里？

## 测试
### 编写测试计划的目的是
### 对关键词触发模块进行测试
### 其他常用笔试题目网址汇总
### 测试人员在软件开发过程中的任务是什么
### 一条软件Bug记录都包含了哪些内容？
### 简述黑盒测试和白盒测试的优缺点
### 请列出你所知道的软件测试种类，至少5项
### Alpha测试与Beta测试的区别是什么？
### 举例说明什么是Bug？一个bug report应包含什么关键字？

## 数据结构
### 数组中出现次数超过一半的数字-Python版
```Python
from collections import Counter

def MoreThanHalfNum_Solution(numbers):
    if not numbers: 
        return None
    res = list()
    count = Counter(numbers).most_common()
    for num in count:
        if num[1] > len(numbers) / 2:
            res.append(num[0])
        else:
            break
    return res
```

### 求100以内的质数
```Python
print(' '.join(['%s' % x for x in range(2, 101) if not [y for y in range(2, int(pow(x, 0.5) + 1)) if x % y == 0]]))
#或者
print(' '.join([str(i) for x in range(2, 101) if not [y for y in range(2, int(pow(x, 0.5) + 1)) if x % y == 0]]))
```
详见[求100以内的质数](https://javyxu.cn/leetcode/leetcode_prime/)

### 无重复字符的最长子串-Python实现
```Python
class Solution:
    def lengthOfLongestSubstring(self, s: str) -> int:
        res = 0
        if s is None or len(s) == 0:
            return res
        d = {}
        tmp = 0
        start = 0
        for i in range(len(s)):
            if s[i] in d and d[s[i]] >= start:
                start = d[s[i]] + 1
            tmp = i - start + 1
            d[s[i]] = i
            res = max(res, tmp)
        return res
```
详见[无重复字符的最长子串](https://javyxu.cn/leetcode/leetcode_longest_substring/)

### 通过2个5和6升得水壶从池塘得到3升水
```Python
class Solution:

```

### 什么是MD5加密，有什么特点？
**MD5** 即Message-Digest Algorithm 5（信息-摘要算法5），用于确保信息传输完整一致。是计算机广泛使用的杂凑算法之一（又译摘要算法、哈希算法），主流编程语言普遍已有MD5实现。将数据（如汉字）运算为另一固定长度值，是杂凑算法的基础原理。

**MD5算法具有以下特点：**
* 压缩性：任意长度的数据，算出的MD5值长度都是固定的。
* 容易计算：从原数据计算出MD5值很容易。
* 抗修改性：对原数据进行任何改动，哪怕只修改1个字节，所得到的MD5值都有很大区别。
* 强抗碰撞：已知原数据和其MD5值，想找到一个具有相同MD5值的数据（即伪造数据）是非常困难的。

MD5的作用是让大容量信息在用数字签名软件签署私人密钥前被”压缩”成一种保密的格式（就是把一个任意长度的字节串变换成一定长的十六进制数字串）。

### 什么是对称加密和非对称加密
**对称加密** 其实总体上来说，对称加密就是在一组人当中相互传文件以打暗号的方式，比如我们约定a用###表示，b用￥￥表示，有这样的一个一一对应的规则在这，我们收到密文之后，只需要根据这张表去寻找对应的字母就可以把暗文转化成明文，叫对称加密，symmetric key encrytion。
原因是总体格式如下：明文<-->密钥<-->密文在这里，明文经过密钥以后就会加密成密文。

**非对称加密** 有个坏处就是，万一有不怀好意的人获取了加密的规则，也就是钥，那么密文很自然就能破解了，因此风险比较高。
对应的非对称加密是采用“公钥和私钥”方式，也就是比如张三要给李四发一份文件，那么就要询问李四的公钥，按照李四的公钥去加密这份文件，而这份文件也只能由李四的私钥去解密。
在这里：
每个人的公钥和私钥是一一对应的，特定的私钥能解特定的公钥。
公钥是可以公开的，相当于给某个特定的人（比如“李四”）解密的特定的锁头，而这个锁头也只有这个人（“李四”）的私钥也就是钥匙才能打开。
总体大概关系就是这样。

### 冒泡排序的思想？
冒泡排序的基本思想就是：从无序序列头部开始，进行两两比较，根据大小交换位置，直到最后将最大（小）的数据元素交换到了无序队列的队尾，从而成为有序序列的一部分；下一次继续这个过程，直到所有数据元素都排好序。

算法的核心在于每次通过两两比较交换位置，选出剩余无序序列里最大（小）的数据元素放到队尾。

### 快速排序的思想？
通过一趟排序将要排序的数据分割成独立的两部分，其中一部分的所有数据都比另外一部分的所有数据都要小，然后再按此方法对这两部分数据分别进行快速排序，整个排序过程可以递归进行，以此达到整个数据变成有序序列。
```Python
def quick_sort(data):    
    """快速排序"""    
    if len(data) >= 2:  # 递归入口及出口        
        mid = data[len(data) // 2]  # 选取基准值，也可以选取第一个或最后一个元素        
        left, right = [], []  # 定义基准值左右两侧的列表        
        data.remove(mid)  # 从原始数组中移除基准值        
        for num in data:            
            if num >= mid:                
                right.append(num)            
            else:                
                left.append(num)        
        return quick_sort(left) + [mid] + quick_sort(right)    
    else:        
        return data
 
# 示例：
array = [2,3,5,7,1,4,6,15,5,2,7,9,10,15,9,17,12]
print(quickSort(array))
# 输出为[1, 2, 2, 3, 4, 5, 5, 6, 7, 7, 9, 9, 10, 12, 15, 15, 17]
```

### 如何判断单向链表中是否有环？

### 你知道哪些排序算法（一般是通过问题考算法）

### 斐波那契数列
```Python
# F[n]=F[n-1]+F[n-2](n>=3,F[1]=1,F[2]=1)
def fibonacci_sequence(n):
    if n <= 0:
        return 0
    elif n == 1:
        return 1
    else:
        return fibonacci_sequence(n - 1) + fibonacci_sequence(n - 2)
```

### 如何翻转一个单链表？

### 青蛙跳台阶问题

### 两数之和Two Sum
```Python
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        res = dict()
        for index, num in enumerate(nums):
            another_num = target - num
            if another_num in res:
                return [res[another_num], index]
            res[num] = index
        return None
```
详见[两数之和](https://javyxu.cn/leetcode/leetcode_two_sum/)

### 搜索旋转排序数组(Search in Rotated Sorted Array)
```Python
```

### Python实现一个Stack的数据结构
栈（有时称为“后进先出栈”）是一个项的有序集合，其中添加移除新项总发生在同一端。这一端通常称为“顶部”。与顶部对应的端称为“底部”。

栈的底部很重要，因为在栈中靠近底部的项是存储时间最长的。最近添加的项是最先会被移除的。这种排序原则有时被称为LIFO，后进先出。它基于在集合内的时间长度做排序。较新的项靠近顶部，较旧的项靠近底部。
```Python
class Stack:
    def __init__(self):
        self.items = []

    def isEmpty(self):
        retun self.items == []
    
    def push(self, item):
        self.items.append(item)
    
    def pop(self):
        return self.items.pop()
    
    def peek(self):
        return self.items[len(self.times) - 1]

    def size(self):
        return len(self.items)
```

### 写一个二分查找
有序列表对于我们的比较是很有用的。在顺序查找中，当我们与第一个项进行比较时，如果第一个项不是我们要查找的，则最多还有`n-1`个项目。 **二分查找**从中间项开始，而不是按顺序查找列表。 如果该项是我们正在寻找的项，我们就完成了查找。如果它不是，我们可以使用列表的有序性质来消除剩余项的一半。如果我们正在查找的项大于中间项，就可以消除中间项以及比中间项小的一半元素。如果该项在列表中，肯定在大的那半部分。然后我们可以用大的半部分重复这个过程。从中间项开始，将其与我们正在寻找的内容进行比较。再次，我们找到元素或将列表分成两半，消除可能的搜索空间的另一部分
1. 方案一
```Python
def binarySearch(alist, item):
    start = 0
    end = len(alist) - 1
    found = False

    while start < end and not found:
        mid = (start + end ) // 2
        if alist[mid] == item:
            found = True
        else:
            if item < alist[mid]:
                last = mid - 1
            else:
                start = mid + 1

    return found  
```

2. 方案二
```Python
def binarySearch(alist, item):
    if alist is None:
        return False
    mid = len(alist) // 2
    if alist[mid] == item:
        return True
    else:
        if item < alist[mid]:
            binarySearch(alist[:mid], item)
        else:
            binarySearch(alist[mid+1:], item)
```

### set用in时间复杂度是多少，为什么？
时间复杂度为: `O(1)`
内部实现是dict的

### 列表中有n个正整数范围在[0，1000]，进行排序
```Python
test = [1, 3, 5, 6, 10, 99, 100, 0, 999, 777]
sorted(test)

test.sort()
```

### 面向对象编程中有组合和继承的方法实现新的类
组合指的是，在一个类中以另外一个类的对象作为数据属性，称为类的组合

## 大数据
### 找出1G的文件中高频词

### 一个大约有一万行的文本文件统计高频词

### 怎么在海量数据中找出重复次数最多的一个？

### 判断数据是否在大量数据中

给了三张表，按照题目要求，写了三个涉及关联查询，子查询，组函数用HAVING做过滤而不是WHERE，分组统计，
建临时表，把几个查询语句合起来
索引为何选B树，B+树，不选二叉树，
### 事务的ACID
[参考OLTP和OLAP的关系](https://javyxu.cn/bigdata/oltp_olap_doc/)
传统关系型数据库和非关系型数据库HBASE的区别（着重和我聊了ROWKEY，ROWKEY怎么选的？过长和过热的问题？）
数据库数据改变后怎么获取哪些数据改变了，哪些没改变
范式
HBASE删除数据怎么搞得（时间戳切入）
实际问题，堆排解决，然后讲了一遍，包括时间空间复杂度，他说你很熟悉堆排，那么让你写快排？最大最小时间复杂度多少？为何是这个？

HIVE里面的东西，怎么玩HIVE
项目里面怎么离线处理离线数据的？
数据量多大？
基于磁盘离线处理和基于内存处理海量数据的区别？
MAPREDUCE和HIVE区别？HIVE的外部表和内部表？
我说我比较拿手离线的MAPREDUCE代码，他要我讲了MAPREDUCE的10个步骤（董西成深入理解系列里面有）
怎么优化？
磁盘IO你觉得MR里面哪里最大？
我设计模式都讲一遍，选个你拿手的写一下。集合，HASHMAP源码给他讲一下？预留数多少？怎么扩容？对性能影响？
写了算法，好像是有序数组求2个数的差值绝对值最大数，
还有个二叉树镜像。
然后问我如果公司的东西都学习完了，你该怎么办，会不会觉得工作比较无聊？然后就放我过了。

1 TCP/IP/UDP？
2 HTTP/HTTPS？
3 HTTP1.0和1.1区别？
4 COOKIE和SEEION


1 HBASE为何能海量存储，ORACLE为何不行，底层什么形式存在HDFS上？
2 HBASE和HDFS区别？
3 HADOOP1.0和2.0区别？（4点）
4 NAMENODE的HA？
5 槽位数的共享问题？需要注意什么？（REDUCE SLOT提前启动和MAPSLOT饿死）
6 ZK的LEADER选举算法？
7 如何设置优先级？
8 2.0如何资源调度？
9 HIVE和MAPREDUCE区别？
10 怎么优化？
11 HADOOP1.0和2.0HDFS的BLOCK各为多少？

## 机器学习和深度学习
cnn

