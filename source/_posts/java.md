---
title: java学习
cover: https://s3.amazonaws.com/com.twilio.prod.twilio-docs/original_images/java-logo-wide.jpg
---
```

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

