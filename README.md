# leaflet-echarts
A plugin for leaflet to load echarts map and make BigData Visualization.
## 基于leaflet 扩展echarts，使ECharts的地图可以加到leaflet上

> 根据百度地图echarts的扩展改写，在事件联动这个地方以及echarts的容器与地图容器在拖动和缩放中的适应上耗费了很长时间，为了兼容echarts的map其他类型的数据又下了不少功夫。现在可以算是一个稍微完美的版本了。

# [在线访问(Demo)](http://wandergis.github.io/leaflet-echarts)

# 使用方法（Usage）

1. Confirm you have import `leaflet` first, 引入leaflet的js和css库自然不用说 
2. Import `eaflet-echarts.js` ,可以通过npm安装，输入`npm install leaflet-echarts` 即可
3. Import `echarts.source.js` under directory `lib` 引入lib目录下的`echarts.source.js`文件
4. As you can use this plugin like this,按照下面的方法使用

	```
		var overlay = new L.echartsLayer(map, echarts);
    	var chartsContainer=overlay.getEchartsContainer();
    	var myChart=overlay.initECharts(chartsContainer);
    	var option={};//这里跟百度echarts的map的option一样,the option is same as echarts map
    	overlay.setOption(option);
   	 ```
 5. If you don't konw how to use this plugin,hava a look at `/examples/index.html`,如果你不会用，看看examples目录下的`index.html` 
# 截图示例

![](http://7xp11v.com1.z0.glb.clouddn.com/15-12-11/73352372.jpg)

# 参考

>[https://github.com/ecomfe/echarts](https://github.com/ecomfe/echarts)