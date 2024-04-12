# 抽空整理了一下 An

# 抽空整理了一下 An

小猿 : 抽空整理了一下 Android 学习路线，如何从技术小白到 Android 工程师，这边有个比较详细的学习路线，推荐给大 家，希望对你有帮助！喜欢的不要忘记点个赞哈！ 第一周

【UI 基础】 第 1 天： Android 环境搭建及工程目录介绍 1.1 Android 开发(版本：SDK21 及以上版本)环境搭建 1.2 Android

发展史、移动设备操作系统、四层系统架构等理论知识 1.2.1

Android 发展史介绍 1.2.2 移动设备操作系统介绍 1.2.3 Android

四层系统架构的介绍 1.3 HelloWorld 程序 1.3.1 编写 HelloWorld 程序 1.3.2 APP 的目录结构介绍 1.4 adb shell 简介 第 2 天： 常用 UI 布局与控件 2.1 View 与 ViewGroup 2.1.1 View 的概念 2.1.2

ViewGroup 的概念 2.1.3 View 的树形结构 2.2 LinearLayout【重

点讲解】 2.2.1 View 常用属性 2.2.2 Android 中长度单位的概

念、区别及转换公式（sp、dp、dip、px、dpi) 2.2.3

LinearLayout 特有属性 2.3 RelativeLayout 2.4 FrameLayout 2.5

GridLayout 2.5.1 GridLayout 特有属性 2.6 TextView 2.6.1 TextView 属性 第 3 天： 表单 UI 控件及控件的事件处理 3.1 EditText、Button、ImageView 3.1.1 EditText 常用属性介绍 android:inputType android:hint android:imeOptions 3.1.2 Button 常 用属性介绍及监听器使用 android:onClick Button 绑定监听器方 式 3.1.3 ImageView 常用属性介绍 3.2 RadioButton 及 RadioGroup

的用法 3.2.1 RadioButton、RadioGroup 的常用属性 3.2.2 绑定

RadioGroup 特有监听器 3.3 CheckBox 的多选效果及监听 3.3.1

CheckBox 的常用属性 3.3.2 绑定 CheckBox 特有监听器 3.4 Toast 的基本用法 第 4 天： Spinner、AutoCompleteTextView、 ScrollView 及适配器、数组资源 4.1 Spinner 4.1.1 Spinner 的常

用属性 android:entries="" 4.1.2 Spinner 的常用方法 4.2 适配器

4.2.1 适配器的介绍 4.2.2 ArrayAdapter 的介绍及使用 4.3 数组

资源 4.3.1 定义数组资源 4.3.2 获取数组资源 4.4

AutoCompleteTextView 4.4.1 AutoCompleteTextView 的常用属

性 4.4.2 AutoCompleteTextView 的常用方法 4.5 ScrollView 4.5.1

垂直 ScrollView 的使用 4.5.2 HorizontalScrollView 的使用 4.6

ProgressBar、SeekBar、RatingBar 4.6.1 ProgressBar 的基本用法

4.6.2 SeekBar 的基本用法及美化 4.6.3 RatingBar 的基本用法及 美化 第 5 天： UI 美化及 Android 资源 5.1 Style 的简单用法 5.1.1 style 的基本使用 5.1.2 style 的继承 5.1.3 利用 selector 及 shape 修 改多选框的显示效果 5.1.4 利用 selector 实现选中与否、改变默 认 RadioButton 的显示效果 5.2 Android 资源汇总 5.2.1 id、字符 串资源、颜色资源、尺寸资源、布局资源、字符数组资源、 样式和主题资源 5.2.2 菜单资源、图像资源、动画资源 5.2.3 其他资源 原生 xml 资源 raw 资源 特殊 Drawable 资源 动画资源 自定义属性资源 第 2 周：【应用核心组件初识】 第 6 天： Activity 及页面跳转 6.1 Activity 的声明和使用 6.1.1 创建 Activity

6.1.2 在清单文件中配置 Activity 6.1.3 启动 Activity 6.2 Activity 生命周期 6.2.1 Activity 生命周期的作用 6.2.2 Activity 生命周期 方法 6.2.3 Activity 生命周期方法执行顺序 6.2.4 横竖屏切换时 Activity 生命周期变化（Manifest.xml 设置 configChange） 6.3 Activity 现场保护 6.4 Activity 基本页面跳转及传值 6.4.1 使用 Intent 实现页面跳转 6.4.2 使用 Bundle 实现传递对象 6.4.3 使用 Application 全局对象传值 6.5 Activity 具有返回值的页面跳转

