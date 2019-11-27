# CaptureFace
Face cupture based on cv2,py,dlib
## 可以看做是升级版的CaptureFrame！
在视频帧抽取的基础上又调用了dlib库的人脸识别功能
## 使用方法
类似于之前的CaptureFrame，更改成自己的资源地址。
## 注意
```python
img1=frame[face.top()-50:face.bottom()+50,face.left()-50:face.right()+50]
```
这一行我解释一下：
如果不进行加减操作的话，生成的图像局限于人物的脸，甚至耳朵都没在画面里，这样对训练不利。
所以我微调了取景框的大小，使之不至于太小又不至于太大，生成的脸部有利于训练DFD系统！
