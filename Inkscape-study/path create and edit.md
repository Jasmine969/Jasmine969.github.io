`#侧边栏|钢笔工具：贝塞尔曲线/直线#(green)`

# 曲线的创建

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220306110905.png?mode=logol)
![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220306111520.png?mode=logor)
按住 <kbd>Ctrl</kbd> 可以拖出15度倍数倾角的直线

按住鼠标左键不动，则生成贝塞尔曲线

如果点出第二个点后松开鼠标，则生成折线

注意：当控制点与途径点重合，则曲线变为直线






![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220306111827.png)

曲线的颜色可以Shift+单击颜色条设置，线宽可以在描边旁快捷选择

<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/1646539276(1).png?mode=logol" style="zoom: 67%;" />
控制点与途径点的确定是交替的

如果鼠标按住状态，则下一个待确定点是控制点；

如果鼠标是松开状态，则下一个待确定点是途径点。

<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/1646540850(1).png" style="zoom:50%;" />
让控制点连线变陡，则曲线曲率增大；拖动控制点远离途径点，则弯曲范围变宽

如果在确定途径点后立刻松开鼠标，则这个途径点形成一个角的顶点（折线）

<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/1646541710(1).png?mode=logol" style="zoom:67%;" />
<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/20220306125040.png?mode=logor" style="zoom:67%;" />
通过这两个小工具可以使节点在尖角节点和平滑节点之间转换

---











# 节点的添加与删除

<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/412cbad7e6c47b6cde76bac8364c4a6.jpg?mode=logol" style="zoom: 35%;" />
<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/b1cd2d63426c74f24317f73f965880a.jpg?mode=logor" style="zoom: 35%;" />

想在原有曲线上某处==增加==一个节点：选中节点工具，在添加处双击鼠标左键即可（或<kbd>Ctrl</kbd> + <kbd>Alt</kbd> + 鼠标左键单击）

而如果要==删除==节点，则节点工具选中节点，然后 <kbd>Del</kbd> ，或 <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + 鼠标左键单击）















# 曲线的断开与接合

==断开==曲线：先在断开处添加一个节点（如果原来就有节点就不用新添加了），然后 <kbd>Shift</kbd> +<kbd>B</kbd> ，就可以断开了，`B`应该是`break`的意思

==接合==曲线：<kbd>Shift</kbd> 选中两个端节点，然后 <kbd>Shift</kbd> + <kbd>J</kbd> ，就可以接合了，`J`应该是`join` 的意思

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220307105826.png)

# 控制手柄直线与折线的转换

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220307112017.png)
首先可以看到{平滑点}和{端点、尖角节点}的节点形状是不一样的，前者是横平竖直的正方形，后者是45度摆放的正方形


---

> ###### 控制手柄的直线改成折线
>
> 选中节点，<kbd>Shift</kbd> + <kbd>C</kbd> 
>
> 使用这个工具可以将平滑点改成尖角顶点，也就是把控制手柄的直线改成折线
>
> 
>
> ![](https://gitee.com/feng-xiaomo/fengimages/raw/master/1646629925(1).png)
>
> 
>
> `>(red!)`

> ###### 控制手柄的折线改成直线
>
> 如果要从尖角顶点改回平滑顶点，也就是把控制手柄的折线改成直线
> 选中节点，<kbd>Shift</kbd> + <kbd>S</kbd>
>
> 
>
> ![](https://gitee.com/feng-xiaomo/fengimages/raw/master/1646629771(1).png)
>
> `>(cyan!)`

# 控制手柄的取消与复原
---

> 取消一侧手柄
> <kbd>Ctrl</kbd> + 鼠标单击一侧的节点
> ![](https://gitee.com/feng-xiaomo/fengimages/raw/master/1646630554(1).png)
>
> `>(red!)`

> 复原一侧手柄
> <kbd>Shift</kbd> + 从一侧拖出节点
>
> ![](https://gitee.com/feng-xiaomo/fengimages/raw/master/1646630802(1).png)
>
> `>(cyan!)`
