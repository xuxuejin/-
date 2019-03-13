在做移动端开发的时候，或多或少都会碰见一些疑难杂症，这里做一个记录，确保以后少踩坑，也希望能帮助到其他同学！

### 在微信中，点击可能不起作用，可能是内置浏览器不支持
    两种解决办法：
        1. 改为$(‘#select’).click(function(){}) 有效
        2. 给目标元素加一条样式规则 cursor: pointer;

### 移动端做层中层的滑动，不是很流畅
  解决办法：
    给外层容器加上overflow-y: scroll，同时设置属性-webkit-overflow-scrolling: touch;
  
  顺便提一下其他几个移动端可能会用到的属性
    
    // 文字抗锯齿
    -webkit-font-smoothing: antialiased
    
    // 避免点击a标签或者注册了click事件的元素时产生高亮
    -webkit-tap-highlight-color: transparent
    
    //禁用Webkit内核浏览器的文字大小调整功能
    -webkit-text-size-adjust: none
    
    // 阻止长按图片之后呼出菜单提示复制的行为 
    -webkit-touch-callout: none
