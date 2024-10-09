---
title: Java考试题目汇总
---

答案均由搜题软件搜出，不一定正确，欢迎[反馈](https://qm.qq.com/cgi-bin/qm/qr?k=GtIKywDddJguGtKz8TjrFOCw-DWsKJkT&noverify=0)

<!-- more --><!-- more -->

### 选择题

设有定义：String s =“World”;，下列语句错误的是（ ）。

A char c = s.charAt(0);

B int m = s.indexOf(‘r’);

C int n = s.length( );

**D String str = s.append(‘2’);**

---

在Java中，"456"属于（ ）类的对象。

A Integer **B String** C Number D int

---

下列对封装性的描述中，错误的是( )

A 封装体包含了属性和行为

**B 封装体中的属性和行为的访问权限是相同的**

C 被封装的某些信息在封装体外是不可见的

D 封装使得抽象的数据类型提高了可重用性

---

给出下面代码段, （ ）行将引起一个编译时错误？

```java
public class Test { 
	int n = 0;
	int m = 0;
	public Test(int a) {m=a;} 
public static void main(String arg[]) {
	Test t1,t2;
	int j,k;
	j=3; k=5;
	t1=new Test();
	t2=new Test(k);
	} 
}
```

A 行6 B 行1 C 行4 **D 行9**

---

```java
public class Increment {
	public static void main(String args[]) {
	int c;
	c = 2;
	System.out.println(c);
	System.out.println(c++);
	System.out.println(c);
	}
}
```

运行结果是：（ ）

**A 2 2 3**

B 3 4 4

C 2 3 3

D 2 2 2

---

在创建对象时必须（ ）

A 先声明对象，然后才能使用对象
B 先声明对象，为对象分配内存空间，然后才能使用对象
**C 先声明对象，然后才能使用对象**
D 先声明对象，为对象分配内存空间，对对象初始化，然后才能使用对象

---

如果希望某个变量只可以被类本身访问和调用，则应该使用下列( ) 访问控制修饰。

**A private**

B protected

C default

D public

---

指出下列程序运行的结果 （ ）

```java
public class Example{
	String str=new String("good");
	char[] ch = {'a','b','c'};
	public static void main(String args[]){
		Example ex=new Example();
		ex.change(ex.str,ex.ch);
		System.out.print(ex.str+" and ");
		Sytem.out.print(ex.ch);
	}
	public void change(String str,char ch[]){
		str="test ok"; ch[0]='g';
	}
}
```

A test ok and abc

**B good and gbc**

C good and abc

D test ok and gbc

---

下面（ ）操作符的优先级最高？

**A ( )**
B ||
C &&
D !

---

下面的代码片段实现的是什么功能？( )

```java
File file = new File("C:\\test.dat");
if (file.exists()) {
	file.delete();
}
```

A 移动C:\test.dat
B 创建C:\test.dat
**C 删除C:\test.dat**
D 打开C:\test.dat文件输出流

---

getCustomerInfo()方法如下, try中可以捕获三种类型的异常, 如果在该方法运行中产生了一个IOException ,将会输出( )

```java
public void getCustomerInfo()
{
	try{
		//一些可以引起异常的语句
	} catch (java.io.FileNotFoundException ex){
		System.out.print("FileNotFoundException!");
	} catch (java.io.IOException ex) {
		System.out.print("IOException!");
	}catch (java.lang.Exception ex) {
		System.out.print("Exception!");
	}
}
```

A IOException!Exception!

B FileNotFoundException!IOException!

**C IOException!**

D FileNotFoundException!IOException!Exception!

---

设有定义 float x=3.5f, y=4.6f, z=5.7f；则以下的表达式中，值为true的是( )

**A x != y**
B x > y || x > z
C z > ( y + x )
D x < y & ! ( x < z )

---

Java源文件中最多只能有一个（）类，其他类的个数不限。

A interface
B abstract
C final
**D public**

---

定义有如下的方法:

abstract void performDial( );

该方法属于( )。

A 接口方法

B 最终方法

C 空方法

**D 抽象方法**

---

下列关于for循环和while循环的说法中( )是正确的 ?

A 两种循环任何时候都可替换

**B while循环能实现的操作, for循环也都能实现**

C 两种循环结构中都必须有 循环体,循环体不能为空

D while循环判断条件一般是程 序结果, for循环判断条件一般是非程序结果

---

参照以下Java代码，以下四个叙述中最确切的是（　　　）

```java
class A{
	int x;
	static int y;
	void fac(String s){
		Syatem. out. println(＂字符串:＂+s);
	}
}
```

A x、y和s都是实例变量

**B x是实例变量、y是类变量、s是局部变量**

C x和y是实例变量、s是参数

D x、y和s都是成员变量

---

```java
int total = 0;
for ( int i = 0; i < 4; i++ )
{
	if ( i == 1) continue;
	if ( i == 2) break;
	total += i;
}
```

则执行完该程序段后total的值为（ ）。

**A 0**

B 6

C 1

D 3

---

下面的方法,当输入为2的时候返回值是( )

```java
public int getValue(int i) {
	int result = 0;
	switch (i) {
	case 1:result = result+i;
	case 2: result= result+i*2;
	case 3: result= result+i*3;
	}
	return result;
}


```

A 4

B 2

C 0

**D 10**

---

指出正确的表达式 （ ）

A double d = 0.9239d;

**B long l = 0xfffL;**

C Boolean b = null;

D byte a = 128;

>解析：
>
>A.没变量名
>
>B.没错，类型有、变量名有、赋值没错
>
>C.boolean 类型只能赋值 true 或者false。而这里的Boolean应该是boolean类型的包装类，Boolean类型时可以被赋值为null的。所以此选项缺少变量名
>
>D.byte赋值范围为-128~127

---

下面语句在编译时不会出现警告或错误的是( )

A Boolean b = null;

B int i = 10.0;

C char c =" C";

D float f = 3.14;

>全错？

---

关于被私有访问控制符private修饰的成员变量，以下说法正确的是（ ）

**A 只能被该类自身所访问和修改**

B 可以被两种类访问和引用：该类本身、该类的所有子类

C 只能被同一个包中的类访问

D 可以被三种类所引用：该类自身、与它在同一个包中的其他类、在其他包中的该类的子类

---

类Test1定义如下：

```java
1public class Test1{
2	public float aMethod（float a，float b）{ }
3
4}
```
将以下（ ）方法插入行3是不合法的。
A public int aMethod（int a， int b）{ }

**B public float aMethod（float c，float d）{ }**

C private float aMethod（int a，int b，int c）{ }

D public float aMethod（float a， float b，float c）{ }

---

类Test1、Test2定义如下：

```java
1public class Test1
2{
3	public float aMethod（float a，float b） throws IOException { }
4}
5	public class Test2 extends Test1{
6
7}
```

将以下（ ）插入行6是不合法的。

A public int aMethod（int a，int b）throws Exception{ }
B public float aMethod（float p，float q）{ }
**C float aMethod（float a，float b）{ }**
D public int aMethod（int a，int b）throws IOException{ }

---

关于以下程序代码的说明正确的是（ ）

```java
1class HasStatic{
2 	private static int x=100;
3 	public static void main(String args[ ]){
4 		HasStatic hs1= new HasStatic( );
5 		hs1.x++;
6 		HasStatic hs2=new HasStatic( );
7		hs2.x++;
8 		hs1=new HasStatic( );
9	 	hs1.x++;
10		HasStatic.x- -;
11		System.out.println(“x=”+x);
12	}
13}
```

A 5行不能通过编译，因为引用了私有静态变量
B 10行不能通过编译，因为x是私有静态变量
**C 程序通过编译，输出结果为：x=102**
D 程序通过编译，输出结果为：x=103

---

执行语句int i = 1, j = ++i; 后i与j的值分别为（ ）。

A 2与1
**B 2与2**
C 1与1
D 1与2

---

在调用方法时,若要使方法改变实参的值,可以( )

**A 用对象作为参数**

B 用基本数据类型作为参数

C 用String类型做参数

D使用对象的数据域做参数

---

在Java中，在包com.db下定义一个类，要让包com.util下的所有类都可以访问这个类，这个类必须定义为（ ）

**A public**
B default
C protected
D private

---

关键字supper的作用，叙述错误的是（ ）

**A 用来调用父类中被重载的方法**
B 用来调用父类的构造函数
C 用来调用父类的私有方法
D 用来访问父类被隐藏的成员变量

---

下列关于异常处理的描述中，错误的是( )

**A 捕获到的异常只能在当前方法中处理，不能在其他方法中处理**
B 使用throw语句抛出异常
C 使用try-catch-finally语句捕获异常
D 程序运行时异常由Java虚拟机自动进行处理

---

下列（ ）是合法的Java标识符？

A theLastOne

B Tree&Glasses

C 273.5

**D FirstJavaApplet**

---

以下声明合法的是( )

**A public final static int w() ;**

B abstract double d ;

C abstract final double hyperbolicCosine();

D default String s ;

---

下面不是合法标识符的是( )

A $d2000_

B whataQuiz

C giveMes

**D 2ofUS**

---

在Java的类库中,包含实现输入输出操作的包是( )

**A java.io**

B java.awt

C java.util

D java.applet

---

声明成员变量时,如果不使用任何访问控制符(public, protected, private) ,则以下( ) 类型的类不能对该成员进行直接访问。

**A 不同包中的子类**

B 同一包中的子类

C 同一包中的非子类

D 同一类

---

下面声明数组的写法错误的是（ ）。

A int[ ] a;
B int[ ] a = {1，2，3};
**C int[3][ ] a;**
D int a[ ];

---

java语言中，负责并发管理的机制是（）

**A 多线程**
B 虚拟机
C 字节码
D 垃圾回收

---

执行完 int[ ] x=new int[10]；后，正确的是（ ）

A x[9]未定义
B x[0]为空
**C x[9]为0**
D x[10]为0

---

Java语言中，只限子类或者同一包中的类的方法能访问的访问权限是( )

A public
B 无修饰即缺省的访问控制修饰符
C private
**D protected**

---

()是构成Java程序的基本单位

A 对象 **B 类** C main方法 D 方法

---

在Java中，下列（ ）语句不能通过编译。

A float f = 5 + 5.5;
B String s= “join”+ 3;
C String s= “join”+ “was”+ “here”;
**D int a = 3 + 5;**

---

下列（ ）类的声明是正确的？

A abstract final class HI{ }
**B public abstract class Car{ }**
C abstract private move(){ }
D protected private number;

---

下述概念中不属于面向对象方法的是（ ）。

A 继承、多态
B 类、封装
**C 过程调用**
D 对象、消息

---

在switch语句中, switch后面括号内的表达式的类型不能是( )

A byte

B int

C char

**D long**

---

以下关于构造函数的描述错误的是（ ）。

A 一般在创建新对象时，系统会自动调用构造函数。
**B 构造函数的返回类型只能是void型。**
C 构造函数的主要作用是完成对类的对象的初始化工作。
D 构造函数是类的一种特殊函数，它的方法名必须与类名相同。

---

A派生出子类B，B派生出子类C，并且在Java源代码中有如下声明：

```java
A a0=new A();

A a1=new B();

A a2=new C();
```

问以下（ ）说法是正确的

A 第1、2、3行能通过编译，但第2、3行运行时出错
**B 第1行、第2行和第3行的声明都是正确的**
C 只有第1行能通过编译
D 第1、2行能通过编译，但第3行编译出错

---

下列语句序列执行后

```java
int i=10, j=18, k=30;
switch( j - i ) {
	case 8 : k++;
	case 9 : k += 2;
	case 10: k += 3;
	default : k /= j;
}
```

k的值是( )
**A 2**
B 31
C 3
D 33

---

Java语言的许多特点中，下列（）特点是C++语言所不具备的。

A 高性能
**B 跨平台**
C 有类库
D 面向对象

---

在Java中用( ) 关键字修饰的方法可以直接通过类名来调用。
A void
**B static**
C final
D private

---

为AB类的一个无形式参数无返回值的方法method书写方法头，使得使用类名AB作为前缀就可以调用它，该方法头的形式为( )。

**A static void method( )**
B public void method( )
C final void method( )
D abstract void method( )

---

下面是People和Child类的定义和构造方法，每个构造方法都输出编号在执行new Child("mike")的时候都有哪些构造方法被顺序调用?
请选择输出结果()

```java
class People {
String name;
public People(){ System.out.print(1);
}
	public People(String name) {
		System.out.print(2);
this.name = name;
	}
}
class Child extends People {
	People father;
public Child(String name) {
	System.out.print(3);
	this.name= name;
	father= new People(name + ":F");
}
public Child(){
	System.out.print(4);
	}
}

```

**A.312** B.32 C.13 D.132

---

在Java中如果父类中的某些方法不包含让任何逻辑，并且并且需要子类重写，可以用()关键字来声明父类中的这些方法

A.final B.static C.void **D.abstract**

---

以下关于继承的叙述正确的是()
**A 在Java中类只允许单一继承**
B 在Java中一个类只能实现一个接口
C 在Java中一个类不能同时继承一个类和实现一个接口
D 在Java中接口只允许单一继承

> 解析:该题考查的是类的继承。继承分为单继承和多继承两种形式。单继承允许一个类可以有多个子类，但只能有一个父类;多继承则允许一一个类不仅可以有多个子类，还可以有多个父类。但需要注意- -点，Java只支持单继承，但可以通过接口实现多继承的功能。一个类可以同时继承一个类和实现一个接口。所以选项A是正确的。

---

下列属于合法的Java标识符是()

**A.cat** B.5books C.+static D.-3.14159

---

有语句String s="hello world";，以下操作不合法的是()
A int i=s.length();
**B s>>>=3;**
C String s=s.trim();
D String t=s+"!";

---

java语言的类间的继承关系是（）

A 不能继承
B 多重的
**C 单重的**
D 线程的

---

执行语句int i=1,j=++i;后i与j的值分别为()

A 2与1

B 1与1

**C 2与2**

D 1与2

---

下面( )行代码正确的声明了一个类方法(静态方法)

A public int method(inti)

B protected method(int i)

C public static method(Strings)

**D public static void method(lnteger i)**

---

分析如下的java代码段,( )编译没有异常和错误

A. byte b=257; B. boolean b=null; C. float f=1.3; **D. int i=12;**

---

假设方法unsafe()将抛出lOException,请问可将以下()可以第1行

```java
{if(unsafe(){//do something..}
 else if (safe()){//do the other..}
}
```

A public IOException methodName()
B public void methodName()
**C public void methodName() throws IOException**
D public void methodName() throw IOException

---

下面程序定义了一个类，关于该类说法正确的是( )。
abstract class abstract Class{}
关于该类说法正确的是()
A 该类不能被继承
B 该类的方法不能被重载
C 该类能调用new abstractClass()方法实例化为一个对象
**D 该类中可以有普通的方法**

---

欲构造ArrayList类的一个实例，此类继承了List接口，下列( )是正确的

A ArrayList myList=new Object( );

B ArrayList myList=new List( );

**C List myList=new ArrayList( );**

D List myList=new List( );

---

下列关于包的描述中,错误的是()

**A 包是一种特殊的类**

B 包是若干个类的集合

C 包是使用package语句创建的

D 包有有包名包和无名包两种

---

有一段java应用程序，它的主类名是a1，那么保存它的源文件名可以是()。

**A. a1.java** B. a1.class C. a1 D.a.jsp

---

若a的值为3时，执行

```java
if (a>0)
if (a>3) 
c=2; 
elsec=3; 
elsec=4;
```

c的值是多少? ()
A.1 B.2 **C.3** D.4

---

若需要定义一个类的作用域或类中使用的方法应使用 ()修饰符。

A private

B public

C package

**D static**

---

下面（）行代码正确的声明了一个类方法（静态方法）

A protected method(int i)

B public static method(Strings s)

C public int method(int i)

**D protected static void method(Integer i)**

---

有以下方法的定义请选择该方法的返回类型

```java
ReturnType method(byte x,double y){
	return (short)x/y*2;
}
```

A int

**B double**

C int

D short

---

在Java中,一个类可同时定义许多同名的方法，这些方法的形式参数个数，类型或顺序各不相同，传回的值也可以不相同。这种面向对象程序的特性称为（）

A 隐藏

B 覆盖

C Java不支持此特性

**D 重载**

---

一个可以独立运行的Java应用程序（ )

