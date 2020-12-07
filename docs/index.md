### 首页
<strong><span style="font-size:20px;">一、CSS：</span></strong><br>
<br/>
1、全局封装平时用的多的样式，flex布局、清除浮动、边框、伪类等;
<br/>
2、样式的话，可以根据scss封装多个主题色，以便后期维护迭代；
<br/>
3、用的公用方法尽量写到外部引用，避免重复引用影响页面加载速度;
<br/>
4、手机端有些小标签、按钮在安卓上显示里面的文字会偏上或偏下;

```html
案例
a {
    height: 30px;
    line-height: 30px;
    font-size: 14px;
    text-align: center;
    width: 70px;
    vertical-align: middle;
}

解决方法：去掉line-height和vertical-align 使用 flex 布局。

把父元素设为：

display: flex;
align-items: center;
justify-content: center；
```
<br/>

?> <span style="font-size:13px;">备注：开始项目前必须要沟通好，一些细节的地方该怎么显示或功能模块，这样后期写页面时需要注意哪些地方，不然对接口时候会很耽误时间；</span>

<br/>
<strong><span style="font-size:20px;">二、JS：</span></strong><br>
<br/>
1、将工具方法封进Vue实例中，或写入mixin全局引入也可以；
<br/>
2、页面公共相同类型的值，最好全局写个过滤器给相同类型加上，因为你不知道后期会有什么更改；
<br/>

```html
案例
<p>{{price | changePrice}}</p>

```

<br/>
<br/>

# Arthur
那年那袅袅娜娜你能快乐<br>
的萨达喀纳斯的打死你袅袅娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜那你看打死你袅袅娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜你能看到打死你袅袅娜娜娜娜娜娜娜娜娜娜娜娜娜娜你能快乐大三那年那袅袅娜娜你能快乐<br>
的萨达喀纳斯的打死你袅袅娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜那你看打死你袅袅娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜娜你能看到打死你袅袅娜娜娜娜娜娜娜娜娜娜娜娜娜娜你能快乐大三那年那袅袅娜娜你能快乐<br>