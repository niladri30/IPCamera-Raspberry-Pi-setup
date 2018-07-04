# IP-Camera-Raspberry-Pi-setup
Connect n-number of IP cameras to raspberry pi setup using RTSP (real time streaming protocol)
Raspberry Pi with USB cameras is an easy setup !

For details about RTSP, please check https://en.wikipedia.org/wiki/Real_Time_Streaming_Protocol

But problem is with the number of cameras which can be connected (I have connected maximum 4 cameras) and can stream any video. To have a fully functional wireless setup, we need IP cameras to stream video or click any images.

For various applications I have used RPi3 as a processing unit, like facial recognition, object detection and other setups which includes deep learning technologies. I have listed down the setup which is installed in RPi3.
1. OpenCV3
2. Facial Recognition
3. Dlib
4. TensorFlow
5. Upgraded Node-Red and Node.js
6. Python 3
7. VLC player

There are multiple IP cameras in market. I have chosen a cheap but powerfull IP camera from Amazon (https://www.amazon.in/D3D-Wireless-Indoor-Security-Support/dp/B01LY2TN7G).

Setup:
--------
1. The camera setup is very easy and within minutes its online. It comes with a video tutorial about the setup(https://www.youtube.com/watch?v=mdefgUis6aA).
2. Once you are able to get the IP of the camera, log in using Username and Password for accessing the camera console.
3. In IP-camera > open settings tab > open Network -- check the RTSP port (default: 554)

Code-setup:
------------
1. We need the rtsp url to configure the python code. To form the rtsp url you have to consider:

    a. Username and password for IP-camera console
    b. rtsp port
    c. Channel (I have taken 1)
    
  Output url:  
  rtsp://username:password@192.xxx.xx.xx:554/1

2. Sample python code provided to stream the video from IP cameras.
3. We can have multiple scripts to connect with different IP cameras for different use-cases.

Note: Raspberry Pi and IP-camera should be connecetd on same Wi-Fi network.