A 最多只能有两个main( )方法

**B 只能有一个main( )方法**

C 可以有一个或多个main( )方法

D 可以有一个或零个main( )方法

---

下列关于包的描述中，错误的是（）

A 包是使用package语句创建的

B 包有有名包和无名包两种

C 包是若干个类的集合

**D 包是一种特殊的类型**

---

假设在Java源程序文件“MvClassiava”中只含有一个类,而且这个类必须能够被位于个庞大的软件系统中的所有Java类访问到,那么下面()声明有可能是符合要求的类声明。

A private class MyClass extends Object

B public class myclass extends Object

**C public class MyClass**

D class MyClass extends Object

---

```java
public class foo{
	public static void main(String[] args){
		String s;
		System.out.println("s="+s);
	}
}??
```

输出结果应该是：
A 代码得到编译，但捕获到NullPointException异常
B 代码得到编译，并输出"s="
C 由于Strings没有初始化，代码不能编译通过
**D 代码得到编译，并输出"s=null"**

---

整型数据类型中，需要内存空间最少的是（)

A.int B.long C.short **D.byte**

---

在java中（）关键宇用于终止语句

A continue

**B break**

C exit

D return

---

下列说法不正确的是

A 一个子类的对象可以接收父类对象能接收的消息

B 当子类对象和父类对象能接收同样的消息时，它们针对消息产生的行为可能不同

