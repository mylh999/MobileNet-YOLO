# MobileNet-YOLO Caffe

## MobileNet-YOLO 

A caffe implementation of MobileNet-YOLO detection network , first train on COCO trainval35k then fine-tune on 07+12 , test on VOC2007

Currently , I can not get good accuracy , but I will keep these models on the git.

## Windows Version

[Caffe-YOLOv3-Windows](https://github.com/eric612/Caffe-YOLOv2-Windows)

### Oringinal darknet-yolov3

[Converter](models/darknet_yolov3) 

test on coco_minival_lmdb (IOU 0.5)

Network|mAP|Resolution|Download|Netron|
:---:|:---:|:---:|:---:|:---:
yolov3|54.2|416|[caffemodel](https://drive.google.com/file/d/1nYgjOg8o48qQ3Cw47CamERgJVgLlo-Cu/view?usp=sharing)|[graph](http://lutzroeder.github.io/netron/?gist=59c75a50e5b91d6dd80a879df3cfaf55)
yolov3-spp|59.8|608|[caffemodel](https://drive.google.com/file/d/1eEFXWPFnCt6fWtmS6zTsPkAQgW0VFkt7/view?usp=sharing)|[graph](http://lutzroeder.github.io/netron/?gist=71edbfacf4d39c56f2d82cbcb739ae38)

* I haven't implement [correct_yolo_boxes](https://github.com/pjreddie/darknet/blob/master/src/yolo_layer.c) and relative function , so here only support square input resolution

## Other Models

You can find non-depthwise convolution network here , [Yolo-Model-Zoo](https://github.com/eric612/Yolo-Model-Zoo.git)

network|mAP|resolution|macc|param|
:---:|:---:|:---:|:---:|:---:|
PVA-YOLOv3|0.703|416|2.55G|4.72M|
Pelee-YOLOv3|0.703|416|4.25G|3.85M|

### Model visulization tool

Supported on [Netron](https://github.com/lutzroeder/netron) , [browser](https://lutzroeder.github.io/netron/) version

### Build , Run and Training

See [wiki](https://github.com/eric612/MobileNet-YOLO/wiki)


## License and Citation


Please cite MobileNet-YOLO in your publications if it helps your research:

    @article{MobileNet-YOLO,
      Author = {eric612,avisonic},
      Year = {2018}
    }
    
## Reference

> https://github.com/weiliu89/caffe/tree/ssd

> https://pjreddie.com/darknet/yolo/

> https://github.com/gklz1982/caffe-yolov2

> https://github.com/yonghenglh6/DepthwiseConvolution

> https://github.com/alexgkendall/caffe-segnet

> https://github.com/BVLC/caffe/pull/6384/commits/4d2400e7ae692b25f034f02ff8e8cd3621725f5c

> https://github.com/shicai/MobileNet-Caffe

> https://github.com/cjerry1243/MobilenetV2_tf_to_caffe
