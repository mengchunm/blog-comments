---
title: java学习
cover: https://images.weserv.nl/?url=https://article.biliimg.com/bfs/article/58be6ff09e814f4d02ea6a631eeb7461a52426e1.jpg
---

记录下java作业
<!-- more --><!-- more -->

## 第五章

### 5.19 数字金字塔

```java
package chapter5;

public class Class2007210530 {
		public static void main(String[] args){
        int line=8;
        int temp=line;
        for(;line>=1;line--)
        {
        	for(int i=1;i<line;i++)
        		System.out.print("    ");
        	for(int i=0;i<=(temp-line);i++)
                System.out.printf("%4d",(int)Math.pow(2, i));
            for(int i=(temp-line);i>=1;i--)
                System.out.printf("%4d",(int)Math.pow(2, i-1));
        	System.out.print("\n");
        }
    }                                                  				
}
```

## 第六章

### 6.19 三角形面积

```java
package chapter6;
import java.util.Scanner;
public class MyTriangle2007210530 {
	public static void main(String[] args) {
    Scanner input = new Scanner(System.in);
    System.out.print("请输入三条边的值：");
    double side1=input.nextDouble(),side2=input.nextDouble(),side3=input.nextDouble();
    input.close();
    if (isValid(side1,side2,side3)){
        System.out.println("输入无效");
        System.exit(1);
    }
    System.out.println("这三角形的面积为："+area(side1, side2, side3));
}
public static boolean isValid(double side1, double side2, double side3){
    if (Math.abs(side1-side2)>side3||Math.abs(side3-side2)>side1||Math.abs(side3-side1)>side2)
    return(true);
    return(false);
}
public static double area(double side1,double side2,double side3){
    double p=(side1+side2+side3)/2;
    return Math.pow(p*(p-side1)*(p-side2)*(p-side3),0.5);
}
}
```



## 第九章

### 9.7 创建一个account类

```java
import java.util.Date;
public class Account2007210530{
	private int id=0;
	private double balance=0;
	private double annualInterestRate=0;
	private Date dateCreated;
	public Account2007210530(){
		dateCreated =new Date();
	}
	public Account2007210530(int id,double balance) {
		this.id=id;
		this.balance=balance;
		dateCreated = new Date();
	}
	public int getId() {
		return id;
	}
	public void setId(int id) {
		this.id = id;
	}
	public double getBalance() {
		return balance;
	}
	public void setBalance(double balance) {
		this.balance = balance;
	}
	public double getAnnualInterestRate() {
		return annualInterestRate;
	}
	public void setAnnualInterestRate(double annualInterestRate) {
		this.annualInterestRate = annualInterestRate;
	}
	public Date getDateCreated() {
		return dateCreated;
	}
	public double getMonthlyInterestRate() {
		return annualInterestRate/100/12;
	}
	public double getMonthlyInterest() {
		return balance*annualInterestRate/100/12;
	}
	public void withDraw(double money) {
		balance-=money;
	}
	public void deposit(double money) {
		balance+=money;
	}
	public static void main(String[] args) {
		Account2007210530 account = new Account2007210530(1122, 20000);
		account.setAnnualInterestRate(4.5);
		account.withDraw(2500);
		account.deposit(3000);
		System.out.println("余额: "+account.getBalance()+"\n"+"月利息: "+account.getMonthlyInterest()+"\n"+"开户日期: "+account.getDateCreated());
	}
}
```
## 第十一章

### 11.2 Person类

```java
package chapter11;
import java.util.Date;

class Person{
    private String name;
    private String address;
    private String phoneNumber;
    private String email;
    Person(String name,String address,String phoneNumber,String email){
        this.name = name;
        this.address = address;
        this.phoneNumber = phoneNumber;
        this.email = email;
    }
    public String getThisName(){
        return this.name;
    }
    public String toString(){
        return ("Person " + this.name);
    }
}
class Student extends Person{
    private String grade;
    Student(String name,String address,String phoneNumber,String email,String grade){
        super(name,address,phoneNumber,email);
        this.grade = grade;
    }
    public String toString(){
        return ("Student " + this.getThisName());
    }
}
class Employee extends Person{
    private String office;
    private double salary;
    private Date acceptDate;

    Employee(String name,String address,String phoneNumber,String email,String office,double salary,Date acceptDate){
        super(name,address,phoneNumber,email);
        this.office = office;
        this.salary = salary;
        this.acceptDate = acceptDate;
    }
    public String toString(){
        return ("Employee " + this.getThisName());
    }
}
class Faculty extends Employee{
    private Date workDate;
    private int level;
    Faculty(String name,String address,String phoneNumber,String email,String office,double salary,Date acceptDate,Date workDate,int level){
        super(name,address,phoneNumber,email,office,salary,acceptDate);
        this.level = level;
        this.workDate = workDate;
    }
    public String toString(){
        return ("Faculty " + this.getThisName());
    }
}
class Staff extends Employee{
    private String title;
    Staff(String name,String address,String phoneNumber,String email,String office,double salary,Date acceptDate,String title){
        super(name,address,phoneNumber,email,office,salary,acceptDate);
        this.title = title;
    }
    public String toString(){
        return ("Staff " + this.getThisName());
    }
}
public class Account2007210530 {
    public static void main(String[] args) {
        Person person = new Person("人名","地址","电话","邮箱");
        System.out.println(person.toString());
        Student student = new Student("学生人名","学生地址","学生电话","学生邮箱","班级状态");
        System.out.println(student.toString());
        Employee employee = new Employee("雇员人名","雇员地址","雇员电话","雇员邮箱","雇员办公室",1,new Date());
        System.out.println(employee.toString());
        Faculty faculty = new Faculty("教员人名","教员地址","教员电话","教员邮箱","教员办公室",1,new Date(),new Date(),1);
        System.out.println(faculty.toString());
        Staff staff = new Staff("职员人名","职员地址杏园","职员电话","职员邮箱","职员办公室",1,new Date(),"头衔");
        System.out.println(staff.toString());
    }
}
```