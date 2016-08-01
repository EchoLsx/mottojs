# MottoJS
Show your motto in an amazing way!


# 用法
create a html tag such as `<h1></h1>` etc
```
<h1 class="motto"></h1>
```
then include `MottoJS` 

```
<script src="motto.min.js"></script>
```

then use `new` to create a MottoJS instance
```
var motto = new Motto(el, config)
```
# 参数
`MottoJS` 接受两个参数
- ### el {String / HTML element} `required`
use CSS selector to select a html element for showing the motto.

- ### config {Object} `required`
it's an object with five optional properties.

# 配置
基本的配置对象如下：
```
{
    lyric: 'To be or not to be, that\'s a question.',
    showUpSpeed: 1000,
    flashSpeed: 100,
    flashTimeout: 1000,
    callback: function() { ... }
}
```
- #### lyric {String} `optional`  `default: ''`
你的内容


- #### showUpSpeed {Number} `optional` `default: 0`
文字会一个字一个字地出现，这个选项用于设置它们出现的间隔时间。

- #### flashSpeed {Number} `optional` `default: 0`
控制文字从乱码转化成有意义的句子的时间

- #### flashTimeout {Number} `optional` `default: 0`
设置从句子完全输出到乱码转换之间的过渡时间

- #### callback {Function} `optional` `default: {}`
乱码转换完后的回调函数


