<!--
 * @Description: 
 * @Author: 曹俊
 * @Date: 2022-06-24 20:57:48
 * @LastEditors: 曹俊
 * @LastEditTime: 2022-06-24 21:03:10
-->
# position的属性值
- static(静态布局)
- relative(相对布局)
- fixed(固定布局)
- absolute(绝对布局)
- sticky(粘性布局)

## 1. static布局
### 默认情况下，HTML 元素是静态定位的。

### 静态定位元素不受 top、bottom、left 和 right 属性的影响。
### 没有以任何特殊方式定位的元素；它总是按照页面的正常流程定位：
```css
div.static {
  position: static;
  border: 3px solid #73AD21;
  left:20px; //无效
}
```


## 2.relative布局
### 元素position: relative;相对于其**正常位置**定位。

### 设置相对定位元素的 top、right、bottom 和 left 属性将导致它被调整远离其正常位置。其他内容不会被调整以适应元素留下的任何间隙。