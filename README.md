#jquery-Microslider

#slider_json.js ，为自定义的JSON 格式参数，例如：
var slider_json = [
	{
		"imagePath": "images/c1.jpg",
		"order": "2",
		"url": "#刘若英",
		"slideText": "刘若英巡回演唱会"
	}
];

#加载CSS~	
'''html
<link rel="stylesheet" href="css/font-awesome.css">
<link rel="stylesheet" href="css/slider.css">
<link rel="stylesheet" href="css/demo.css">
'''

#加载JS
'''html
<script type="text/javascript" src="jquery-3.1.0.min.js"></script>
<script type="text/javascript" src="slider_c.js"></script>
<script type="text/javascript" src="slider_json.js"></script>
'''

#应用
'''html
var qq = $.slider_mm({
	"obj" :$("#slider") ,  
	"json":slider_json 
}) ;
'''
##禁用图片另存为
'''html
$("#slider img").bind("contextmenu",function(e){   
	return false;   
});
'''
