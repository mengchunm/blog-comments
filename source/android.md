## 一. 程序阅读题（共9 题，40.0分）

1. (程序阅读题,4.4分)在activity_main.xml文件中，放置了一个Button（其中部分属性设置为android:id="@+id/button"）控件用于表示一个按钮。调用按钮的setOnClickListener（）方法，在该方法中通过匿名内部类来实现OnClickListener接口，请补充下面缺失的代码。（注意方法名大小写）
   
   ```
   public class MainActivity extends AppCompatActivity {
   
       private Button button;
   
       @Override
   
       protected void onCreate(Bundle savedInstanceState) {
   
       super.onCreate(savedInstanceState);
   
       setContentView(R.layout.activity_main);       //设置Activity对应的布局文件
   
       button = (Button) _______1________(R.id.button); //获取界面上的按钮控件
   
       //通过匿名内部类来实现OnClickListener接口
   
       button.setOnClickListener(new View.OnClickListener() {
   
           @Override
          
           public void _______2_____(View view) {
          
               Toast.makeText(MainActivity.this, "您点击了按钮",Toast.LENGTH_SHORT).show();
          
           }
   
       });
   
       }
   
   }
   
   
   ```
   
   
   

正确答案：
(1) findViewById
(2) onClick

2. (程序阅读题,4.4分)在activity_main.xml文件中，放置了一个Button（其中部分属性设置为android:id="@+id/button"）控件用于表示一个按钮。MainActivity实现了OnLongClickListener 接口，实现了长按按钮弹出Toast的代码。请阅读代码补充下面缺失的代码。（注意方法名大小写）
   
   ```
   2. public class MainActivity extends AppCompatActivity _______1________View.OnLongClickListener {
   
       private Button button;
   
       @Override
   
       protected void onCreate(Bundle savedInstanceState) {
   
           super.onCreate(savedInstanceState);
          
           setContentView(R.layout.activity_main);       //设置Activity对应的布局文件
          
           button = (Button) findViewById(R.id.button); //获取界面上的按钮控件
          
           button.___________2____________(this);          //注册监听
   
       }
   
       @Override
   
       public boolean ______3__________(View v) {  //实现OnLongClickListener接口中的方法
   
           if (v == button) {                   //判断长时间按下的控件是否是button
          
               Toast.makeText(MainActivity.this, "您长时间按下了按钮",Toast.LENGTH_SHORT).show();
          
           }
          
           return false;
   
       }
   
   }
   ```
   
   


正确答案：
(1) implements  
(2) setOnLongClickListener
(3) onLongClick

3. (程序阅读题,4.4分)以下代码通过startService（）方法开启服务，请阅读代码并补充确实的代码。
   
   ```
   public class MainActivity extends AppCompatActivity {
   
       @Override
   
       protected void onCreate(Bundle savedInstanceState) {
   
           super.onCreate(savedInstanceState);
          
           setContentView(R.layout.activity_main);
          
           init();
   
       }
   
       private void init(){
   
           Button btn_start = (Button) findViewById(R.id.btn_start);
          
           Button btn_stop = (Button) findViewById(R.id.btn_stop);
          
           btn_start.setOnClickListener(new View.OnClickListener() {
          
               @Override
          
               public void ______1_____(View view) {
          
                   //开启服务
          
                   ___________   intent = new _________(MainActivity.this, MyService.class);
          
                   startService(intent);
          
               }
          
           });
          
           btn_stop.setOnClickListener(new View.OnClickListener() {
          
               @Override
          
               public void onClick(View view) {
          
                   //关闭服务
          
                   Intent intent = new Intent(MainActivity.this, MyService.class);
          
                   __________(intent);
          
               }
          
           });
   
       }
   
   }
   ```
   
   
   


正确答案：
(1) onClick
(2) Intent
(3) stopService

