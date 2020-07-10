---
layout: post
title: 'BDD测试框架Cucumber学习记录'
date: 2020-07-08
author: Liuyuxin
color: rgb(255,245,238)
cover: '../assets/Image/cucumber.jpeg'
tags: 学习记录
---
### 什么是BDD

BDD（Behavior Driven Development)，行为驱动开发。
BDD可以让项目成员（甚至是不懂编程的）使用自然语言来描述系统功能和场景，从而根据这些描述步骤进行系统自动化的测试。

### Cucumber框架

Cucumber是一种可以使用文本描述语言来执行自动测试用例的工具，使用的语言叫做Gherkin。

Cucumber为我们建立一个**易读的**、**可执行**的特性文档。

1. **Cucumber三大组成**：Features、Step_definitions、Cucumber command

   其关键字含义与原有自动化测试工具中概念相同：

   | Cucumber | Unit Test  |
   | -------- | ---------- |
   | Feature  | Test suite |
   | Scenario | Test case  |
   | Given    | Setup      |
   | When     | test       |
   | Then     | assert     |

   **Feature**：用一些具有代表性例子描述一个用户需求

   **Scenario**：测试场景，一个用户特性涉及的一个关键用例

   **Step_definations**：步骤定义，测试用例中步骤的执行顺序

   2. 工作原理

      ![Cucumber工作原理]()

   

### Two ways of creating Cucumber dependencies

- 使用Maven dependencies
- 使用Library

---

#### 1. Maven Dependencies

1. 创建Maven Project

2. 在`pom.xml`文件中添加相关`dependencies`

   Eg:

   ```
   <dependency>
   	<groupId>info.cukes</groupId>
   	<artifactId>cucumber-java</artifactId>
   	<scope>test</scope>
   	<version>1.0.11</version>
   </dependency>
   <dependency>
   	<groupId>info.cukes</groupId>
   	<artifactId>cucumber-jvm</artifactId>				   				    
      <version>1.0.11</version>
   	<type>pom</type>
   </dependency>
   ```

   **注意**：version版本要与安装一致

   #### 2. 使用Libraries

   1. 在Maven工程中，点击`Project Structure`
   2. 点击`Modules` `Dependencies`
   3. 勾选相关以来包
   4. Apply改变

---

持续学习，持续更新。。。

