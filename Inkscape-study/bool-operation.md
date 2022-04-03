![这六个就是布尔运算了](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220310102925.png)

# 并集

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/1646879517(1).jpg)

<kbd>Ctrl</kbd> + <kbd>+</kbd> 求并集，新对象的填充和描边以底层图形为准

# 差集

<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/1646880026(1).png" style="zoom:80%;" />

<kbd>Ctrl</kbd> + <kbd>-</kbd> 求差集，运算对象应该是两个，用底层的减去顶层的

# 交集

<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/1646880707(1).png" style="zoom:80%;" />

<kbd>Ctrl</kbd> + <kbd>*</kbd> 求差集，用底层的样式作为结果样式

# 互斥

<img src="https://gitee.com/feng-xiaomo/fengimages/raw/master/20220312094247.png" style="zoom: 67%;" />

还是上面三张图，做了互斥运算后，去除了重叠的部分，留下来的样式是最底层的

# 分割

![分割](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220312095354.png)
<kbd>Ctrl</kbd> + <kbd>/</kbd> ，用底层的样式作为结果样式。可以看到底层对象上层的对象被分割成了不同的小块，可以拖动使之分离。

默认情况下小块之间会==自动吸附==，按住<kbd>Shift</kbd> 再拖动可以取消吸附

# 剪切

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/6c1e7325b86d76eed71b6ba33e6aaba.png)

纯粹的切开路径，没有任何新增的路径，两个切开的路径相加后就是原路径
