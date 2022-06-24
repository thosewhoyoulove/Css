<!--
 * @Description: 
 * @Author: 曹俊
 * @Date: 2022-06-24 20:48:49
 * @LastEditors: 曹俊
 * @LastEditTime: 2022-06-24 20:55:47
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