6.5.1 启动 Activity 回传数据 第 7 天：Activity 启动模式及 Intent

7.1 Task 和 Back Stack 的基本概念 7.1.1 Task 的介绍 7.1.2 Back Stack 的介绍 7.1.3 Task 和 Back Stack 的关系 7.1.4 退出 APP 时销 毁回退栈中所有 Activity 7.2 Activity 的启动模式 7.2.1 启动模式 的简介 7.2.2 启动模式的应用 7.3 Intent 属性的特点及用法 第 8 天： AsyncTask 异步任务 8.1 使用异步任务的原因 8.1.1 Android 中线程使用规则 8.1.2 异步任务使用步骤 8.2 异步任务 的应用 8.2.1 AsyncTask 中范型参数说明 8.2.2 AsyncTask 中方 法的说明 8.2.3 异步任务与线程池 8.2.4 异步任务的取消 第 9 天： ListView 基本用法及适配器介绍 9.1 AdapterView 与 Adapter 简介 9.1.1 AdapterView 的范畴 9.1.2 Adapter 的作用 9.2 ListView 基本用法 9.3 SimpleAdapter 9.4 BaseAdapter 9.4.1

BaseAdapter 中的四个方法的说明 9.4.2 ListView 的 ConvertView 复用 第 10 天：ListView 优化及分页、GridView 10.1 ListView 优 化 10.1.1 内存空间优化(ConvertView) 10.1.2 运行时间优化

（ViewHolder） 10.1.3 ListView 的 item 多布局的复用 10.2

ListView 滚动监听实现分页加载数据 10.2.1 ListView 滚动事件

OnScrollListener 10.2.2 ListView 实现分页效果 10.3 GridView 加

载图片 10.3.1 GridView 的常用属性 10.3.2 GridView 的基本用 法 10.3.3 GridView 的事件 扩展部分- ExpandableListView – 录 视频 第 3 周：【Menu、Dialog、数据存储】 第 11 天：菜单及 对话框 11.1 OptionsMenu 11.1.1 OptionsMenu 创建方式 11.1.2

菜单项点击事件 11.2 ContextMenu 11.2.1 ContextMenu 创建方

式 11.2.2 上下文菜单项点击事件 11.2.3 上下文菜单绑定注册

11.3 PopupMenu 11.3.1 PopupMenu 的创建 11.4 PopupWindow

11.5 AlertDialog 11.5.1 AlertDialog 的创建及点击事件 11.6 ProgressDialog 11.6.1 ProgressDialog 的创建及样式 11.7 列表对 话框 11.7.1 列表对话框的创建 11.8 自定义 Dialog 11.8.1 自定 义 Dialog 的实现 第 12 天：数据存储 12.1 SharedPreferences

12.1.1 SharedPreferences 使用场景; 12.1.2 SharedPreferences 的 常用方法 12.2 内部存储 12.2.1 内部存储的概念 12.2.2 内部存 储的实现 12.3 外部存储 12.4 存储 Bitmap 图片到外部存储 第 13 天：SQLite 数据库与 CursorAdapter 适配器 13.1 回顾 SQLite 13.1.1 SQLite 数据库的特点 13.1.2 SQL 常用语法 13.2 SQLiteOpenHelper 的用法 13.3 CursorAdapter 13.3.1 CursorAdapter 的用法 13.3.2 CursorAdapter 结合 ViewBinder 第 14 天：ContentProvider 14.1 ContentResolver 实现系统数据库的 操作 14.1.1 ContentProvider 与 ContentResolver 的概念及关系

14.1.2 利用 ContentResolver 实现系统数据的操作 14.2 自定义 ContentProvider 14.2.1 自定义 ContentProvider 的实现步骤 第 15 天：Loader 15.1 CursorLoader 的用法 15.1.1 CursorLoader 的使 用场景 15.1.2 CursorLoader 的用法 15.2 AsyncTaskLoader 加载 本地数据 15.2.1 AsyncTaskLoader 与 CursorLoader 对比 15.2.2 AsyncTaskLoader 的用法 周末案例：对本周知识点综合练习

