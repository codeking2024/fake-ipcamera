# fake-ipcamera
This is guide to make rtsp stream from webcamera

### Setup the environment for ffmpeg.

### How to check camera devices on PC

`ffmpeg -list_devices true -f dshow -i dummy`

### Run mediamtx.exe and run the following command.

`ffmpeg -f dshow -i video="Integrated Camera" -f rtsp rtsp://localhost:8554/live`

### Open the stream using vls (Media/Open Network Stream)

`rtsp://localhost:8554/live`
