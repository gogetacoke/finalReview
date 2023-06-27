# Kontlin数据类型

1. 基本数据类型

   + 整数

     byte、sort、int、long

   + 浮点数

     float、double

   + 布尔

     boolean

   + 字符

     char

2. 字符串类型

   string

3. 数组类型

   array

4. 集合类型

   list、mutableList、set、map、mutableSet、mutableMap

5. 空安全类型

   可空类型(表达式或变量可能为null)、非空类型(表达式或变量必定不为null)

6. 其他特殊类型

   any、unit、nothing

# var与val区别

+ **var** 用于声明**可变变量**，即变量的值可以在声明后被修改
+ **val**用于声明**不可变变量**，即变量的值在声明后不能再被修改

# 函数定义

+ 使用fun关键字定义函数

  ```kotlin
  fun 函数名(参数列表): 返回类型 {
      // 函数体
      // 可选的返回语句
  }
  // 简单demo
  fun greet(name: String) {
      println("Hello, $name!")
  }
  // 使用=来定义函数的单行表达形式，省略return关键字
  fun addNumbers(a: Int, b: Int) = a + b
  ```
# 继承

+ 使用  **:**  表示继承关系

  ```kotlin
  // 单继承
  open class Animal{
      open fun sound(){
          println("This animal")
      }
  }
  class Dog:Animal(){
      override fun sound(){
          println("The dog barks")
      }
  }
  // 多继承
  interface Walkable {
      fun walk()
  }
  
  interface Swimmable {
      fun swim()
  }
  
  class Human : Walkable, Swimmable {
      override fun walk() {
          println("The human is walking")
      }
  
      override fun swim() {
          println("The human is swimming")
      }
  }
  ```

# when表达式

+ 用于多条件分支语法结构

  ```kotlin
  when (expression) {
      value1 -> {
          // 执行逻辑1
      }
      value2 -> {
          // 执行逻辑2
      }
      value3, value4 -> {
          // 执行逻辑3
      }
      else -> {
          // 默认逻辑
      }
  }
  // 例子
  fun describeNumber(number: Int) {
      when (number) {
          1 -> println("One")
          2 -> println("Two")
          3, 4 -> println("Three or Four")
          else -> println("Other")
      }
  }
  
  describeNumber(2)  // 输出：Two
  describeNumber(5)  // 输出：Other
  ```

# 系统架构层分类

+ 表现层
+ 应用层
+ 领域层
+ 基础设施层

# 四大组件

+ 活动 activity
+ 服务 service
+ 广播接收器 broadcastReceiver
+ 内容提供器 contentProvider

# Activity生命周期

+ onCreate()
+ onStart()
+ onResume()
+ onPause()
+ onStop()
+ onRestart()
+ onDestory()

# Intent理解显示与隐式区别

+ 显示Intent（Explicit Intent）是**明确**指定了目标组件的Intent。它通过指定目标组件的类名或包名与类名的方式来明确指定要启动的组件
+ 隐式Intent（Implicit Intent）是**没有明确**指定目标组件的Intent。它通过指定操作（Action）和数据（Data）来描述所需的操作，然后由系统根据

> 显示Intent适用于启动特定的组件，适用于应用内部的组件调用。
>
> 而隐式Intent适用于更通用的场景，可以调用其他应用的组件，或者通过系统提供的功能完成特定的操作，如发送邮件、拨打电话等

# Intent-Filter三部分

+ Action 操作
+ Data 数据
+ Category 类别

# Activity四种启动模式

+ 标准模式 Standard
+ 单顶模式 SingleTop
+ 单任务模式 SingleTask
+ 单例模式 SingleIstance

# 布局方式

+ 线性布局 LinearLayout
+ 相对布局 RelativeLayout
+ 约束布局 ConstraintLayout
+ 帧布局 FrameLyout
+ 网格布局 GridLayout
+ 表格布局 TableLayout

# 使用布局方式设置控件居中

+ 线性布局

  > 设置父容器的`android:gravity`属性为`center`，将控件在水平和垂直方向上居中对齐。

+ 相对布局

  > 使用`android:layout_centerInParent="true"`属性将控件置于父容器的中心位置。
  >
  > 或者使用相对位置的属性（如`android:layout_centerHorizontal="true"`和`android:layout_centerVertical="true"`）将控件水平或垂直居中。

+ 约束布局

+ 帧布局