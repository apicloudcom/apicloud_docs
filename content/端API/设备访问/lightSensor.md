/*
Title: lightSensor
Description: lightSensor
*/

<p style="color: #ccc;margin-bottom: 30px;">来自于：开发者</p>

<ul id="tab" class="clearfix">
	<li class="active"><a href="#method-content">Method</a></li>
</ul>
<div id="method-content">

<div class="outline">
[startListener](#a1)
[closeListener](#a2)


</div>

#**概述**

lightSensor封装了android的光传感器，使用此模块可轻松实现对光照亮度获取的功能


#**startListener**<div id="a1"></div>

打开光传感器

startListener({params}, callback(ret, err))

##params



type：

- 类型：数字
- 默认值：无
- 描述：不能为空，可选填0(特别快游戏用),1(游戏用 ),2(用户接口用 ),3( 取得倾斜度的时候使用)

##callback(ret, err)

ret：

- 类型：JSON 对象

内部字段：

```js
{
	state:		//该传感器是否可用
	x:              //亮度（LX）
	
}
```

##示例代码

```js
var lightSensor = api.require('lightSensor');


lightSensor.startListener({type:1},function(ret, err){api.alert("可获取状态:"+ret.state+"亮度:"+ret.x)});
```

##补充说明

无

##可用性

Android系统

可提供的1.0.0及更高版本

#**closeListener**<div id="a2"></div>

关闭光传感器


closeListener()




##示例代码

```js
var lightSensor = api.require('lightSensor');


lightSensor.closeListener();
```

##补充说明

无

##可用性

Android系统

可提供的1.0.0及更高版本


