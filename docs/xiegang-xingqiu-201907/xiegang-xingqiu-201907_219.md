# 本周分享的第一个开

# 本周分享的第一个开

小猿 : 本周分享的第一个开源项目：Android 高仿微信 App 本 项目仿最新版微信 6.5.7（除图片选择器外），基于融云 SDK，使用目前较火的 Rxjava+Retrofit+MVP+Glide 技术开 发。微信的基本功能差不多都模仿出来了，有兴趣的欢迎学 习 ~ github 项目地址： 下面截几张项目图片供大家观看！ 2018-04-09

评论区： 远哥 : 牛逼

小猿 : 欢迎大家把平时收藏压箱底的项目分享出来哈[色][色][色]

![image](img/Image_159.png)

![image](img/Image_160.png)

![image](img/Image_161.png)

![image](img/Image_162.png)

![image](img/Image_163.png)

关注公众号"懒人找资源"，星球资源一站式服务

### Android 面试

小猿 : Android 面试题 1、Android 的四大组件以及作用 Activity：Activity 是 Android 程序与 用户交互的窗口，是 Android 构造块中最基本的一种，它需要为保持各界面的状态，做 很多持久化的事情，妥善管理生命周期以及一些跳转逻辑。 service：后台服务于 Activity，封装有一个完整的功能逻辑实现，接受上层指令，完成相关的动作，定义好 需要接受的 Intent 提供同步和异步的接口。 Content Provider：是 Android 提供的第三方应 用数据的访问方案，对外提供数据，屏蔽内部数据的存储细节，向外提供统一的借口 模型，大大简化上层应用对数据的整合提供了更方便的途径。 BroadCast Receiver：接 受一种或者多种 Intent 作触发事件，接受相关消息，做一些简单处理，转换成一条 Notification，统一了 Android 的事件广播模型。 2、描述下 Activity 的生命周期？ Activity 的生命周期方法有：onCreate()、onStart()、onReStart()、onResume()、onPause()、 onStop()、onDestory()； 可见生命周期：从 onStart()直到系统调用 onStop() 前台生命周 期：从 onResume()直到系统调用 onPause() 屏幕旋转时的 Activity 生命周期: 不设置 Activity 的 android:configChanges 时，切屏会重新调用各个生命周期，切横屏时会执行一次，切 竖屏时会执行两次； 设置 Activity 的 android:configChanges="orientation"时，切屏还是会 重新调用各个生命周期，切横、竖屏时只会执行一次； 设置 Activity 的 android:configChanges="orientation|keyboardHidden"时，切屏不会重新调用各个生命周 期，只会执行 onConfigurationChanged 方法。 3、请介绍下 ContentProvider 是如何实现数 据共享的 一个程序可以通过实现一个 Content provider 的抽象接口将自己的数据完全暴 露出去，而且 Content providers 是以类似数据库中表的方式将数据暴露。

Content providers 存储和检索数据，通过它可以让所有的应用程序访问到，这也是应用 程序之间唯一共享数据的方法。 要想使应用程序的数据公开化，可通过 2 种方法：创建 一个属于你自己的 Content provider 或者将你的数据添加到一个已经存在的

Content provider 中，前提是有相同数据类型并且有写入 Content provider 的权限。 如何通 过一套标准及统一的接口获取其他应用程序暴露的数据？ Android 提供了 ContentResolver，外界的程序可以通过 ContentResolver 接口访问 ContentProvider 提供的数 据。 4、解释下 Handler 的运行机制？ Message，理解为线程间交流的信息 Handler，是 Message 的主要处理者，负责 Message 的发送和执行处理 Message Queue，用来存放通过 Handler 发布的消息，按照先进先出执行 Looper ，是每条线程里的 Message Queue 的管家 Handler 一般在主线程中创建，子线程通过处理器对象的 sendMessage 发消息到 MessageQueue(消息队列)里，主线程中已经包含了一个 Looper(轮循器)，Looper 是死循 环的，会一直轮询消息队列，看是否有 Message(消息) ，如果有，轮询器会把消息对象 传给 Handler(消息处理器)，然后调用 handlerMessage 处理该消息，进而更新 UI。 5、什 么是 ANR？如何避免 ANR 异常？ ANR：Application Not Responding。在 Android 中，活 动管理器和窗口管理器这两个系统服务负责监视应用程序的响应，当用户操作的在 5s 内 应用程序没能做出反应，BroadcastReceiver 在 10 秒内没有执行完毕，就会出现应用程序 无响应对话框，就是 ANR。 避免方法：Activity 应该在它的关键生命周期方法（如 onCreate()和 onResume()）里尽可能少的去做创建操作。潜在的耗时操作，例如网络或 数据库操作，或者高耗时的计算如改变位图尺寸，应该在子线程里（或者异步方式） 来完成。主线程应该为子线程提供一个 Handler，以便完成时能够提交给主线程。 6、 Android 中三种动画,特点和区别是什么？ Android 中的动画有帧动画，补间动画，属性 动画。 帧动画：一张张图片不断的切换，形成动画效果，类似小时候的电影。很多应 用的 loading 是采用这种方式。 补间动画：是对某个 View 进行一系列的动画的操作，包

