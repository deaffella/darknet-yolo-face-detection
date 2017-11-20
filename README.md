![Darknet Logo](http://pjreddie.com/media/files/darknet-black-small.png)

#Darknet#
Darknet is an open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.

For more information see the [Darknet project website](http://pjreddie.com/darknet).

For questions or issues please use the [Google Group](https://groups.google.com/forum/#!forum/darknet).


---------------------------------------

## What this fork do
This fork is to make darknet work with yolo-face weights.

## Follow these steps:
- download the source code and build

```sh
make
```
- download yolo-face cfg and [weights](https://git.mikael.io/ml/data/yolo2-face-detection/blob/fc04327de88111ee6a2ae618d0bdcd8d481db33f/yolo-face_final.weights) to source directory
- run demo which will open camera and show the face boxes

```sh
./darknet yolo demo yolo-face.cfg yolo-face_final.weights
```
- run test on image

```sh
./darknet yolo test yolo-face.cfg yolo-face_final.weights test.jpg
```

