# Picamera Style Transfer

**Apply style transfer to picture taken from the Raspberry Pi camera (or usb camera, files).**

<img src="images/utils/style_transfer.jpg" alt="" />

**And create your own style transfer camera/box.**

![](https://github.com/cmembrez/Raspberry-Robotics101/blob/master/images/utils/examples-box.png)

* The code is based on https://github.com/pytorch/examples/tree/master/fast_neural_style


## Required : 

### Hardware    

* Raspberri Pi 3/4
* Pi camera (or usb camera)
* Intel Neural Compute Stick - NCS2 (optional but recommended)

### Software    

* Pytorch
* Torchvision
* Opencv
* Openvino (NCS2)

## Graphical User Interface

* To test on PC :  
In neural_style directory:`python Picamera_st_gui_pc.py `

* On Raspberry Pi (work in progress, some problems with the display of windows) :  
In neural_style directory:`python Picamera_st_gui_pi.py `  

![](https://github.com/cmembrez/Raspberry-Robotics101/blob/master/images/utils/GUI.png)

* Device : select Picamera, USB Camera or File (and select input file)
* Style : select the style to use. Use only a style whose name begins with NCS if you checked the NCS2 box.
* Push button : check if you want to use a push button
* NCS2 : check if you want to use a Neural Compute Stick (NCS2)
* Downscale : use it to downscale the size of your image (if File device selected)

## Adding a push button (Box) : 

Check the box to add a push button. Use pin 3.3v and n10. See image bellow :

<img src="https://raspberrypihq.com/wp-content/uploads/2018/02/02_Push-button_bb-min.jpg" alt="button" width="300"/>

## Limitation :

* Raspberry Pi with 1Go Ram (if the NCS2 box is not checked): do not use an image larger than ~200x200px (use Downscale)
* Raspberry Pi with 4Go Ram (if the NCS2 box is not checked): do not use an image larger than ~600x600px (use Downscale)