**C 父类比它的子类的方法更多**

D 子类在构造函数中可以使用super( )来调用父类的构造函数

---

下面（）循环会导致死循环？

A for(int k=0;k<0;k++)

B for(int k=0;k>0;k++）

C for(int k=10;k>0;k--)

**D for(int k=0;k<10;k--)**

---

Java为移动设备提供的平台是（ )

A JDK6

**B Java ME**

C Java SE

D Java EE

---

```java
int a=b=5;
String s1="祝你今天考出好成绩!";
String s2 = s1;
```

则表达式a==b与s2==s1的结果分别是:( )
**A.true与true**

B.false与true

C.true与false

D.false与false

---

有语句String s="hello world";以下操作（）是不合法的？

**A s>>>=3 ;**

B String t=s+"!";

C String ts =s.trim;

D int i=s.length();

---

设i、j为int型数组变量名，a为int型数组名，以下选项中，正确的赋值语句是()
A i=i+2

**B a[0]=7;**

C i++---j;

D a(0)=66;

---

### 判断题

接口里不能定义成员变量。

**✅**对

**⬜**错

equals()方法只有在两个对象的内容一致时返回true

**⬜**对

**❌**错

父类的构造方法不可以被子类继承

**✅**对

**⬜**错

构造方法一般不允许有任何返回值，因此需要在构造方法返回类型处标注为void

