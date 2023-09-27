# technology-stack-summary

A summary about popular program frameworks.

[toc]

## GUI framework

### Qt

当前大版本Qt6，使用c++

KDE桌面管理器的核心组件

官网：[https://doc.qt.io/](https://doc.qt.io/)
all classes：[https://doc.qt.io/qt-5.15/classes.html](https://doc.qt.io/qt-5.15/classes.html)

### Gtk

当前大版本Gtk4，使用c语言

Gnome桌面管理器的核心组件

官网：[https://www.gtk.org/](https://www.gtk.org/)
文档：[https://www.gtk.org/docs/getting-started/hello-world/](https://www.gtk.org/docs/getting-started/hello-world/)

`Gnome Shell使用JavaScript和css来构建主题系统，拥有很好的扩展性。`

## 跨平台GUI框架

### Flutter

使用dart语言，由Facebook提供。

常用来写app，存在常用控件交互不合理问题。

官网：[https://flutter.dev/](https://flutter.dev/)
文档：[https://docs.flutter.dev/ui](https://docs.flutter.dev/ui)

## .NET相关UI框架

### WinForm

c#原生提供，不做解释。

### WPF

重量级UI框架，使用xml描述界面。

### MAUI

现代级别的UI库，稍轻量于WPF，跨平台，支持移动端，客户端，浏览器端。使用xml描述界面

官网：[https://dotnet.microsoft.com/en-us/apps/maui](https://dotnet.microsoft.com/en-us/apps/maui)

### MahApps.Metro

使用xml

官网：[https://mahapps.com/](https://mahapps.com/)

### GacUI - vczh提供

使用xml

官网：[http://gaclib.net/](http://gaclib.net/)

vczh代码库中有很多值得学习研究的c++相关的内容

```text
WYSIWYG
- What You See Is What You Get
- 所见即所得
```

## Lexer和Parser

### flex yacc

远古工具，弃用

### bison

现代工具
官网：[https://www.gnu.org/software/bison/](https://www.gnu.org/software/bison/)

`Bison is a general-purpose parser generator that converts an annotated context-free grammar into a deterministic LR or generalized LR (GLR) parser employing LALR(1) parser tables.`

### jflex

jetbrains插件使用的java版本的flex工具

### antlr4

lexer和parser生成器，guido推荐的！

基于Java，使用ebnf(强化版巴斯科范式)

提供更多功能，写grammar更顺滑。

### VlppParser2 - vczh

代码库：[https://github.com/vczh-libraries/VlppParser2](https://github.com/vczh-libraries/VlppParser2)

### 编程语言语法研究

词法着重研究DFA(确定有穷自动机)，语法着重研究lr(1)自动机。

| 文章简述           | 相关链接                                                                                                                                                                                   |
|----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| scala的bnf语法    | [https://www.scala-lang.org/files/archive/spec/2.11/13-syntax-summary.html](https://www.scala-lang.org/files/archive/spec/2.11/13-syntax-summary.html)                                 |
| 另一篇介绍          | [https://dotty.epfl.ch/docs/internals/syntax.html](https://dotty.epfl.ch/docs/internals/syntax.html)                                                                                   |
| 理解状态机          | [https://www.freecodecamp.org/news/state-machines-basics-of-computer-science-d42855debc66/](https://www.freecodecamp.org/news/state-machines-basics-of-computer-science-d42855debc66/) |
| lr parser介绍    | [https://www.geeksforgeeks.org/lalr-parser-with-examples/](https://www.geeksforgeeks.org/lalr-parser-with-examples/)                                                                   |
| 介绍lr(1) parser | [http://www.cs.ecu.edu/karl/5220/spr16/Notes/Bottom-up/lr1.html](http://www.cs.ecu.edu/karl/5220/spr16/Notes/Bottom-up/lr1.html)                                                       |
| 介绍巴斯科范式        | [https://slideplayer.com/amp/7715859/](https://slideplayer.com/amp/7715859/)                                                                                                           |

## 图形学

### OpenGL

mesa

`关键词：图形渲染管线,VAO,VBO,VFO,离屏渲染,glsl`

LearnOpenGL地址：[https://learnopengl-cn.github.io/](https://learnopengl-cn.github.io/)

渲染的三要素：

1. 模型
2. 材质(+贴图)
3. 光源

`问题：OpenGL在Windows和Linux中的安装`

`问题：如何将渲染过程变成程序的模块化代码？`

`问题：如何制作贴图？如深度贴图，法线贴图等 可借助工具`

`问题：如何制作粒子特效？`

PBR材质(Physically-Based Rendering)

原理性BSDF(双向散射分布函数)

#### 常用的OpenGL库

- glm - 矩阵库
- glfw - 窗口库
- glew

### Vulkan

教程参考：[https://geek-docs.com/vulkan/vulkan-tutorial/vulkan-tutorial-index.html](https://geek-docs.com/vulkan/vulkan-tutorial/vulkan-tutorial-index.html)

### Direct3D

`问题：Direct2D，DirectX，Direct3D之间的区别?`

### 常用建模工具

- blender
- 3dmax
- maya
- c4d - oc渲染器
- zbrush - 雕刻
- shapr3d - 三维设计

### VTK

### 更多三维应用

| 项目           | 简介                |
|--------------|-------------------|
| OpenCascade  | 三维设计，最佳实践：freecad |
| openscad     | 三维设计              |
| solvespace   | 三维设计              |
| WickedEngine | 渲染引擎              |
| godot        | 游戏引擎              |






