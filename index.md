## Welcome to Yiwu
<!DOCTYPE html>
<meta name="viewport" content="initial-scale=1.0, user-scalable=no" />  
<style type="text/css">  
    html{height:100%}    
    body{height:100%;margin:0px;padding:0px}    
    #container{height:100%}    
</style> 
<script type="text/javascript" src="https://api.map.baidu.com/api?v=2.0&ak=LXpXl6bnXk8EPypPqxwu1CL1s2j0jLU9"></script>
<div id="container"></div> 
var map = new BMap.Map("container"); 
var point = new BMap.Point(116.404, 39.915); 
map.centerAndZoom(point, 15);  
var map = new BMap.Map("container");    
var point = new BMap.Point(116.404, 39.915);    
map.centerAndZoom(point, 15);    
window.setTimeout(function(){  
    map.panTo(new BMap.Point(116.409, 39.918));    
}, 2000);

