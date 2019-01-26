# CamRecorder
Record Camera video through RTSP access

## Prequisites
First of all you have to install ffmpeg.

## Installation
yum install camrecorder-1.0.0-1.x86_64.rpm

## Man page
man camrecorder.conf

## Configuration
Each camera must be defined in a unique file finishing by .conf in the camrecorder.d folder. The file needs to contains the six following options.

## Execution
systemctl start camrecorder.service
