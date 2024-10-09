## Java考试题目汇总

### 选择题

设有定义：String s =“World”;，下列语句错误的是（ ）。

A char c = s.charAt(0); 

B int m = s.indexOf(‘r’);

C int n = s.length( ); 

**D** String str = s.append(‘2’);



在Java中，"456"属于（ ）类的对象。

A Integer **B** String C Number D int



下列对封装性的描述中，错误的是( )

A 封装体包含了属性和行为 

**B** 封装体中的属性和行为的访问权限是相同的 

C 被封装的某些信息在封装体外是不可见的 

D 封装使得抽象的数据类型提高了可重用性



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

A 行6 B 行1 C 行4 **D** 行9



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

**A** 2 2 3 

B 3 4 4 

C 2 3 3

D 2 2 2



在创建对象时必须（ ）

A 先声明对象，然后才能使用对象
B 先声明对象，为对象分配内存空间，然后才能使用对象
**C** 先声明对象，然后才能使用对象
D 先声明对象，为对象分配内存空间，对对象初始化，然后才能使用对象



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

**B** good and gbc 

C good and abc

D test ok and gbc



下面（ ）操作符的优先级最高？

**A** ( )
B ||
C &&
D !



下面的代码片段实现的是什么功能？( ) 

```java
File file = new File("C:\\test.dat");
if (file.exists()) {
	file.delete();
}
```

A 移动C:\test.dat
B 创建C:\test.dat
**C** 删除C:\test.dat
D 打开C:\test.dat文件输出流



设有定义 float x=3.5f, y=4.6f, z=5.7f；则以下的表达式中，值为true的是( )

**A** x != y
B x > y || x > z
C z > ( y + x )
D x < y & ! ( x < z )



Java源文件中最多只能有一个（）类，其他类的个数不限。

A interface
B abstract
C final
**D** public



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

**B** x是实例变量、y是类变量、s是局部变量 

C x和y是实例变量、s是参数 

D x、y和s都是成员变量



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

**A** 0

B 6 

C 1 

D 3



指出正确的表达式 （ ）

A double d = 0.9239d; 

**B** long l = 0xfffL;

C Boolean b = null; 

D byte a = 128;

>解析：
>
>A.没变量名
>
>B.没错，类型有、变量名有、赋值没错。
>
>C.boolean 类型只能赋值 true 或者false。而这里的Boolean应该是boolean类型的包装类，Boolean类型时可以被赋值为null的。所以此选项缺少变量名。
>
>D.byte赋值范围为-128~127；



关于被私有访问控制符private修饰的成员变量，以下说法正确的是（ ）

**A** 只能被该类自身所访问和修改 

B 可以被两种类访问和引用：该类本身、该类的所有子类 

C 只能被同一个包中的类访问 

D 可以被三种类所引用：该类自身、与它在同一个包中的其他类、在其他包中的该类的子类



类Test1定义如下：

```java
public class Test1{
	public float aMethod（float a，float b）{ }

}
```

A public int aMethod（int a， int b）{ } 

**B** public float aMethod（float c，float d）{ } 

C private float aMethod（int a，int b，int c）{ } 

D public float aMethod（float a， float b，float c）{ }



类Test1、Test2定义如下：

```java
public class Test1
{
	public float aMethod（float a，float b） throws IOException { }
}
	public class Test2 extends Test1{

}
```

将以下（ ）插入行6是不合法的。

A public int aMethod（int a，int b）throws Exception{ }
B public float aMethod（float p，float q）{ }
**C** float aMethod（float a，float b）{ }
D public int aMethod（int a，int b）throws IOException{ }



关于以下程序代码的说明正确的是（ ）

```java
1 class HasStatic{
2 	private static int x=100;
3 	public static void main(String args[ ]){
4 		HasStatic hs1= new HasStatic( );
5 		hs1.x++;
6 		HasStatic hs2=new HasStatic( );
7 		hs2.x++;
8 		hs1=new HasStatic( );
9	 	hs1.x++;
10	HasStatic.x- -;
11		System.out.println(“x=”+x);
12	}
13}
```

A 5行不能通过编译，因为引用了私有静态变量
B 10行不能通过编译，因为x是私有静态变量
**C** 程序通过编译，输出结果为：x=102
D 程序通过编译，输出结果为：x=103



执行语句int i = 1, j = ++i; 后i与j的值分别为（ ）。

A 2与1
**B** 2与2
C 1与1
D 1与2



在Java中，在包com.db下定义一个类，要让包com.util下的所有类都可以访问这个类，这个类必须定义为（ ）

**A** public
B default
C protected
D private



关键字supper的作用，叙述错误的是（ ）

**A** 用来调用父类中被重载的方法
B 用来调用父类的构造函数
C 用来调用父类的私有方法
D 用来访问父类被隐藏的成员变量



下列关于异常处理的描述中，错误的是( )

**A** 捕获到的异常只能在当前方法中处理，不能在其他方法中处理
B 使用throw语句抛出异常
C 使用try-catch-finally语句捕获异常
D 程序运行时异常由Java虚拟机自动进行处理



下列（ ）是合法的Java标识符？

A *theLastOne 

B Tree&Glasses 

C 273.5 

**D** FirstJavaApplet



下面声明数组的写法错误的是（ ）。

A int[ ] a;
B int[ ] a = {1，2，3};
**C** int[3][ ] a;
D int a[ ];



java语言中，负责并发管理的机制是（）

**A** 多线程
B 虚拟机
C 字节码
D 垃圾回收



执行完 int[ ] x=new int[10]；后，正确的是（ ）

A x[9]未定义
B x[0]为空
**C** x[9]为0
D x[10]为0



Java语言中，只限子类或者同一包中的类的方法能访问的访问权限是( )

A public
B 无修饰即缺省的访问控制修饰符
C private
**D** protected



()是构成Java程序的基本单位

A 对象 **B** 类 C main方法 D 方法



在Java中，下列（ ）语句不能通过编译。

A float f = 5 + 5.5;
B String s= “join”+ 3;
C String s= “join”+ “was”+ “here”;
**D** int a = 3 + 5;



下列（ ）类的声明是正确的？

A abstract final class HI{ }
**B** public abstract class Car{ }
C abstract private move(){ }
D protected private number;



下述概念中不属于面向对象方法的是（ ）。

A 继承、多态
B 类、封装
**C** 过程调用
D 对象、消息



以下关于构造函数的描述错误的是（ ）。

A 一般在创建新对象时，系统会自动调用构造函数。
**B** 构造函数的返回类型只能是void型。
C 构造函数的主要作用是完成对类的对象的初始化工作。
D 构造函数是类的一种特殊函数，它的方法名必须与类名相同。



A派生出子类B，B派生出子类C，并且在Java源代码中有如下声明：
A a0=new A();

A a1=new B();

A a2=new C();
问以下（ ）说法是正确的

A 第1、2、3行能通过编译，但第2、3行运行时出错
**B** 第1行、第2行和第3行的声明都是正确的
C 只有第1行能通过编译
D 第1、2行能通过编译，但第3行编译出错



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

k 的值是( )
**A** 2
B 31
C 3
D 33



Java语言的许多特点中，下列（）特点是C++语言所不具备的。

A 高性能
**B** 跨平台
C 有类库
D 面向对象



为AB类的一个无形式参数无返回值的方法method书写方法头，使得使用类名AB作为前缀就可以调用它，该方法头的形式为( )。

**A** static void method( )
B public void method( )
C final void method( )
D abstract void method( )