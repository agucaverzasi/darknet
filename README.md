![Darknet Logo](http://pjreddie.com/media/files/darknet-black-small.png)

#Darknet#
Darknet is an open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.

For more information see the [Darknet project website](http://pjreddie.com/darknet).

For questions or issues please use the [Google Group](https://groups.google.com/forum/#!forum/darknet).


# To build darknet
```bash
make -j8
```

#Run YOLO on VOC dataset
```bash
wget http://pjreddie.com/media/files/yolo.weights
./darknet yolo test cfg/yolo.cfg ../yolo.weights data/person.jpg
```
#Run YOLO on COCO dataset
```bash
wget http://pjreddie.com/media/files/yolo-coco.weights
 ./darknet coco test cfg/yolo-coco.cfg ../yolo-coco.weights data/person.jpg
```