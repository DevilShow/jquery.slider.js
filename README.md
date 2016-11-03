# jquery.slider.js #
轮播图内容/项目符号/左右按钮均可由用户自行配置
## HTML 结构
```html
<div id="slider">
    <ul id="slider-items">
        <li class="slider-item"></li>
    </ul>
    <ul id="slider-tags">
    </ul>
    <div class="left-button"></div>
    <div class="right-button"></div>
</div>
```
## JavaScript 初始化
```JavaScript
$("#slider").slider({
    speed: 400,  //动画速度 (必须)
    interval: 4000,  //动画间隔 (必须)
    type: 'slide',  //动画类型 "slide" 或者 "fade" (默认为 "slide")
    direction: 'right',  //动画方向 "right" 或者 "left" (默认 "right")
    itemClass: '.slider-item',  //轮播图选择器 (必须)
    tagUl: '#slider-tags',  //项目符号选择器 (必须)
    tagClass: 'tag',  //项目符号样式 {class} 
    tagSelectedClass: 'tag-selected',  //项目符号选中样式 {class}
    isTurnButton: true,  //是否启用左右按钮
    leftButton: '.left-button',  //左按钮选择器
    rightButton: '.right-button',  //右按钮选择器
});
```
在该插件中所有样式，选择器是可自己配置的，选择器的作用是找到对应的元素，只要`js`中的选择器和`html`元素对应即可，用户可以编写自己的样式。
