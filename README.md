# Picamera Style Transfer

**Apply style transfer to picture taken from the Raspberry Pi camera (or usb camera, files).**

![](https://github.com/cmembrez/Raspberry-Robotics101/blob/master/images/utils/style_transfer.jpg)

**And create your own style transfer camera/box.**

![](https://github.com/cmembrez/Raspberry-Robotics101/blob/master/images/utils/examples-box.png)

* The code is based on https://github.com/pytorch/examples/tree/master/fast_neural_style


## Required : 

### Hardware    

* Raspberri Pi
* Pi camera (or usb camera)
* Intel Neural Compute Stick - NCS2 (optional but recommended)

### Software    

* Pytorch
* Torchvision
* Opencv
* Openvino (NCS2)

## Graphical User Interface

![](https://github.com/cmembrez/Raspberry-Robotics101/blob/master/images/utils/GUI.png)

## Adding a push button (Box) : 

Check the box to add a push button. Use pin 3.3v and n10. See image bellow :

<img src="https://raspberrypihq.com/wp-content/uploads/2018/02/02_Push-button_bb-min.jpg" alt="button" width="300"/>

## Limitation :

* Raspberry Pi with 1Go Ram (if the NCS2 box is not checked): do not use image superior to ~200x200px (use Downscale)
* Raspberry Pi with 4Go Ram (if the NCS2 box is not checked): do not use image superior to ~600x600px (use Downscale)
