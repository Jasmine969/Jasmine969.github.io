# 矩形绘制与键盘的交互

1. 直接拖动鼠标，不按键盘：以拖动起点为矩形一角
2. <kbd>Shift</kbd> + 鼠标：以拖动起点为矩形==中心==
3. <kbd>Ctrl</kbd> + 鼠标：以拖动起点为矩形一角，保持一定比例绘制，比例依次为1:1、1:0.618、2:1、3:1、4:1……
4. <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + 鼠标：以拖动起点为矩形==中心==，保持一定比例绘制，比例同上

# 节点工具与圆角

<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/20220227221929.png?mode=framel" style="zoom:67%;" />
![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220227223149.png?mode=framer)
选中左边的节点工具，点到右边的举行对象上，会出现两个小方块（控制矩形大小)和一个圆圈，*其实圆圈是两个，只不过另一个被盖住了*。
向下拖动圆圈，另一个就露出来了，此时出现了圆角，是1/4圆。
再向左拖动曾被盖住的圆圈，此时圆角部分的1/4圆变成了1/4椭圆，可以看到水平部分开始出现更多的弯曲。
如果 <kbd>Ctrl</kbd> + 鼠标点击其中一个圆圈，1/4椭圆又会恢复为圆，圆的半径与被点的圆圈到右上角的距离相等；如果<kbd>Ctrl</kbd> + 鼠标拖动圆圈，则两个圆圈距离右上角的距离将一直保持相等，也就是圆角一直是1/4圆。
此时如果想让圆角矩形==恢复原状==，只要按住 <kbd>Shift</kbd> ，然后点击其中任意一个圆圈，就可以了。

# 缩放矩形时是否缩放圆角

##  横平竖直的矩形
<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/1645973296(1).png?mode=logol" style="zoom:67%;" />
![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220227224942.png?mode=logor)

灰色时，选中了缩放圆角；白色时，未选中缩放圆角

左图中放大了两个原本一模一样的矩形，蓝的缩放了圆角，红的未缩放圆角。可以看到，蓝的放大同时圆角半径也放大了。

## 倾斜的矩形

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220228121621.png?mode=figure)

先选择`节点工具`，然后拖动任意一个小方块缩放。可以看到，缩放前后，圆角重合。 


# 定量且批量改变圆角大小

![定量改变圆角](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220227225657.png)

1. 先框选住所有要修改的对象（框住星形也没关系）；
2. 选中左侧菜单的矩形；
3. 此时工具栏出现`Rx`和`Ry`，可进行批量修改，不会影响星形。
