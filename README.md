# 2019.9.19-牛客网知识补充
1.executeUpdate(sql)用于执行给定的SQL语句，可以是增删改查或者不返回任何内容的SQL语句，返回值是更新的条数；executeQuery(sql)被用来执行select语句，返回代表查询结果的resultset对象
2.java屏幕左上角被确定为坐标起点
3.在一个静态方法中可以调用本类的静态方法，直接调用；在静态方法中可以通过创建对象，通过对象调用静态方法
4.依赖注入的目的是减少组件之间的耦合度，使开发变得简单；在系统运行中，动态向某个对象提供它所需要的其他对象；依赖注入能够独立开发组件，然后根据组件间的关系进行组装；依赖注入提供使用接口编程
5.继承重写，子类访问修饰符>=父类
6.finally语句块是在try或catch中的return语句之前执行
  try{ return i; }finally{ i++; } -> i=1;
7.垃圾回收机制
  Xmx：JVM最大可用；Xms：JVM初始内存；Xmn：年轻代大小；XX:SurvivorRatio(eden:from:to 8:1:1)=3(3:1:1)
8.java语言中：关于字符集编码和国际化问题
             java一律采用Unicode编码，每个字符无论中文还是英文都占用2个字节
             不同编码之间的转换：将字符串以其自身编码方式分解为字节数组，再将字节数组以你想要输出的编码方式重新编码为字符串；String newUTF8Str = new String(oldGBKStr.getBytes("GBK"),"UTF8");
             java虚拟机中通常使用UTF-16方式保存一个字符
             resourceBundle能根据local不同，选择性读取与local对应后缀的properties文件，达到国际化目的
             
9.构造函数不能声明返回类型，不能用private修饰
10.静态变量未被final时，它的值可以改变
11.引用类型都是直接或间接继承自object，基本类型在赋值时会先自动装箱成其相对应的包装类，然后赋值。
12.web容器是一种服务程序，在服务器一个端口就有一个提供相应服务的程序，而这个程序就是处理从客户端发出的请求，java中的tomcat，一个服务器可以有多个容器。
13.存储结构不属于算法结构
14.数组是一个对象，不同类型的数组具有不同的类；数组长度是固定的；数组是一种引用数据类型，肯定继承object类，所以里面有equals()方法，但是肯定没有重写过，因此并不是比较数组内的内容，使用Arrays.equals()是比较两个数组中的内容

15.接口中定义的成员为常量，方法不能有方法体
16.subset(from,true,to,true)是Treeset的非静态方法，该方法返回从from元素到to元素的一个set集合，两个Boolean类型确认是否包含边境值
17.protected：自身、子类及同一个包中类可以访问
18.round 四舍五入往大数方向入
19.java中，赋值是有返回值的，赋什么值，就返回什么值；C中，赋值后会与0比较，如果大于0就认为是true，java不会与0比较，而是直接把赋值后的结果放入括号中（ if(x=y) ）
20.RandomAccessFile可以附加或更新文件
21.标识符由数字、字母、下划线、美元符号组成；首位不能是数字，标识符不能是关键字
22.