**⬜**对

**❌**错

抽象方法必须在抽象类中，所以抽象类中的方法都必须是抽象方法，不能包含带有方法体的具体方法

**⬜**对

**❌**错

Java的源代码中定义几个类，编译结果就生成几个以“.class”后缀的字节码文件。

**✅**对

**⬜**错

switch语句中可以没有default子句。

**✅**对

**⬜**错

maxElements是一个成员变量，声明为:public static final int maxElements=100;

**✅**对

**⬜**错

如果p是父类Parent的对象，而c是子类Child的对象，则语句c = p是正确的。

**⬜**对

**❌**错

异常处理中总是将可能产生异常的语句放在try块中，用catch子句去处理异常，而且一个try块之后只能对应一个catch语句。

**⬜**对

**❌**错

当声明一个类时，如果用户定义了一个带参数的构造方法，那么系统还会提供给用户一个无参数的构造方法。

**⬜**对

**❌**错

用“+”可以实现字符串的拼接，用“-” 可以从一个字符串中去除一个字符子串。

**⬜**对

**❌**错

Java的各种数据类型所占用的内存长度与具体软硬件环境有关。

**⬜**对

**❌**错

在Java的方法中定义一个常量要用const关键字。

**⬜**对

**❌**错

在Java中，关键字final修饰一个类后，该类就不能派生出子类。

