### 可变参数
JDK 1.5 开始，Java支持传递同类型的可变参数给一个方法。

方法的可变参数的声明如下所示：

typeName... parameterName
在方法声明中，在指定参数类型后加一个省略号(...) 。

一个方法中只能指定一个可变参数，它必须是方法的最后一个参数。任何普通的参数必须在它之前声明。

实例
VarargsDemo.java 文件代码：

```java
public class test {
    public static void main(String[] args) {
        printMax(34, 3, 3, 2, 56);
        printMax(new int[]{1, 2, 3});
    }
 
    public static void printMax(int...a) {
        int result = a[0];
        for (int i = 1; i<a.length; i++){
            if (a[i] >  result) {
                result = a[i];
            }
        }
        System.out.println("The max value is " + result);
    }
}
```
以上实例编译运行结果如下：

The max value is 56
The max value is 3