【带离线阅读的新闻系统】 第 4 周： 【移动开发主流界面实 现】 第 16 天：动画资源 16.1 帧动画 16.1.1 帧动画的具体实现

16.2 补间动画 16.2.1 补间动画的类型（透明度、缩放、旋

转、平移、AnimationSet） 16.2.2 补间动画的动画资源的常用

属性及实现方法 16.2.3 补间动画的 Java 代码实现方法 16.2.4

补间动画的监听方法 16.3 属性动画 第 17 天：Fragment 17.1

Fragment 基本用法 17.1.1 Fragment 简介 17.1.2 Fragment 生命周

期 17.1.3 静态 Fragment 17.1.4 动态 Fragment 17.1.5

FragmentTransaction 17.1.6 Fragment 的回退栈 17.2 Fragment 传

值 17.2.1 Fragment 与 Activity 之间的传值 17.2.2 Fragment 之间传

值 17.3 Fragment 性能优化 17.3.1 Fragment 优化的必要 17.3.2 Fragment 优化相关方法 第 18 天：ViewPager 18.1 ViewPager 与 适配器 18.1.1 ViewPager 的基本使用（ViewPager 实现欢迎引导

页） 18.1.2 ViewPager 的适配器 18.2 ViewPager 加载网络图片

18.2.1 ViewPager 加载网络图片实现广告效果 18.3 PagerAdapter 的优化 18.3.1 PagerAdapter 优化的必要和实现 第 19 天：书签导航 19.1 书签导航多种实现效果展示 19.1.7 ViewPageIndicator（第三方技术） 19.2 RadioGroup + ViewPager + Fragment 实现导航 19.3 HorizontalScrollView + ViewPager + Fragment 实现导航 第 20 天：Handler、Looper 消息 传递机制 20.1 Handler、Looper 消息传递机制的原理 20.1.1

Handler 简介 20.1.2 Handler 具体用法 20.1.3 Handler、Looper 消

息传递机制的原理分析 20.2 Handler、Looper 源码 20.2.1 Handler、Looper 源码分析 周末综合练习【涵盖前四周所有知 识点】 周末作业包括：安装 Android Studio。 第 5 周：【应用 核心组件进阶】 【注】必须使用 Android Studio 开发环境教学 第 21 天：ActionBar （Action View、SearchView）+ ToolBar

