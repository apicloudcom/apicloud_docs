/*
Title: brightness
Description: brightness
*/

<p style="color: #ccc;margin-bottom: 30px;">来自于：开发者</p>
		
<ul id="tab" class="clearfix">
	<li class="active"><a href="#method-content">Method</a></li>
    
</ul>
<div id="method-content">

<div class="outline">
[setBrightness](#a1)
</div>


#**概述**

brightness 封装了 Android 调节当前窗体亮度的功能，使用此模块可轻松实现对窗体亮度调节的功能。**暂仅支持 Android。**


#**setBrightness**<div id="a1"></div>

设置窗体亮度

setBrightness({params})

##params

Brightness：

- 类型：数字
- 描述：表示亮度，取值范围：0--255

##示例代码

```js
var brightness = api.require('brightness');
brightness.setBrightness({
    Brightness: 100
});
```

##可用性

Android 系统

可提供的1.0.0及更高版本

