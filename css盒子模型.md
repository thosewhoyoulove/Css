<!--
 * @Description: 
 * @Author: 曹俊
 * @Date: 2022-06-24 20:48:49
 * @LastEditors: 曹俊
 * @LastEditTime: 2022-07-06 16:09:35
-->
# CSS中的盒子模型包括IE盒子模型和标准的W3C盒子模型

### CSS盒子模型的组成：
- margin
- border
- padding
- content

## 标准盒子模型：
### 宽度 = content(width) + border + padding + margin
### 简单来说就是盒子的width和height的值只取决于内容(content)的宽高

## IE盒子模型
### 宽度 = (content+border+padding)(width) + margin
### 简单来说就是盒子的width和height不仅仅取决于内容的宽高，还取决于padding和border的值

## 可以通过box-sizing的值来指定盒子的类型

#### 属性值：
  1. content-box：默认值，标准盒子模型。 width 与 height 只包括内容的宽和高，不包括边框（border），内边距（padding），外边距（margin）。注意：内边距、边框和外边距都在这个盒子的外部。 比如说，.box {width: 350px; border: 10px solid black;} 在浏览器中的渲染的实际宽度将是 370px。
#### 尺寸计算公式：
- width = 内容的宽度
- height = 内容的高度
  
宽度和高度的计算值都不包含内容的边框（border）和内边距（padding）。

  2. border-box： width 和 height 属性包括内容，内边距和边框，但不包括外边距。这是当文档处于 Quirks 模式 时 Internet Explorer 使用的盒模型。注意，填充和边框将在盒子内 , 例如， .box {width: 350px; border: 10px solid black;} 导致在浏览器中呈现的宽度为 350px 的盒子。内容框不能为负，并且被分配到 0，使得不可能使用 border-box 使元素消失。

#### 尺寸计算公式：
- width = border + padding + 内容的宽度
- height = border + padding + 内容的高度