21.1 ActionBar 21.1.1 ActionBar 介绍(支持 V7 的 ActionBar:android.support.v7.app.ActionBar） 21.1.2 AppCompatActivity、ActionBarActivity 介绍 21.1.3 ActionBar 的 用法 21.1.4 Action View 的介绍 21.1.5 SearchView 的用法 21.2 ToolBar 21.2.1 ToolBar 介绍 21.2.2 ToolBar 的用法 第 22 天：

BroadcastReceiver 及 Notification 22.1 Notification 22.1.1

Notification 的作用 22.1.2 普通通知的用法 22.1.3 PendingIntent

的用法 22.1.4 Notification 的 Flag 属性 22.1.5 大视图通知 22.1.6

进度条通知 22.1.7 自定义通知 22.2 广播接收器 22.3 自定义发 送广播 第 23 天： Service 基础 23.1 Service 介绍 23.1.1 Service 的 概念及使用场景 23.1.2 Service 的分类 23.1.3 Service 生命周期

23.1.4 Service 注册 23.2 Start Service 23.2.1 Start Service 实现音 乐播放器 23.2.2 粘性服务与非粘性服务 23.3 IntentService 23.4 Bind Service 23.4.1 Bind Service 实现音乐播放器 23.5 两种服务 混合使用实现 MediaPlayer 音乐播放 第 24 天： 跨进程的 Service 24.1 AIDL 24.1.1 AIDL 的概念 24.1.2 AIDL 的用法 24.2 Messenger 24.2.1 Messenger 的概念 24.2.2 Messenger 的用法 第 25 天：LruCache 与 Bitmap 二次采样 25.1 LruCache 25.1.1 LruCache 的概念 25.1.2 LruCache 的用法 25.2 二次采样 25.2.1 二次采样的意义 25.2.2 封装二次采样生成缩略图工具类 周末 综合作业 音乐播放器 第 6 周：【View 深入探究】 第 26 天： 百 度地图 26.1 百度地图基本用法 26.1.1 百度地图 API 概述 26.1.2 百度地图密钥申请 26.1.3 百度地图配置 26.1.4 显示基本地图

（交通地图、卫星地图、热力地图） 26.1.5 百度地图定位

26.1.6 百度地图覆盖物基本用法 26.1.7 混淆的意义及地图的

混淆配置 26.2 百度地图搜索 26.2.1 POI 检索 26.2.2 出行线路 规划（公交、步行、自驾） 26.2.3 公交路线查询 第 27 天： 自 定义 View（一） 27.1 自定义 View 介绍 27.1.1 为什么自定义

View 27.1.2 View 和 ViewGroup 的职责回顾 27.1.3 自定义 View

的常规做法 27.1.4 自定义 View 的构造方法规则 27.2 NotePad 继承已有控件方式的自定义 View 27.2.1 绘制 onDraw 的说明 27.2.2 onDraw 方法的注意事项 不要创建对象 27.2.3 Canvas, Paint, drawLine 简介 27.2.4 自定义属性 第 28 天：自定义 View（二） 28.1 继承于 ViewGroup 的自定义 View 28.1.1 重写

View 中的 onLayout()方法 28.1.2 实现自定义流式布局

FlowLayout 28.2 自绘制的自定义 View 28.2.1 重写 View 中的

onDraw()方法 28.2.2 画布画笔（Canvas、Paint） 28.2.3 重写

View 中的 onMeasure()方法 第 29 天：滑动视图 29.1

PullToRefresh 框架 29.1.1 配置 29.1.2 事件回调 29.1.3 多种控

件 29.1.4 PullToRefreshBase 重写 29.2 SlidingPaneLayout 29.2.1 左侧或右侧滑动 29.3 DrawerLayout 使用 第 30 天： 机型适配 及 Git 30.1 机型适配介绍 30.1.1 Android 中机型适配出现的原

因 30.1.2 机型适配的思路 30.2 屏幕相关重要概念回顾 30.2.1

屏幕尺寸 30.2.2 屏幕分辨率 30.2.3 屏幕像素密度及密度比值

30.2.4 dp、dpi、sp、px 30.2.5 mdpi、hdpi、xhdpi、xxhdpi 30.3 机型适配的解决方案 30.3.1 屏幕适配 30.3.2 版本适配 30.3.3 语言自适应 30.4 Git 的使用 30.4.1 Git 介绍 30.4.2 使用 Git 的必 要性 30.4.3 Git 的使用 二、Android 项目实战阶段： 1\. 32.1 MVC 与 MVP 设计模式 2\. 开发流程 3\. glide 图片加载 4\. JSON 5\. AsyncTask 6\. HTTP( okHttp+Handler) 7\. SQLite 8\. ListView 多 布局 9\. Service 10\. MediaPlayer 11\. Notification 12\. ViewPager

13\. Fragment 14\. TabLayout 14.1 与 ViewPager 配合 14.2 自定义 Tab 15\. BroadcastReceiver 耳机拔出 16\. SharedPreferences 17\. 打包，混淆、多渠道打包 第 8 周：【Android 新技术】 第 36 天：视频播放器 36.1 视频播放器 VideoView 36.2 SurfaceView 及 MediaPlayer 36.2.1 SurfaceView 介绍与 View 区别 36.2.2 SurfaceHolder 与 CallBack 36.2.3 MediaPlayer.setDisplay 36.2.4 MediaPlayer 加载网络视频 36.3 播放器全屏显示与恢复 36.3.1 VideoView 全屏显示 onMeasure 重写 36.3.2 Activity 点击切换 横屏方法 36.4 ListView 的 item 实现视频播放 36.4.1 Item 显示视 频 36.4.2 单 Item 播放 36.4.3 Item 滚出时停止播放 第 37 天： RecyclerView 37.1 5.0 新技术介绍（Material Design） 37.1.1 设 计理念 37.1.2 新增控件 37.2 CardView 用法 37.3 RecyclerView 的用法 37.4 RecyclerView 与 ListView 比较 37.5 SwipeRefreshLayout 37.5.1 配置 37.5.2 事件回调 37.5.3 与 RecyclerView 的配合 扩展部分：第三方 UltimateRecycerView 第 38 天：Material Design 全新设计风格 38.1 TextInputLayout

38.1.1 错误监听 38.2 CoordinatorLayout 38.2.1 Toolbar 与 CoordinatorLayout 38.2.2 Behavior 38.2.3 AppBarLayout 38.2.4

NestedScrollView 38.2.5 CollapsingToolbarLayout 38.3 Snackbar

38.3.1 监听 Action 38.4 FloatingActionButton 38.4.1 属性介绍

38.4.2 onClick 事件处理 第 39 天：拍照、传感器、ZXing 二维码

39.1 利用 Intent 实现摄像头拍照 39.1.1 Intent 拍照返回 Bitmap 方 式 39.1.2 Intent 拍照保存文件方式 39.2 加速度传感器实现《摇 一摇》 39.2.1 传感器获取：传感器类型、默认传感器、传感 器列表 39.2.2 传感器监听注册 39.2.3 加速度传感 摇一摇 39.3 ZXing 实现生成二维码（容错等级、二维码正中心 Logo） 39.3.1 二维码生成，生成 BitMatrix 转 Bitmap 39.3.2 配置生成时 的容错等级 39.3.3 形成带有中心 Logo 的二维码 39.4 ZXing 实 现二维码扫描 39.4.1 导包 39.4.2 附加代码包含扫描 Activity

39.4.3 ZXing Activity ACTION 与 扫描操作； 第三方框架

zxing-android-embedded 第 40 天：JPush 推送、第三方登录、友 盟统计分析 40.1 JPush 极光推送的原理及用法 40.1.2 通知推送

40.1.3 消息推送 40.1.4 推送原理 40.2 第三方登录 40.2.1 第三

方登录说明 40.2.2 友盟 API 的使用 40.3 友盟统计分析 40.3.1

应用的创建与申请 40.3.2 统计 API 的说明，启动统计与页面统 计 【第 8 周综合案例】 第 9 周：【流行技术杂项】 第 41 天：加 密解密 41.1 对称加密（AES 、DES、3DES） 41.2 非对称加 密（RSA） 41.3 消息摘要（MD5、 SHA-1 ) 41.4 编码解码

