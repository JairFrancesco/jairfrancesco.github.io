# jairfrancesco.github.io
Website for PeerLive

ffmpeg -threads 2 -re -fflags +genpts -stream_loop -1 -i SampleVideo_1280x720_50mb.mp4 -vcodec libx264 -preset veryfast -maxrate 3000k \
-bufsize 6000k -pix_fmt yuv420p -g 50 -c:a aac -b:a 160k -ac 2 -strict -2 -f flv "rtmp://104.36.18.76/live/jair" 
