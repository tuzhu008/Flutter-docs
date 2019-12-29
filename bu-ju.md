# 布局

## Container

添加 padding、margins、borders、background color 或将其他装饰添加到 widget。

使用 `constraints` 属性，创建一个新的 `BoxConstraints` 来设置 `minWidth` 或 `maxWidth`。

## Row

行布局容器。主轴是水平方向，交叉轴为垂直方向。

有前端经验的开发者，可以将其理解为使用 flex 布局的 DIV，`flex-direction` 为 `row` 。

## Column

列布局容器。主轴是垂直方向，交叉轴为水平方向。

有前端经验的开发者，可以将其理解为使用 flex 布局的 DIV，`flex-direction` 为 `column` 。

## Stack

可以允许其子 widget 简单的堆叠在一起

## Positioned

定位容器

## Center

居中

## Flutter 盒子模型

在Flutter中，widget由其底层的 [`RenderBox`](https://docs.flutter.io/flutter/rendering/RenderBox-class.html) 对象渲染。 渲染框由它们的父级给出约束，并且在这些约束下调整自身大小。约束由最小宽度、最大宽度和高度组成; 尺寸由特定的宽度和高度组成。

通常，按照widget如何处理他们的约束来看，有三种类型的盒子：



* 尽可能大。 例如 [`Center`](https://docs.flutter.io/flutter/widgets/Center-class.html) 和 [`ListView`](https://docs.flutter.io/flutter/widgets/ListView-class.html)  的渲染盒
* 跟随子 widget 大小。 例如，[`Transform`](https://docs.flutter.io/flutter/widgets/Transform-class.html) 和 [`Opacity`](https://docs.flutter.io/flutter/widgets/Opacity-class.html)  的渲染盒。
* 指定尺寸。 例如，[`Image`](https://docs.flutter.io/flutter/dart-ui/Image-class.html) 和 [`Text`](https://docs.flutter.io/flutter/widgets/Text-class.html)的渲染盒



