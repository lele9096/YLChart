# YLChart
YLChart  主要是用来绘制环状图表
===
包含内容:<br> 
>>>>>* 1 渐变色圆环进度条<br>
>>>>>* 2 绘制多色环状图.按顺序绘制。从0 ~ 1.<br>
>>>>>* 3 绘制多色环状图.多段同时绘制<br>
>>>>>* 4 渐变色弧形绘制<br>
>>>>>* 5 折线图，填充色渐变色填充<br>
>>>>>* 6 绘制间隔弧度的多色圆环<br>
<br>
<br>
<br>

效果图
##

渐变色圆环进度条 <br>
-----
 ![](https://github.com/lele9096/YLChart/raw/master/imageSource/demoImg_1.png)
 <br>
绘制多色环状图.按顺序绘制。 <br>
-----
<br>
使用方法:<br>
/**
* @parame dataValue  数据源
* @parame colors  线段颜色
* @parame duration  绘制动画时长
* @parame startAngle  开始绘制角度，直接传度数.eg:50
* @parame radius  绘制半径
* @parame lineWidth  绘制线宽
* @parame cyclicChartType  绘制类型:YLCyclicChartType_sequence 按顺序绘制 YLCyclicChartType_while  多线段同时绘制
*/

NSArray* dataValue = @[@0.25,@0.25,@0.5];
NSArray* colors = @[[UIColor redColor],[UIColor yellowColor],[UIColor blueColor]];
YLCyclicChart* cyclicChart = [[YLCyclicChart alloc] initWithFrame:CGRectMake(0, 100, kScreenWidth, kScreenWidth) dataValue:dataValue colors:colors duration:3.0 startAngle:-90 radius:80 lineWidth:3.0 cyclicChartType:YLCyclicChartType_while];
[self.view addSubview:cyclicChart];

<br>
![](https://github.com/lele9096/YLChart/raw/master/imageSource/demoImg_2.png)
<br>
绘制多色环状图.多段同时绘制 <br>
-----
![](https://github.com/lele9096/YLChart/raw/master/imageSource/demoImg_3.png)
<br>
渐变色弧形绘制 <br>
-----
![](https://github.com/lele9096/YLChart/raw/master/imageSource/demoImg_4.png)
<br>
折线图，填充色渐变色填充 <br>
-----
![](https://github.com/lele9096/YLChart/raw/master/imageSource/demoImg_5.png)
<br>
绘制间隔弧度的多色圆环 <br>
-----
![](https://github.com/lele9096/YLChart/raw/master/imageSource/demoImg_6.png)
<br>
<br>
<br>




[个人博客](http://blog.csdn.net/lele9096_bk )


