# opus
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>IFE JavaScript Task 01</title>
  </head>
<body>

  <h3>污染城市列表</h3>
  <ul id="aqi-list">
<!--   
    <li>第一名：福州（样例），10</li>
      <li>第二名：福州（样例），10</li> -->
  </ul>

<script type="text/javascript">

var aqiData = [
  ["北京", 90],
  ["上海", 50],
  ["福州", 10],
  ["广州", 50],
  ["成都", 90],
  ["西安", 100]
];
var str = '一二三';
function aa(){

  /*
  在注释下方编写代码
  遍历读取aqiData中各个城市的数据
  将空气质量指数大于60的城市显示到aqi-list的列表中
  */
var oul=document.getElementById("aqi-list");
var arr=[];
for(var i=0;i<aqiData.length;i++){
	if(aqiData[i][1]>60){
	arr.push(aqiData[i]);
	}
}
	for(var j=0;j<arr.length;j++){
		 var text ="第"+str.charAt(j)+"名"+"："+arr[j][0] + '，' + arr[j][1];
		var oli=document.createElement("li");
		oli.innerText=text;
		
	oul.appendChild(oli);
};
}
aa();
</script>
</body>
</html>
