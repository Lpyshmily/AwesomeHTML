# AwesomeHTML
Learn web from Bilibili
## AV60293053 [十分钟实现数字增加效果](AV60293053/index.html)
CSS：Font Awesome图标；外部字体引入；渐变背景颜色（linear-gradient）；transfrom属性（translateY）；text-transfrom（改变字母大小写）

JS：counter-up实现数字增加效果

## AV60292728 [十分钟实现炫酷的更改背景色网站](AV60292728/index.html)

CSS：position属性（absolute、relative）；cursor属性（光标形状）；transition属性（延迟）；transfrom属性（translate、rotate）

JS：click（点击触发函数）；keyup（按键弹起触发函数）；toggleClass（增加或删除class）；css（改变CSS样式，属性-逗号-值）；val（获取input的值）

```js
// to have a preview of color
        $('#hex').keyup(function() {
            $('.prev').css("background", $('#hex').val());
        });
```

## AV61048562 [五分钟实现鼠标悬浮出现输入框效果页面](AV61048562/index.html)

CSS：line-height属性（行高）；display属性（设置display为flex后，可通过justify-height来调整对齐方向）；**伪选择器（:hover，:focus，特定动作时触发）**；>表示只选择儿子标签，不选择孙子标签

```css
/*鼠标悬浮在.email-box上时，会触发.tbox的CSS；*/
/*焦点位于.tbox时也会触发*/
.email-box:hover > .tbox, .tbox:focus {
    width: 260px;
    padding: 0 10px;
}
```

## AV59739071 [五分钟实现类似波浪的加载效果](AV59739071/index.html)

CSS：动画效果的实现（@keyframes创建关键帧/animation调用关键帧名称/设置动画时间、速度曲线、不同动画对象之间的延迟）

```css
/*使块体位于页面正中央*/
.middle {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
```

## AV61049670 [十分钟实现鼠标悬浮3D翻转效果网页](AV61049670/index.html)

CSS：text-decoration属性（去除文字装饰，如a标签默认的下划线）；overflow属性（规定当内容溢出元素框时发生的事情）；display属性的值为inline-flex时两个方向的对齐方法（justify-content、align-items）

**重点**：如何用CSS设置翻转效果

```
父元素 {
	/* 定义当元素不面向屏幕时是否可见 */
    backface-visibility: hidden;
}
要翻转的内容{
	/*定义透视高度和翻转角度*/
	transform: perspective(600px) rotateY(180deg);
}
```

## AV62031488 [五分钟实现文字流淌效果](AV62031488/index.html)

CSS：复习动画效果的实现（@keyframes创建关键帧/animation调用关键帧名称/设置动画时间、速度曲线、不同动画对象之间的延迟）；背景图片位置、大小、是否重复的设置（background-position/background-size）；background-clip（设置背景图片出现的范围：是否包含边框、只在文字下方出现背景）

## AV62032518 [十分钟实现图片模糊效果](AV62032518/index.html)

CSS：filter属性（滤镜，可用来实现模糊效果）`filter: blur(10px);`；rgba设置颜色（红、绿、蓝、透明度）；标签内实现事件监听；JS中使用DOM的style方法实现修改标签内容和CSS属性

```html
<button onclick="coverImage()" class="btn">Uncover Image</button>
```

```javascript
var btn = document.querySelector(".btn");
var text = document.querySelector(".text");
btn.innerHTML = "Cover Image"; //修改内容
text.style.display = "none"; //修改CSS属性
```

## AV62541314 [五分钟实现炫酷的加载效果](AV62541314/index.html)

CSS：复习动画效果的实现并设置动画延迟（animation-delay属性）；通过子标签的方法来指定标签（`.obj:n-th-child(2)`）；align-items属性指定flex弹性布局的对齐方式

```css
.obj:nth-child(2) {
    animation-delay: 0.1s;
}
```