**✅**对

**⬜**错

在接口中定义的方法都只能是没有方法体的抽象方法。

**✅**对

**⬜**错

假设文件"a.txt"的长度是100字节，那么当正常运行语句OutputStream f= new FileOutputStream(new File("a.txt"));后，文件a.txt 的长度变为0字节。

**✅**对

**⬜**错

垃圾收集的过程在Java程序的生存期中式自动的，不需要分配和释放内存，也避免了内存泄露。

**✅**对

**⬜**错

如果再定义一个类的时候没有用到关键字extends，则这个类没有直接父类。

**⬜**对

**❌**错

子类覆盖父类的方法时，权限不能比父类的权限小。

**✅**对

**⬜**错

用“+”可以实现字符串的拼接，用“-” 可以从一个字符串中去除一个字符子串。

**⬜**对

**❌**错

### 填空题

方法int numberOfDigits(int n)的功能是计算十进制正整数n的位数。

```java
int numberOfDigits(int n){
	int c=0;
	do{
		n = ______________;
		c++;
	}
	while(______________);
	return c;
}
```

{% copy n / 10 %}

{% copy n != 0 %}

{% folding child:codeblock open:false color:cyan 测试代码如下 %}

```java
public class test{
	static int numberOfDigits(int n){
		int c=0;
		do{
			n = n/10;
			c++;
		}
		while(n!=0);
		return c;
	}
	public static void main(String[] args) {
		System.out.println(numberOfDigits(1234));
	}
}
```

{% endfolding %}

---

子类SubClass求x的n次方。

```java
class SuperClass {
	float x;
	int n;
	SuperClass( float x , int n ) {
	this.x = x ;
	this.n = n;
	}
}
class SubClass extends SuperClass {
	SubClass( float x , int n ) {
		______________;
	}
	double exp( ) {
		double s = 1.0;
		for ( int i = 1; i<=n; i++ ) {
		s =______________;
		}
		return s;
	}
}
```

{% copy super ( x , n ) %}
{% copy s * x %}
{% folding child:codeblock open:false color:cyan 测试代码如下 %}

```java
class SuperClass {
	float x;
	int n;
	SuperClass( float x , int n ) {
	this.x = x ;
	this.n = n;
	}
}
class SubClass extends SuperClass {
	SubClass( float x , int n ) {
		super(x, n);
	}
	double exp( ) {
		double s = 1.0;
		for ( int i = 1; i<=n; i++ ) {
		s =s*x;
		}
		return s;
	}
}
public class test{
	public static void main(String[] args) {
		SubClass a = new SubClass(5,3);
		System.out.print(a.exp());
	}
}
```
{% endfolding %}

---

有一对免子，从出生后第3个月起每个月都生对兔子 ，小兔子长到第三个月后每个月又生一对兔子，假如兔子都不死，问每个月的兔子总数为多少?