4. (程序阅读题,4.4分)在MainActivity 中创建了一个init()方法，在该方法中获取发送求救广播的控件并实现该控件的点击事件。请补充缺失的代码。（注意方法名的大小写）
   
   ```
    public class MainActivity extends AppCompatActivity {
   
       private MyBroadcastReceiver receiver;
   
       @Override
   
       protected void onCreate(Bundle savedInstanceState) {
   
           super.onCreate(savedInstanceState);
          
           setContentView(R.layout.activity_main);
          
           init();
   
       }
   
       private void init(){
   
           receiver = new MyBroadcastReceiver(); //实例化广播接收者
          
           String action = "Help_Stitch";
          
           IntentFilter intentFilter = new IntentFilter(action);
          
           _________________(receiver,intentFilter); //注册广播
          
           Button btn_help= (Button) findViewById(R.id.btn_help);
          
           btn_help.setOnClickListener(new View.OnClickListener() {
          
               @Override
          
               public void onClick(View view) {
          
                   Intent intent = new Intent();
          
                   //定义广播的事件类型
          
                   intent.setAction("Help_Stitch");
          
                   sendBroadcast(intent);//发送广播
          
               }
          
           });
   
       }
   
       @Override
   
       protected void onDestroy() {
   
           super.onDestroy();
          
           unregisterReceiver(receiver);
   
       }
   
   }
   ```
   
   
   


正确答案：
(1) registerReceiver

5. (程序阅读题,4.4分)MyBroadcastReceiver 类继承了BroadcastReceiver ，用于接收发送的广播信息，请补充下面的代码（注意方法名的大小写）
   
   ```
   public class MyBroadcastReceiver extends BroadcastReceiver {
       @Override
   
       public void ____________(Context context, Intent intent) {
   
           Log.i("MyBroadcastReceiver", "自定义的广播接收者,接收到了求救广播事件");
          
           Log.i("MyBroadcastReceiver",intent.getAction());
          
                }
          
                }
   
   ```
   
   
   正确答案：
   (1) onReceive

