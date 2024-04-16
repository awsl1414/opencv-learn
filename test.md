# 图像阈值

## ret, dst= cv2.threshold(src thresh, maxval, type)

- src: 输入图， 只能输入单通道图像 通常来说为灰度图
- dst：输出图I
- thresh: 國值
- maxval: 当像素值超过了阅值 （或者小于阈值 根据type来决定） 所赋予的值
- type: 二值化操作的类型， 包含以下5种类型：cv2.THRESH_BINARY; cv2.THRESH_BINARY_INV; cv2.THRESH_TRUNC; cv2.THRESH_TOZERO; CV2.THRESH TOZERO_INV
- cv2.THRESH_BINARY 超过阅值部分取maxval （最大值）： 否则取0
- cv2.THRESH_BINARY_INV THRESH BINARY的反转
- cv2.THRESH_TRUNC 大于间值部分设为间值 否则不变
- cv2.THRESH_TOZERO 大于阅值部分不改变 否则设为0
- cv2.THRESH_H_TOZERO_INV THRESH TOZERO的反转
