# Android 知识体系图谱

## 系统源码学习

### 组件

#### 四大组件解析

##### Activity

###### Activity的启动过程

###### 启动流程和启动模式

###### 生命周期

####### onNewIntent()

###### 与Window/View的关系

###### 与Fragment的关系

##### Service

###### IPC（AIDL）、IntentService

##### ContentProvider全方位解析

##### BroadcastReceiver全方位解析

###### 静态、有序、本地、粘性

#### Fragment

##### 懒加载

##### 与Activity通信

#### Context详解

#### Window

##### Toast

##### Dialog

##### PopupWindow

##### PopupWindow和Dialog区别

#### WebView

##### JSBridge

##### Deeplink

##### 首屏加速

##### 离线包

#### RecyclerView

##### 四级缓存+局部刷新

##### 与ListView比较

#### LinearLayout 和 RelativeLayout 相同层级下效率比较

### 系统服务

#### ActivityManagerService

#### Window和WindowManager

#### WindowManagerService

#### ServiceManager

### 流程

#### Android系统启动过程

##### system_server启动过程

#### Android Apk安装过程

#### Android应用进程启动

### 通讯

#### WIFI

#### NFC

#### 蓝牙

## 架构能力

### 设计模式

#### Android源码中的设计模式应用

#### OOD原则

### 架构模式

#### MVP

#### MVVM

##### DataBinding

#### Flux

#### Clean Architecture

#### Android Architecture Components

#### Android Jetpack架构

### App框架

#### 分包

#### 分层

## 开源库

### ORM框架

#### GreenDao

#### Room

### 事件总线

#### EventBus

##### 4种模式、粘性事件

##### 观察者模式解耦

### 网络

#### Retrofit

##### 动态代理

##### 运行时注解

##### GsonConverter

##### RxJava2CallAdapter

#### OKHttp

##### 拦截器（责任链模式）

##### 超时重传&重定向

##### Http缓存

##### Socket连接池复用

#### Volley

### 图片

#### Glide

##### 生命周期控制

##### 二级缓存

##### BitmapPool复用

#### Fresco

#### Picasso

### 依赖注入

#### butterknife

##### apt

#### Dagger2

### 序列化

#### Gson

#### FastJson

### ARouter

### 响应式编程

#### RxJava

##### 常用操作符

##### 线程调度

##### 异常处理

##### Flowable背压

#### RxBinding

#### RxAndroid

## 测试

### 单元测试

#### robolectric

### 自动化测试

#### UI自动化

#### Money

## 常见机制

### 线程通信

#### Handler原理

#### AsyncTask

#### HandlerThread

#### IntentService

#### RxJava

### 进程

#### IPC通信Binder

##### AIDL

##### 序列化

##### 匿名共享内存

#### lowmemorykiller 

#### 进程的优先级

### View体系

#### 自定义控件

##### 事件分发机制

###### 滑动冲突

###### 滑动、嵌套滑动

##### 自定义动画

##### Lottie动画解析库

##### 绘制

###### measure

###### layout

###### draw

####### requestLayout() 和 invalidate() 区别

### Android消息机制

### 本地存储

#### Sqlite、SharedPreferences、文件

### 资源管理系统、资源加载机制

## 基础能力

### Java高级

#### 反射

#### 动态代理

#### NIO

#### 垃圾回收和GC

#### 多线程（并发锁）

#### 网络协议

#### 集合框架

### 数据结构和算法

#### 线性表

#### 栈和队

#### 树

##### 树的基础

##### 其他常见的树

##### 并查集

##### B-树，B+树，B*树

#### 图

##### 图的基础

##### 拓扑排序

##### Kruskal算法、Prim算法、Dijkstra算法、Floyd算法

#### 散列查找

#### 排序

#### 海量数据处理

### 操作系统

### 计算机网络

#### DNS HTTP/1.x HTTPs HTTP/2 TCP 等网络协议知识

#### SSL

### 虚拟机

#### JVM

#### ART & Dalvik

##### AOT compilation 

##### GC

##### Bytecode & Dex

## 进阶

### 资源管理

#### 主题样式

#### 多分辨率适配

#### AssertManager

#### Resource

### 打包

#### Gradle

#### 编译

#### 混淆

#### 签名

### AOP

#### AspectJ

#### APT

#### Javassist

### 组件化

#### 页面路由

### 消息推送&保活

#### 长连接保活

##### 心跳包

#### 进程保活

### NDK

#### 调用JNI方法

#### 回调JAVA方法

#### CMAKE语法

#### NDK MakeFile语法

### 安全

#### root原理

#### 二进制漏洞挖掘

#### 经典的漏洞研究如cve20143153 cve20153636之类

#### poc和exp

#### 逆向

##### arm汇编

##### smali字节码

##### dex和ELF结构

##### 安卓和Linux调试体系和反调式体系

##### 加固与反加固

##### Hook

### 多媒体

#### 图片

##### 图片处理

###### Bitmap压缩策略

###### Bitmap裁剪

###### Bitmap复用

##### 动画

###### View动画、帧动画、属性动画

##### 图片加载

###### 缓存策略

####### LRUCache

#### 音视频

##### 音频编解码

##### AudioTrack播放

##### 视频解码

##### OpenGL绘制

##### 视频编辑转码

##### 视频滤镜

### 性能优化

#### 启动时间和冷启动优化

##### 避免启动白屏

#### Crash 收集分析

#### 卡顿检测和优化

##### ARR

##### 避免频繁GC

##### ViewHolder

#### 布局优化

##### include、merge、ViewStub的使用

#### 线程优化

#### 监控

##### 埋点

##### APM性能检测

##### WebView性能监控

##### leakcanary内存泄露监控

#### 内存优化

##### OOM

##### 内存泄露

##### 图片压缩

##### 内存分析

###### MAT

###### monitor

#### apk瘦身

#### 电量优化

#### 网络优化

##### 网络调试

###### Charles

###### Fiddler

###### tcpdump

###### postman

##### 低网速优化

##### API优化

##### 流量优化

### 持续集成

#### Jenkins

### 动态化

#### 混合开发

##### React Native

##### Fuchsia+Flutter+Dart

##### weex

##### JavaScript引擎

##### 渲染引擎

#### 插件化技术

##### class、dex基础知识

##### ClassLoader原理

###### 如何hook Activity启动流程

###### 双亲委派

##### 插件化原理

##### 插件化框架学习

#### 热修复

##### 插桩

###### ASM字节码

##### 类加载方式

##### 底层替换

## 其他

### Python

### Linux

#### kernel源码

#### SELinux

### Docker

## Android 书籍

### 入门

#### 第一行代码

#### Android群英传

#### Android编程权威指南

#### Android编程实战

### 进阶

#### Android开发进阶从小工到专家

#### 深入理解Android

#### Android组件化架构

#### App研发录

#### Android 进阶解密

#### Android 进阶之光

### 源码

#### Android源码设计模式解析与实战

#### Android开发艺术探索

#### Creating Dynamic UI with Android Fragments

### 安全

#### Android安全架构深究

#### Android软件安全与逆向分析

### 底层

#### Android系统源代码情景分析  

#### Android内核剖析

#### 深入理解Android内核设计思想  

## T型成长

### 团队管理

#### 敏捷

#### Devops

#### CodeReview

#### 代码质量与代码规范

### 自我管理

#### 代码质量

#### 时间管理

### 后端

#### 领域驱动设计

#### 微服务

## 语言

### Kotlin

### C、C++（NDK）

### SQL（DB）