括淡入淡出(Alpha)，缩放(Scale)，平移(Translate)，旋转(Rotate)四种模式。 属性动画： 属性动画不再仅仅是一种视觉效果了，而是一种不断地对值进行操作的机制，并将值 赋到指定对象的指定属性上，可以是任意对象的任意属性。 7、注册广播有几种方式， 有何优缺点？ 第一种:在清单文件中声明,添加 第二种使用代码进行注册： IntentFilter filter = new IntentFilter("android.provider.Telephony.SMS_RECEIVED"); IncomingSMSReceiver receiver = new IncomgSMSReceiver(); registerReceiver(receiver.filter); 两种注册类型的区别是： 1)第一种不是常驻型广播，也就是说广播跟随程序的生命周 期。 2)第二种是常驻型，也就是说当应用程序关闭后，如果有信息广播来，程序也会 被系统调用自动运行。 8、Service 的生命周期 1.Service 常用生命周期回调方法如下： onCreate() 该方法在服务被创建时调用，该方法只会被调用一次，无论调用多少次 startService()或 bindService()方法， 服务也只被创建一次。 onDestroy()该方法在服务被终 止时调用。 2\. Context.startService()启动 Service 有关的生命周期方法 onStart() 只有采用 Context.startService()方法启动服务时才会回调该方法。该方法在服务开始运行时被调 用。 多次调用 startService()方法尽管不会多次创建服务，但 onStart()方法会被多次调 用。 3\. Context.bindService()启动 Service 有关的生命周期方法 onBind()只有采用 Context.bindService()方法启动服务时才会回调该方法。该方法在调用者与服务绑定时被 调用， 当调用者与服务已经绑定，多次调用 Context.bindService()方法并不会导致该方法 被多次调用。 onUnbind()只有采用 Context.bindService()方法启动服务时才会回调该方 法。该方法在调用者与服务解除绑定时被调用。 备注： 1\. 采用 startService()启动服务

Intent intent =new Intent(DemoActivity.this, DemoService.class); startService(intent); 2.Context.bindService()启动 Intent intent =new Intent(DemoActivity.this, DemoService.class); bindService(intent, conn, Context.BIND_AUTO_CREATE);

//unbindService(conn);//解除绑定 9、 请介绍下 Android 的数据存储方式。 一.SharedPreferences 方式 二.文件存储方式 三.SQLite 数据库方式 四.内容提供器

（Content provider）方式 五. 网络存储方式 10、AIDL 的全称是什么？如何工作？能处 理哪些类型的数据？ AIDL 的英文全称是 Android Interface Define Language 当 A 进程要去 调用 B 进程中的 service 时，并实现通信，我们通常都是通过 AIDL 来操作的 A 工程： 首先 我们在 net.blogjava.mobile.aidlservice 包中创建一个 RemoteService.aidl 文件，在里面我们自 定义一个接口，含有方法 get。ADT 插件会在 gen 目录下自动生成一个 RemoteService.java 文件，该类中含有一个名为 RemoteService.stub 的内部类，该内部类中含有 aidl 文件接口 的 get 方法。 说明一：aidl 文件的位置不固定，可以任意 然后定义自己的 MyService 类， 在 MyService 类中自定义一个内部类去继承 RemoteService.stub 这个内部类，实现 get 方 法。在 onBind 方法中返回这个内部类的对象，系统会自动将这个对象封装成 IBinder 对 象，传递给他的调用者。 其次需要在 AndroidManifest.xml 文件中配置 MyService 类，代 码如下： 为什么要指定调用 AIDL 服务的 ID,就是要告诉外界 MyService 这个类能够被别的进程访问，只要别的进程知道这个 ID，正是有了这个 ID,B 工程才能 找到 A 工程实现通信。 说明：AIDL 并不需要权限 B 工程： 首先我们要将 A 工程中生 成的 RemoteService.java 文件拷贝到 B 工程中，在 bindService 方法中绑定 aidl 服务 绑定 AIDL 服务就是将 RemoteService 的 ID 作为 intent 的 action 参数。 说明：如果我们单独将 RemoteService.aidl 文件放在一个包里，那个在我们将 gen 目录下的该包拷贝到 B 工程中。 如果我们将 RemoteService.aidl 文件和我们的其他类存放在一起，那么我们在 B 工程中就 要建立相应的包，以保证 RmoteService.java 文件的报名正确，我们不能修改 RemoteService.java 文件

bindService(newInten("net.blogjava.mobile.aidlservice.RemoteService"),serviceConnection, Context.BIND_AUTO_CREATE); ServiceConnection 的

onServiceConnected(ComponentName name, IBinderservice)方法中的 service 参数就是 A 工程 中 MyService 类中继承了 RemoteService.stub 类的内部类的对象。 大家有关于 Android 面试 更全的面试题，欢迎发帖补充，谢谢！

2018-04-04

关注公众号"懒人找资源"，星球资源一站式服务