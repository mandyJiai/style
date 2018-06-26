# horizontalMutiDiv

## 关于
目前采用三种方式实现多个div横向排列，分别是：
- display： inline-block;
- float: left;
- display：flex；

demo适合场景：
- 文字和图片横向排列
- 多个块元素横向排列
- 多块元素宽度自适应
## 说明
### 1、display: inline-block;
这种是我个人比较常用的方式，因为会考虑IE8的兼容性，而且写法非常方便容易理解，尤其对于px的掌握可以更加精确。
注意点：
- 父元素加font-size:0px；清除inline-block的默认间隙。 
- vertical-align的使用，尤其是span标签和img标签是，同时设置vertical-align: middle，可以使两者垂直居中。
- 如果要是自适应宽度，注意calc的使用，要减去margin和padding的距离。

### 2、float: left;
个人不太经常使用浮动，浮动会增加冗余代码。记得清除浮动就好，清除浮动与三种方法，代码里只给出了利用伪元素清除法。

### 3、display: flex；
如果不考虑IE的兼容性，flex是非常好的选择，只需父元素设置一下布局方式就可以，并且可以完美的兼容手机端，推荐。
## 感谢
如果有更好的方法欢迎留言指教，感激不尽！