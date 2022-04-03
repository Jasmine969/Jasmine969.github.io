# 椭圆创建

和矩形类似，有三种

- 直接鼠标拖动
- <kbd>Shift</kbd> + 鼠标拖动：以起点为中心绘制
- <kbd>Ctrl</kbd> + 鼠标拖动：按比例绘制，1:1 1:0618 2:1 3:1 4:1 ……

# 节点工具

也有两个小方块和两个原本重叠的圆圈

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220302102431.png?mode=logol)
![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220302102848.png?mode=logor)

当拖动圆圈并且光标位于椭圆外部时，形成饼状（下面是无填充）

当拖动圆圈并且光标位于椭圆内部时，形成弓形，未填充时显示为未闭合的弧线。

如果想让饼形或弓形恢复为完整的椭圆，只需要按住 <kbd>Shift</kbd> 然后点击任意一个圆圈。



<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/20220302105256.png?mode=logor" style="zoom:67%;" />
当按住<kbd>Ctrl</kbd> 拖动圆圈的时候，每次变化15度，右图从15度变化了5次变化到90度

---



也可以改变每次变化的角度
![改变旋转捕捉周期](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220302105534.png)

通过`#编辑|首选项#(magenta)`中的`#行为|步进#(lime)`中的`旋转捕捉周期`来设置
