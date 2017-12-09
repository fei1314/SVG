1)svg样式的两种写法<br>
1.属性形式<br>
2.style形式------推荐<br>

样式优先级：属性<*<标签<class<id<行内<important<br>


2)SVG图形<br>
1.样式操作---------跟HTML一样(推荐用style)<br>
2.事件操作---------跟HTML一样(完全一样)<br>
3.属性操作---------有点区别(set/get)<br>

  HTML<br>
设置:<br>
    .xxx=xxx<br>
    .setAttribute<br>
获取:<br>
    .xxx<br>
    .getAttribute<br>

SVG<br>
设置:<br>
    .setAttribute<br>
获取:<br>
    .getAttribute<br>

3)DOM操作<br>
获取：和HTML一样<br>
创建：SVG：createElementNS('http://www.w3.org/2000/svg')<br>


事件、修改、大部分操作跟HTML一样<br>
不同：attribute、createElementNS('网址', 标签)<br>


4)图形<br>
1.rect 矩形 x,y,width,height,rx,ry<br>
  x:起点坐标<br>
  y:终点坐标<br>
  width:矩形的宽度<br>
  height:矩形高度<br>
  rx:x方向上的圆角<br>
  ry:y方向上的圆角<br>

2.circle  正圆 cx,cy,r<br>
  cx:圆心坐标x<br>
  cy:圆心坐标y<br>
  r:圆的半径<br>
3.ellipse 椭圆 cx,cy,rx,ry<br>
  cx:圆心坐标x<br>
  cy:圆心坐标y<br>
  rx:长半轴<br>
  ry:短半轴<br>
4.line 直线 x1,y1,x2,y2(起点坐标，终点坐标)<br>
5.path  M/L/Z/A<br>

  M x,y  起点坐标<br>
  L x,y  直线的终点坐标(可以是多个)<br>
  Z 关闭路径<br>
  A rx      ry      x-axis-rotation large-arc-flag sweep-flag   x y<br>
    x半径   y半径     x轴旋转的角度       大弧标志       镜像标志   终点坐标<br>


注意：如果没有背景色(fill:none)，会导致背景没有事件——用透明<br>
