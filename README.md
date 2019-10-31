# Regain-the-front-end
Regain the front end 重拾前端

## Css 部分
### Css 选择器
- id,*  选择指定元素中被用户选中的内容
- ,     联合选择器
- 空格   子孙(后代)选择器
- >     子选择器
- []    属性选择器

### 定位与盒子
- position 定位
	* absolute 绝对定位 相对于浏览器
- overflow 溢出处理
	* visible 默认值  内容不会被修剪  会呈现
	* hidden 超出部分被隐藏
	* scroll 无论是否需要 都显示滚动条
	* auto 自动
- outline (和overflow结合使用) 溢出的边框
	* dashed 虚线
	* dotted 点状轮廓
	* solid 实线
	* double 双实线
- box-sizing  
	* content-box 在宽度和高度之外绘制元素和边框
	* border-box  已设定的宽度和高度分别减去边框和内边距才能得到内容的高度和宽度

### 浮动 
- 破坏  包裹  特性
- 清除浮动方法1
```html
<style>
	.clearfloat {
		clear:both;
	}
</style>
```
- 清除浮动放法2
```html
.clearfix:after {
	content: "";
	display: block;
	height: 0;
	clear:both;
	visibility: hidden;
}
```

### 定位专题
- position 
	* relative 相对 相对于自己以前的位置  [元素空间位置会被保留]
	* absolute 绝对 相对于最近的祖先元素(如果没有就相对于body)  [元素空间位置不会被拆除] 有遮挡的效果
	* static   无
	* fixed    固定
- 绝对定位于float
	* 相同点
		* 都会产生浮动
		* 都会破坏文档流
	* 不同点
		* float 文档流的其他内容(不会忽略)dir的位置
		* adsolute 文档流的其他内容 (会忽略) dir的位置
- 浮动和相对定位
	* 定位可以设置相对距离  浮动是让它脱离文本流

## JavaScript 部分
