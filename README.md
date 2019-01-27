# CamRecorder
Record Camera video through RTSP access

## Prequisites
First of all you have to install ffmpeg.

## Installation
yum install camrecorder-1.0.0-1.x86_64.rpm

## Man page
man camrecorder.conf

## Configuration
Each camera must be defined in a unique file finishing by .conf in the camrecorder.d folder. The file needs to contains the following options.

       rtsp_status
              Permit or not the recording of the camera.  Example : rtsp_status="off"
              Default : "on"

       rtsp_uri
              RTSP URI to access to the camera.  It includes URL : username,  password,  hostname,  port  number  and  the  URN.   Example  :
              rtsp_uri="rtsp://username:password@hostnameorip:portnumber/live/ch0"


       rtsp_maxsecondcreating
              The maximum time, in seconds, for each recording file.  Example : rtsp_maxsecondcreating="3600"



## Execution
systemctl start camrecorder.service