（Base64、URLEncode、URLDecode） 第 42 天：网络支付 42.1 购物车 42.2 [Alipay 支付] 42.3 [微信支付] 第 43 天： 事件分 发原理 43.1 事件分发消费机制原理 43.1.1 事件分发消费机制

的原理分析 43.1.2 事件分发三大方法 43.2 事件分发消费机制

的应用场景 43.2.1 如何解决 ScrollView、ListView 的嵌套

43.2.2 解决 ListView 中 item 的 Button 事件冲突 43.2.3 DrawerLayout 及其中的事件冲突问题的解决 第 44 天： 高性能 ORM 框架与 WebApp 44.1 ORM 框架 44.1.1 Dagger2/ormlite

44.1.2 Dagger2 与 Retrofit 组合应用— 选讲 扩展 greenDao —录 视 44.2 Android WebView 应用 44.2.1 网页的加载 44.2.2 WebClient 网址拦截 44.2.3 WebChrome 网址进度、标题接收 简介 44.2.4 网址导航 前进、后退、历史管理 44.2.5 Web 页面

与本地代码的通信 44.2.6 JS 与 Java 间的交互 44.2.7 WebApp

混淆的配置 到这里差不多就结束了，欢迎转发~ 2018-03-16

评论区：

郑惜娟 : 请问有相关的配套视频吗?

小猿 : 这个是整套的 Android 视频链接： 密码：4mw8[百度网盘](https://pan.baidu.com/s/1pTCgH8CIkXGLtWZ53uydeA)[+](https://pan.baidu.com/s/1pTCgH8CIkXGLtWZ53uydeA)[请输入提取密码](https://pan.baidu.com/s/1pTCgH8CIkXGLtWZ53uydeA) 郑惜娟 : 非常感谢

郑惜娟 : 链接失效了

小猿 : 链接： 密码：5qux 失效你加我微信 18159020735，私聊我，我私发你[百度网盘](https://pan.baidu.com/s/1-SchfiEo0j1sYYYqWSRiyA)[+](https://pan.baidu.com/s/1-SchfiEo0j1sYYYqWSRiyA)[请输入提取密码](https://pan.baidu.com/s/1-SchfiEo0j1sYYYqWSRiyA) 路过 : 第 8 周的 31,32,33,34,35 天的学习计划没有

王丰 : 俺是新开的，俺也要[撇嘴]

关注公众号"懒人找资源"，星球资源一站式服务