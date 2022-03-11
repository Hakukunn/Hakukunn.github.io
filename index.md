<html>
<head>
	<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
	<meta name="viewport" content="initial-scale=1.0, user-scalable=no" />
	<style type="text/css">
	body, html,#allmap {width: 100%;height: 100%;overflow: hidden;margin:1000;font-family:"微软雅黑";}
	</style>
	<script type="text/javascript" src="//api.map.baidu.com/api?v=2.0&ak=LXpXl6bnXk8EPypPqxwu1CL1s2j0jLU9"></script>
	<title>地图展示</title>
</head>

	<div id="allmap"></div>

</html>
<script type="text/javascript">
	// 百度地图API功能
	var map = new BMap.Map("allmap");    // 创建Map实例
	map.centerAndZoom(new BMap.Point(120.081007,29.451391), 11);  // main初始化地图,设置中心点坐标和地图级别
	//添加地图类型控件
	map.addControl(new BMap.MapTypeControl({
		mapTypes:[
            BMAP_NORMAL_MAP,
            BMAP_HYBRID_MAP
        ]}));	  
	map.setCurrentCity("义乌");          // 设置地图显示的城市 此项是必须设置的
	map.enableScrollWheelZoom(true);     //开启鼠标滚轮缩放
</script>
![yiwu](https://github.com/Hakukunn/Hakukunn.github.io/blob/main/yiwu.jpg)

[义乌介绍](https://baike.baidu.com/item/%E4%B9%89%E4%B9%8C/214555?fr=aladdin)	

      
//<img src="https://github.com/Hakukunn/Hakukunn.github.io/blob/main/yiwu.jpg" width="16px">
	<br>


