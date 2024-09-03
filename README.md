# yolov5
yolov5进行口罩识别

MaskDataSet数据集[下载地址官方](https://public.roboflow.com/)<br/>
[百度网盘下载地址](https://pan.baidu.com/s/1ldUAiOvTOL-U1gfdvfH86Q?pwd=y8qi)

用pycharm打开项目,找到train.py
![image](https://github.com/user-attachments/assets/4e78eac5-94cf-4d5a-99f3-fdcd1d562cc9)
在script里加上一下代码
![image](https://github.com/user-attachments/assets/b378bd51-ba4f-4a1a-b922-c05ce08fa90f)
```
--data
../MaskDataSet/data.yaml
--cfg
models/yolov5s.yaml
--weights
''
--batch-size
16
```
即可开始训练

测试，在detect.py
![image](https://github.com/user-attachments/assets/1697315b-2aee-4576-968e-5a450be1fd1b)
![image](https://github.com/user-attachments/assets/6272c086-e7dc-42b9-b3f0-e1890dfee13b)
```
--source
0
--weights
./weights/last.pt
--conf
0.4
```
