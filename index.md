
<!DOCTYPE html>
<html>
<head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <meta name="viewport" content="initial-scale=1.0, user-scalable=no" />
    <style type="text/css">
        body, html, #allmap {
            width: 100%;
            height: 100%;
            overflow: hidden;
            margin: 0;
            font-family: "微软雅黑";
        }
    </style>
    <script type="text/javascript" src="//api.map.baidu.com/api?type=webgl&v=1.0&ak=LXpXl6bnXk8EPypPqxwu1CL1s2j0jLU9"></script>
    <title></title>
</head>
<body>
    <div id="allmap"></div>
</body>
</html>
<script type="text/javascript">

    // 百度地图API功能
    var map = new BMapGL.Map("allmap");    // 创建Map实例
    map.centerAndZoom(new BMapGL.Point(120.070448, 29.320831), 11);  // 初始化地图,设置中心点坐标和地图级别
    map.enableScrollWheelZoom(true);     //开启鼠标滚轮缩放

    var point = new BMapGL.Point(120.070448, 29.320831);
    var marker = new BMapGL.Marker(point);  // 创建标注
    map.addOverlay(marker);              // 将标注添加到地图中

    var sContent =
"<h4 style='margin:0 0 5px 0;padding:0.2em 0'>义乌</h4>" +
"<img style='float:right;margin:4px' id='imgDemo' src='https://p8.itc.cn/q_70/images01/20210531/13599242b1bd4da98ca42fe2b0ff3b9c.jpeg' width='200' height='104' title='义乌市场'/>" +
"<a style='color:#87CEFA;text-decoration:none;' href='https://baike.baidu.com/item/%E4%B9%89%E4%B9%8C/214555?fr=aladdin'>更多信息见百度百科</ a>"
    "</div>";

    var infoWindow = new BMapGL.InfoWindow(sContent);     // marker添加点击事件
    marker.addEventListener('click', function () {
        this.openInfoWindow(infoWindow);
        // 图片加载完毕重绘infoWindow
        document.getElementById('imgDemo').onload = function () {
            infoWindow.redraw(); // 防止在网速较慢时生成的信息框高度比图片总高度小，导致图片部分被隐藏
        };
    });
</script>