```java
int fibonacci (int m) {
int f1= 1,f2= 1,f;
	for(int i=3;______________;i++){
	f = f2;
	f2 = ______________;`
	f1= f;
	System.out.println("第" + i +"个月的免子对数: "+f2);
	}
}
```

{% copy i <= m %}
{% copy f2 + f1 %}
{% folding child:codeblock open:false color:cyan 测试代码如下 %}

```java
public class test{
	static void fibonacci (int m) {
		int f1= 1,f2= 1,f;
			for(int i=3;i<=m;i++){
			f = f2;
			f2 =f2+f1+1;
			f1= f;
			System.out.println("第" + i +"个月的免子对数: "+f2);
			}
		}
	public static void main(String[] args) {
		fibonacci(10);
	}
}
```
{% endfolding %}

---

程序获取当前日期,将日期字符串输出;
截取日期字符串中从第11位开始到字母C之前的字符串，并输出

```java
public class Class1{
public static void main(Srting args[]){
	Date date1=new Date();
	System. out. println(datel);
	String t=datel.toString0;
	int endPos =______________;
	t=______________;
	System. out.println(t);
	}
}
```

{% copy 11 %}
{% copy t.substring(endPos,t.indexOf('C')) %}
{% folding child:codeblock open:false color:cyan 测试代码如下 %}

```java
import java.util.Date;
public class Test2007210530{
	public static void main(String args[]){
        Date date1=new Date();
        System.out.println(date1);
        String t=date1.toString();
        int endPos =11;
        t=t.substring(endPos,t.indexOf('H'));
        System. out.println(t);
	}
}
```
{% endfolding %}

---

方法void primeNumber(int n )将一个正整数分解质因数。例如：输入90，打印出2\*3\*3\*5。

```java
void primeNumber(int n) {
	int k=2;
	System.out.print(n + "=" );
	while(k <= n){
		if(k==n){
			System.out.println(n);
			______________;
		}
		else if(n%k == 0) {
			System.out.print(k + "*");
			n=______________;
		}
		else k++;
	}
}
```

{% copy break %}
{% copy n / k %}
{% folding child:codeblock open:false color:cyan 测试代码如下 %}

```java
public class test{
	static void primeNumber(int n) {
		int k=2;
		System.out.print(n + "=" );
		while(k <= n){
			if(k==n){
				System.out.println(n);
				break;
			}
			else if(n%k == 0) {
				System.out.print(k + "*");
				n=n/k;
			}
			else k++;
		}
	}
	public static void main(String[] args) {
		primeNumber(10);
	}
}
```
{% endfolding %}

---

方法int maxDigit(int n)的功能是找出十进制整数n各位中最大的一位数字。例如，n=23765，该方法的返回值是7。

```java
static int maxDigit(int n){
	int c=0,d;
	while(n>0){
		d = ______________;
		if(d>c) c=d;
		n/=10;
	}
	______________;
}
```

{% copy n % 10 %}
{% copy return c %}
{% folding child:codeblock open:false color:cyan 测试代码如下 %}

```java
public class test{
	static int maxDigit(int n){
		int c=0,d;
		while(n>0){
			d = n%10;
			if(d>c) c=d;
			n/=10;
		}
		return c;
	}
	public static void main(String[] args) {
		System.out.println(maxDigit(23765));
	}
}
```

{% endfolding %}

---

方法 void MaxAndMin（int a[ ]）求数组中最大值和最小值。

```java
public void MaxAndMin(int a[]){
	int i,Max,Min;
	Max = Min =______________ ;
	for ( i = 1 ; i < a.length; i++) {
		if (______________)Min = a[i];
		if ( a[i]>Max ) Max = a[i];
	}
	System.out.println( Max+" "+Min );
	System.out.println( );
}
```

{% copy a[0] %}
{% copy a[i] < Min %}
{% folding child:codeblock open:false color:cyan 测试代码如下 %}

```java
//import java.util.Scanner;
public class test{
	public static void MaxAndMin(int a[]){
		int i,Max,Min;
		Max = Min =a[0] ;
		for ( i = 1 ; i < a.length; i++) {
			if ( a[i]<Min )Min = a[i];
			if ( a[i]>Max )Max = a[i];
		}
		System.out.println( Max+" "+Min );
		System.out.println( );
	}
    public static void main(String[] args){
        //Scanner sc=new Scanner(System.in);
		//String a[] = sc.nextLine().split(" ");
		//int n[] = new int[a.length];
		//for(int i=0;i<a.length;i++){
		//	n[i]=Integer.parseInt(a[i]);
		//}
		//MaxAndMin(n);
		MaxAndMin(new int[]{1, 2, 3});
        //int [] a = {1,2,3};
		//MaxAndMin(a);
	}
}
```

{% endfolding %}

---

方法void narcissistic（）打印所有的水仙花数。

"水仙花数 "是指一个三位数，其各位数字立方和等于该数本身。例如：153是一个 "水仙花数 "，因为153=1的三次方＋5的三次方＋ 3的三次方。

```java
void narcissistic(){
	int b1, b2, b3;
	for(int m=101; m<1000; m++) {
		b3 = m / 100;
		b2 = ______________;
		b1 = m % 10;
		if(______________ == m) {
			System.out.println(m+"是一个水仙花数"); 
		}
	}
}
```

{% copy m / 10 % 10 %}
{% copy b1 * b1 * b1 + b2 * b2 * b2 + b3 * b3 * b3 %}
{% folding child:codeblock open:false color:cyan 测试代码如下 %}

```java
public class test{
	static void narcissistic(){
		int b1, b2, b3;
		for(int m=101; m<1000; m++) {
			b3 = m / 100;
			b2 = m/10%10;
			b1 = m % 10;
			if(b1*b1*b1+b2*b2*b2+b3*b3*b3 == m) {
				System.out.println(m+"是一个水仙花数"); 
			}
		}
	}
	public static void main(String[] args) {
		narcissistic();
	}
}
```
{% endfolding %}

---

方法int sigmaEvenNum（int[]a）的功能是求已知数组中偶数的个数。

```java
static int sigmaEvenNum(int a[]){
	int s =0;
	for (______________) {
		if(______________)
		s++;
	}
	return s;
}
```

{% copy int i = 0 ; i < a.length ; i++ %}
{% copy a[i] % 2 == 0 %}
{% folding child:codeblock open:false color:cyan 测试代码如下 %}

```java
public class test{
	static int sigmaEvenNum(int a[]){
		int s =0;
		for (int i=0;i<a.length;i++){
			if(a[i]%2==0)
			s++;
		}
		return s;
	}
	public static void main(String[] args) {
		int a[]= {1,23,43,-36,4};
		System.out.println(sigmaEvenNum(a));
	}
}
```
{% endfolding %}

---

类Fact求n的阶乘，请将程序补充完整。

```java
class Fact {
	int n ;
	Fact( int n ) {
		______________;
	}
	int fact( ) {
		int f = 1;
		for (int i = 1; i <= n; i++ )
		f = ______________;
	return f;
	}
}
```

1. {% copy this.n = n %}
2. {% copy f * i %}

{% folding child:codeblock open:false color:cyan 测试代码如下 %}

```java
class Fact{
	int n ;
	Fact( int n ) {
		this.n=n;
	}
	int fact() {
		int f = 1;
		for (int i = 1; i <= n; i++ )
		f = f*i;
		return f;
	}
}
public class test{
	public static void main(String[] args) {
		Fact a=new Fact(10);
		System.out.print(a.fact());
	}
}
```

{% endfolding %}

---

### 简答题

类CountChar有方法int countNum(String str , char a),该方法的功能是找出给定字符a在字符串str中出现的次数。
例如,countNum("Welcome",'e')的返回值是2.
请上传源代码截图,截图需带类名和行号。类名用给定类名+学号命名,例如161007112王明, CountChar类名为CountChar161007112java ,其余类名依此规则定义。并将运行结果截图上传,运行结果需要带输出窗口的运行时间。
[最小截图工具.exe](https://api.dzzui.com/api/lanzoujx?url=https://mengchunm.lanzouw.com/i7mj203r320b&type=down)

```java
class CountChar{
	int countNum(String str,char a){
		int counts=0;
		for(int i=0;i<str.length();i++){
			if(str.charAt(i)==a)
			counts++;
		}
		return counts;
	}
}
public class Test2007210530{
	public static void main(String[] args) {
		CountChar a=new CountChar();
		System.out.println(a.countNum("Welcome",'e'));
		
	}
}
```

---

定义一个表示学生信息的类Student，要求如下：

1. 类Student的成员变量： sNO表示学号；sName表示姓名；sSex表示性别；sAge表示年龄；sJava：表示Java课程成绩。

2. 类Student带参数的构造方法： 在构造方法中通过形参完成对成员变量的赋值操作。

3. 类Student的成员的get和set方法。

4. 根据类Student的定义，使用数组存储创建五个该类的对象，输出每个学生的信息，计算并输出这五个学生Java语言成绩的 平均值，以及计算并输出他们Java语言成绩的最大值和最小值。

   请上传源代码截图，截图需带类名和行号。类名用给定类名+学号命名，例如161007112王明，Student类名为 Student161007112.java，其余类名依此规则定义。并将运行结果截图上传，运行结果需要带输出窗口的运行时间。
   [最小截图工具.exe](https://api.dzzui.com/api/lanzoujx?url=https://mengchunm.lanzouw.com/i7mj203r320b&type=down)

   ```java
   
   public class test {
           private String id;//学号
           private String name;//姓名
           private String sex;//性别
           private int age;//年龄
           
   		//设置学生学号
   		 public void setsNO(String id) {
   		        this.id = id;
   		}
   		//获取学生学号
   		public String getsNO() {
   		        return id;
   		}
   		//设置姓名
   		public void setsName(String name){
   		        this.name = name;
   		}
   		//获取姓名
   		 public String getsName() {
   		          return name;
   		}
   		 //设置性别
   		public void setsSex(String sex) {
   		        this.sex = sex;
   		}
   		//获取性别
   		 public String getsSex() {
   		          return sex;
   		}
   		 //设置年龄  
   		 public void setsAge(int age) {
   		        this.age = age;
   		}
   		 //获取年龄
   		 public int getsAge() {
   		          return age;
   		}
   		//重写toString()
   		public String toString() {
           return "学号："+id+" 姓名："+name+" 性别："+sex+" 年龄："+age;
   }
           public static void main(String args[]) {
                    test s = new test();
                    s.setsNO("20072105");
                    s.setsName("摇摆震");
                    s.setsSex("男");
                    s.setsAge(20);
                    System.out.println(s);//打印内容为重写toString()后的内容 
           }     
   } 
   
   ```

   
---

类Count有方法int countNum(String str)，该方法的功能是统计已知字符串str中数字的个数。

例如，countNum("A42B83C2D")的返回值是5。

请上传源代码截图，截图需带类名和行号。类名用给定类名+学号命名，例如161007112王明，Count类名为 Count161007112.java，其余类名依此规则定义。并将运行结果截图上传，运行结果需要带输出窗口的运行时间。
[最小截图工具.exe](https://api.dzzui.com/api/lanzoujx?url=https://mengchunm.lanzouw.com/i7mj203r320b&type=down)

```java
public class Count {
	int countNum(String str)
	{
		int result=0;
		byte num[]=str.getBytes();
		for(int i=0;i<num.length;i++)
		{
			if(num[i]>='0'&&num[i]<='9')
			result++;
		}
		return result;
	}

