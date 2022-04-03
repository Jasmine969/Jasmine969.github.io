现有两个形状一样的“S”，把他们重叠在一起后，对绿色的进行路径偏移。

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220314101629.png)

# 向外偏移与向内偏移

用 <kbd>Ctrl</kbd> + <kbd>)</kbd> 进行向外偏移，看到绿色的向外扩张了

![向外偏移](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220314101807.png)

用 <kbd>Ctrl</kbd> + <kbd>(</kbd> 进行向内偏移，绿色又会向内收缩

---

# 动态偏移

还可以 <kbd>Ctrl</kbd> + <kbd>J</kbd> 动态偏移，此时“S”上出现一个红色节点，拖动这个节点可以进行偏移

![动态偏移](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220314102228.png)

# 链接偏移

这边用链接偏移（<kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>J</kbd> ）生成了一个新的“S”，然后把S往左挪。

可以看到此时链接偏移与动态偏移效果差不多，也是有一个节点可以拖动

![链接偏移1](https://gitee.com/feng-xiaomo/fengimages/raw/master/1647224998(1).jpg)

---

> <img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/20220314105103.png?mode=logol" alt="对原路径剪切变换" style="zoom:80%;" />

> <img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/20220314105638.png?mode=logor" alt="对原路径改变节点" style="zoom:80%;" />

所不同的是对原路径（蓝色的)进行变换后，链接的路径也会随之改变，这就是==链接==的作用

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220314120127.png)

对比一下可以发现，链接出的路径只有一个控制点，而原路径有很多控制点

![链接对象缩放、剪切、旋转后，改变原路径](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220314120403.png)

即使在缩放、剪切、旋转链接对象后，改变原路径，链接对象依然能随之改变

如果要让二者脱离链接关系，只需把链接偏移的对象转为路径

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220314120644.png)