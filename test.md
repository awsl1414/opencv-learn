### cv2.findContours(img, mode, method)

mode:轮廓检索模式

- RETR_EXTERNAL：只检索最外面的轮廓
- RETRLIST：检索所有的轮廓，并将其保存到一条链表当中；
- RETRCCOMP：检索所有的轮廓，并将他们组织为两层：顶层是各部分的外部边界，第二层是空洞的边界
- RETRTREE：检索所有的轮廓，并重构嵌套轮廓的整个层次

method:轮廓逼近方法

- CHAINAPPROXNONE：以Freeman链码的方式输出轮廓，所有其他方法输出多边形（顶点的序列）。
- CHAINAPPROXSIMPLE：压缩水平的、垂直的和斜的部分，也就是，函数只保留他们的终点部分
