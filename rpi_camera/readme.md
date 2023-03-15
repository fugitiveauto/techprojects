rpi_camera
Connect the raspberry pi to the pi camera, and display on a screen automatically at boot

View Pi Cam
raspivid -o - -t 0 -hf -w 640 -h 360 -fps 25 | cvlc -vvv stream:///dev/stdin --sout '#rtp{sdp=rtsp://:8554}' :demux=h264

Start camera
cvlc -f  rtsp://192.168.0.101:8554/

