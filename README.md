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