	public static void main(String[] args) {
		String s="A42B83C2D";
		Count o=new Count();
		System.out.print(o.countNum(s)) ;
	}
}
```
---

编写个计算图形面积的程序，程序能够计算并输出圆的面积。设计个图形抽象类: Shape，Shape有两个抽象方法:计算面积getArea( ) 方法。显示图形的基本信息toString( )方法。和在此基础上派生出Circle类。

1. Circle类基本信息:圆心坐标、半径，園心坐标使用系统提供的Point2D类进行声明。

2. Circle有默认的构造方法及带参数的构造方法，默认是圆心在(0,0)点，半径为1.0的圆;成员变量为private属性，成员方法为public属性。

3. Circle类有属性的get和set方法.
   请上传源代码截至，截图需带美名和行号。类名用给定类名+学号命名，例如161007112王明，Shape类名为
   Shape161007112.java，其余类名依此规则定义。并将运行结果截图上传，运行结果需要带输出窗口的运行时间。
   [最小截图工具.exe](https://api.dzzui.com/api/lanzoujx?url=https://mengchunm.lanzouw.com/i7mj203r320b&type=down)



---

Points2D类表示平面坐标下点的坐标，必须满足如下要求：

1. 类Points2D的属性有：x,y 分别表示点的横纵坐标

2. 类Points2D 的方法有：

   属性x,y的get和set方法 Points2D( ) : 构造函数，将x和y坐标都置0

   copy Points2D( double x, double y) : 构造函数，设置x和y为给定坐标。

   copy double distance(Points2D a) : 计算当前点与给定点的距离。

   copy double distance(double x，double y)：计算当前点与给定x,y坐标点的距离。

   copy String ToString( ) : 输出当前点的坐标信息。

   请写出测试方法，分别计算给定两点的距离的两种情况，并输出，然后输出当前点的坐标信息。

   请上传源代码截图，截图需带类名和行号。类名用给定类名+学号命名，例如161007112王明，Points2D类名为 Points2D161007112.java，其余类名依此规则定义。并将运行结果截图上传，运行结果需要带输出窗口的运行时间。
   [最小截图工具.exe](https://api.dzzui.com/api/lanzoujx?url=https://mengchunm.lanzouw.com/i7mj203r320b&type=down)

---



设计一个名为Rectangle的矩形类，并实现Comparable接口，这个类包括:

1. 两个名为width和height的double数据域，它们分别表示矩形的宽和高；

2. Rectangle的无参构造方法，width和height的默认值都为1；

3. Rectangle的有参构造方法，用width和height为指定值构造一个矩形;

4. 一个名为getArea()的函数返回矩形的面积;

5. 一个名为getPerimeter()的函数返回矩形的周长；

6. compareTo（Rectangle a）方法用于比较和给定矩形的面积。
   编写一个测试程序，创建一个Rectangle对象，从键盘输入矩形的宽和高，然后输出矩形的面积和周长，再创建一个矩形对象，并比较两个矩形大小，输出结果。
   请上传源代码截图，截图需带类名和行号。类名用给定类名+学号命名，例如161007112王明，Rectangle类名为Rectangle161007112.java，其余类名依此规则定义。并将运行结果截图上传，运行结果需要带输出窗口的运行时间。
   [最小截图工具.exe](https://api.dzzui.com/api/lanzoujx?url=https://mengchunm.lanzouw.com/i7mj203r320b&type=down)