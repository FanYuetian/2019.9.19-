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
9.