6. (程序阅读题,4.4分)下面代码创建了一个名为MyService 服务，并重写了服务的声明周期，请补全下面缺失的代码。（注意大小写）
   public class MyService extends ____________{

    

   ```
   @Override
   
       public void onCreate() {
   
           super.onCreate();
          
           Log.i("MyService", "创建服务，执行onCreate()方法");
   
       }
   
       @Override
   
       public int onStartCommand(Intent intent, int flags, int startId) {
   
           Log.i("MyService", "开启服务，执行onStartCommand()方法");
          
           return super.onStartCommand(intent, flags, startId);
   
       }
   
       @Override
   
       public IBinder onBind(Intent intent) {
   
           return null;
   
       }
   
       @Override
   
       public void onDestroy() {
   
           super.onDestroy();
          
           Log.i("MyService", "关闭服务，执行onDestroy()方法");
   
       }
   
   }
   ```
   
   
   
   
   


正确答案：
(1) Service 

7. (程序阅读题,4.4分)创建内容观察者代码如下，创建了一个MyObserver  的类，继承了内容观察者，在该类中重写了父类的构造方法。请补全下面的代码（注意大小写）
```
   public class MyObserver extends ______________{

        public MyObserver(Handler handler) {//handler 是一个消息处理器。
       
            super(handler);
       
        }
       
        @Override
       
        //当info表中的数据发生变化时则执行该方法
       
        public void onChange(boolean selfChange) {
       
            Log.i("监测数据变化", "有人动了你的数据库！");
       
            super.onChange(selfChange);
       
        }

    }
```

正确答案：
(1) ContentObserver 

8. (程序阅读题,4.4分)
   注册内容观察者的代码如下，请补充缺失的代码（注意大小写）

    

   ```
     ContentResolver resolver=getContentResolver();//获取ContentResolver 对象
   
          Uri uri = Uri.parse("content://cn.itcast.contentobserverdb/info");
   
   
           
   
           //参数true定义了监测的范围，最后一个参数是一个内容观察者对象
          
           //注册内容观察者，参数uri指向要监测的数据库info表，
          
           resolver.________________(uri, true,new MyObserver(new Handler()));
   
   
   ```
   
   
   正确答案：
   (1) registerContentObserver

9. (程序阅读题,4.8分)
    创建SQLite数据库的代码如下，请补充缺失的代码（注意大小写）

  ```
  class MyHelper extends ____1______{
       //构造方法
       public _____2__(Context context) {
           super(context, "itcast.db", null, 1);
       }
       @Override
       //数据库第一次被创建时调用的方法
       public void onCreate(SQLiteDatabase db) {
           db._____3___("CREATE TABLE information(_id INTEGER PRIMARY KEY AUTOINCREMENT, name VARCHAR(20),  phone VARCHAR(20))");
       }
       @Override
       public void onUpgrade(SQLiteDatabase db, int oldVersion, int newVersion) {
       }
   }
  
  ```

  正确答案：

(1)SQLiteOpenHelper

(2) MyHelper

(3)execSQL

## 二. 单选题（共6 题，20.0分）

1. (单选题,3.3分)Android项目中的主题和样式资源，通常放在（）目录
     A. res/drawable
       B. res/layout
       C. res/values
       D. assets
       我的答案:C 正确答案: C

2. (单选题,3.3分)关于Logcat，下列说法错误的是（   ）

     A.主要用于Android程序调试时输出信息

      B. 可以通过Log.v(),Log.d(),Log.w(),Log.i(),Log.e()输出不同级别的日志
      C. 可以通过设置日志输出的tag值来过滤掉不需要的日志信息
      D. 与System.out.println()控制台输出相比，使用较为复杂，因此不推荐
       我的答案:D 正确答案: D

3. (单选题,3.3分)想从ActivityA跳转到ActivityB，下面正确的显式Intent的构造方法是（   ）
      A. Intent intent = new Intent(ActivityA.class, ActivityB.this); 
       B. Intent intent = new Intent(ActivityA.this, ActivityB.class); 
       C. Intent intent = new Intent(ActivityB.class, ActivityA.this); 
       D. Intent intent = new Intent(ActivityB.this, ActivityA.class); 
       我的答案:B 正确答案: B

4. (单选题,3.3分)Android项目中存放程序代码的位置是（    ）
       A. res
       B. gen
       C. src
       D. bin 
       我的答案:C 正确答案: C

5. (单选题,3.3分)
     下面关于RadioButton控件的描述，正确的是（）。

       A. RadioButton默认为选中状态
       B. RadioButton表示单选按钮
       C. RadioButton表示文本控件
       D. 以上说法都不对
       我的答案:B 正确答案: B

6. (单选题,3.5分)
     下列选项中，属于为ListView添加适配器的方法的是（）。

      A. setAdapter()
       B. setBaseAdapter()
       C. addAdapter()
       D. addBaseAdapter()
       我的答案:A 正确答案: A
     
## 三. 填空题（共6 题，10.0分）

1. (填空题,1.6分)
请根据下面显示效果，补全布局文件的代码。



```
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"

    android:orientation="vertical"
    
    android:layout_width="match_parent"
    
    android:layout_height="match_parent"
    
    android:gravity="______①______">

<______②________

    android:layout_width="match_parent"
    
    android:layout_height="wrap_content"
    
    android:text="@string/question_river"
    
    android:textSize="24sp"
    
    android:gravity="center"
    
    android:id="@+id/textview_question">

</______②________>

    <LinearLayout
    
        android:layout_width="match_parent"
    
        android:layout_height="wrap_content"
    
        android:orientation="horizontal"
    
        android:______③________="center">
    
        <______④_____
    
            android:id="@+id/button_pre"
    
            android:layout_width="wrap_content"
    
            android:layout_height="wrap_content"
    
            android:text="上一个"></______④_____>
    
        <______④_____
    
            android:id="@+id/button_next"
    
            android:layout_width="wrap_content"
    
            android:layout_height="wrap_content"
    
            android:text="下一个"></______④_____>
    
    </LinearLayout>
    
    <LinearLayout
    
        android:layout_width="match_parent"
    
        android:layout_height="wrap_content"
    
        android:orientation="horizontal"
    
        android:______③________="center">
    
        <______④_____
    
            android:id="@+id/button_correct"
    
            android:layout_width="wrap_content"
    
            android:layout_height="wrap_content"
    
            android:text="正确"></______④_____>
    
        <______④_____
    
            android:id="@+id/button_wrong"
    
            android:layout_width="wrap_content"
    
            android:layout_height="wrap_content"
    
            android:text="错误"></______④_____>
    
    </LinearLayout>

<______④_____

    android:layout_width="wrap_content"
    
    android:layout_height="wrap_content"
    
    android:text="______⑤_____"
    
    android:id="@+id/button_jump_cheat">

</______④_____>

</LinearLayout>
```



我的答案：
(1) center
(2) TextView
(3) gravity
(4) Button
(5) 偷看一眼答案
正确答案：
(1) center
(2) TextView
(3)gravity
(4) Button
(5) 偷看一眼答案

2. (填空题,1.6分)
每个Activity都要经历从创建到销毁的整个过程，请根据下述情景填入其所经历的生命周期方法。

运行某个App，该App的主Activity会依次运行 onCreate( )→________①________→________②__________;

单击Home按钮，该主Activity会依次运行 onPause( )→________③________;

单击最近使用键，再选择该应用重新运行，则该主Activity会依次运行_______④_______→_______⑤_______→onResume( )



我的答案：
(1) onStar()
(2) onResume()
(3) onStop()
(4) onRcstart()
(5) onStart()
正确答案：

(1)onStart( )；onStart

(2)onResume( )； onResume

(3)onStop( )；onStop

(4) onRestart( )；onRestart

(5) onStart( )；onStart

3. (填空题,1.6分)
请根据下面显示效果，补全布局文件的代码。

```
<?xml version="1.0" encoding="utf-8"?>

<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"

    android:layout_width="match_parent"
    
    android:layout_height="match_parent"
    
    android:background="#E6E6E6"
    
    android:orientation="______①______"
    
    android:padding="10dp">
    
    <ImageView
    
        android:layout_width="70dp"
    
        android:layout_height="70dp"
    
        android:layout_centerHorizontal="true"
    
        android:layout_gravity="center_horizontal"
    
        android:layout_marginTop="30dp"
    
        android:src="@drawable/head" />
    
    <LinearLayout
    
        android:layout_width="match_parent"
    
        android:layout_height="wrap_content"
    
        android:layout_marginTop="15dp"
    
        android:background="@android:color/white"
    
        android:orientation="horizontal">
    
        <_______②________
    
            android:layout_width="wrap_content"
    
            android:layout_height="wrap_content"
    
            android:padding="10dp"
    
            android:text="账号:"
    
            android:textColor="#000"
    
            android:textSize="20sp" />
    
        <_____③_______
    
            android:id="@+id/et_account"
    
            android:layout_width="match_parent"
    
            android:layout_height="wrap_content"
    
            android:layout_marginLeft="5dp"
    
            android:background="@null"
    
            android:padding="10dp" />
    
    </LinearLayout>
    
    <_____④___
    
        android:layout_width="match_parent"
    
        android:layout_height="wrap_content"
    
        android:layout_marginTop="10dp"
    
        android:background="@android:color/white"
    
        android:orientation="horizontal">
    
        <TextView
    
            android:id="@+id/tv_password"
    
            android:layout_width="wrap_content"
    
            android:layout_height="wrap_content"
    
            android:padding="10dp"
    
            android:text="密码:"
    
            android:textColor="#000"
    
            android:textSize="20sp" />
    
        <EditText
    
            android:id="@+id/et_password"
    
            android:layout_width="match_parent"
    
            android:layout_height="wrap_content"
    
            android:layout_marginLeft="5dp"
    
            android:background="@null"
    
            android:inputType="textPassword"
    
            android:padding="10dp" />
    
    </LinearLayout>
    
    <_____⑤_____
    
        android:id="@+id/btn_login"
    
        android:layout_width="match_parent"
    
        android:layout_height="wrap_content"
    
        android:layout_marginTop="25dp"
    
        android:background="#3C8DC4"
    
        android:text="登录"
    
        android:textColor="@android:color/white"
    
        android:textSize="20sp" />

</LinearLayout>
```



我的答案：
(1) vertical
(2) TextView
(3) EditText
(4) LinearLayout
(5) Button
正确答案：
(1) vertical
(2) TextView
(3) EditText
(4) LinearLayout
(5) Button
4. (填空题,1.6分)
在Android中，AlertDialog对话框用来提示一些重要信息或者显示一些需要用户交互的内容，请根据描述补全

代码



```
public class MainActivity extends AppCompatActivity {

    @Override
    
    protected void onCreate(Bundle savedInstanceState) {
    
        super.onCreate(savedInstanceState);
    
        setContentView(R.layout.activity_main);
    
    }
    
    @Override
    
    public void onBackPressed() {
    
        //声明对象
    
        AlertDialog dialog;
    
        AlertDialog.Builder builder =_______①___________ AlertDialog.Builder(this)
    
                .______②_______("普通对话框")                      //设置对话框的标题
    
                .setIcon(R.mipmap.ic_launcher)           //设置设置标题图标
    
                .setMessage("是否确定退出应用？")           //设置对话框的提示信息
    
                //添加“确定”按钮
    
                .________③__________("确定", new DialogInterface.OnClickListener() {
    
                    @Override
    
                    public void onClick(DialogInterface dialog, int which) {
    
                        dialog.dismiss();                   //关闭对话框
    
                        MainActivity.this.finish();       //关闭MainActivity
    
                    }
    
                })
    
                //添加“取消”按钮
    
                .setNegativeButton("取消", new DialogInterface.OnClickListener() {
    
                    @Override
    
                    public void onClick(DialogInterface dialog, int which) {
    
                        dialog.______④______();
    
                    }
    
                });
    
        dialog =  builder.create();
    
        dialog.________⑤_________();
    
    }

}
```



我的答案：
(1) new
(2) setTitle
(3) setPositiveButton
(4) dismiss
(5) show
正确答案：
(1) new
(2) setTitle
(3) setPositiveButton
(4) dismiss
(5) show
5. (填空题,1.6分)
    Dalvik中的Dx工具会把部分class文件转换成（）文件
    我的答案：
    (1) dex
    正确答案：
    (1) dex

6. (填空题,2.0分)发送隐式Intent后，Android 系统会使用（）匹配相应的组件
    我的答案：
    (1) IntentFilter
    正确答案：
    (1) InterFilter
    四. 判断题（共5 题，25.0分）

7. (判断题,5.0分)
    android:textSize属性可以设置TextView中的文本显示的大小。

    A. 对
    B. 错
      我的答案: 对 正确答案: 对

2. (判断题,5.0分)Toast是Android系统提供的轻量级信息提醒机制，用于向用户提示即时消息。
    A. 对
    B. 错
    我的答案: 对 正确答案: 对

3. (判断题,5.0分)Button控件可以显示文本信息，也可以显示图片资源。
    A. 对
    B. 错
    我的答案: 对 正确答案: 对

4. (判断题,5.0分)
    TextView控件用于显示文本信息。

    A. 对
    B. 错
      我的答案: 对 正确答案: 对

5. (判断题,5.0分)
    当Toast提示Wifi连接时，会打断用户点击按钮的操作。
    
    A. 对
    B. 错
     我的答案: 错 正确答案: 错
