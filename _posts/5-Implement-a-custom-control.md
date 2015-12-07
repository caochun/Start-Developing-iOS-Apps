title: 五. 实现自定义控件
date: 2015-12-04 11:58:40
tags:
---

### 创建自定义视图

点击File > New > File ，选择ios下的source选项，选择Cocoa Touch Class，点击next，Class设置为RatingControl，“Subclass of”选择UIView,Language选择Swift

![](/images/5-1.png)

在RatingControl.swift代码区的class里添加代码

```
required init?(coder aDecoder: NSCoder) {
    super.init(coder: aDecoder)
}
```

### 显示自定义视图

从Object library中拖拽一个View,将其放置在image view下面，打开它的Size inspector，Intrinsic Size标签设置为Placeholder，宽和高分别设置为44和240,打开它的 Identity inspector，class标签选择RatingControl.

### 向视图添加button按钮
