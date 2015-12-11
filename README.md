# leaflet-echarts
A plugin for leaflet to load echarts map and make BigData Visualization.
## 基于leaflet 扩展echarts，使ECharts的地图可以加到leaflet上

> 根据百度地图echarts的扩展改写，在事件联动这个地方以及echarts的容器与地图容器在拖动和缩放中的适应上耗费了很长时间，为了兼容echarts的map其他类型的数据又下了不少功夫。现在可以算是一个稍微完美的版本了。
# [在线访问](http://wandergis.github.io/leaflet-echarts)

# 使用方法（Usage）

1. 引入leaflet的js和css库自然不用说
2. 引入leaflet-echarts库，可以通过npm安装，输入`npm install leaflet-echarts` 即可
3. 引入lib目录下的`echarts.source.js`文件
4. 按照下面的方法使用

	```
		var overlay = new L.echartsLayer(map, echarts);
    	var chartsContainer=overlay.getEchartsContainer();
    	var myChart=overlay.initECharts(chartsContainer);
    	var option={};//这里跟百度echarts的map的option一样
    	overlay.setOption(option);
   	 ```
   	 
# 截图示例

![](http://7xp11v.com1.z0.glb.clouddn.com/15-12-11/73352372.jpg)