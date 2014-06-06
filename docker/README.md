This runs mjpg-streamer in a container.

To run:
    `docker run -d -v /mnt/webcam:/data -p 8080:8080 chuckleb/mjpg-streamer`
    
*-v* is where the files are stored mapped to /data inside the container  
*-p* maps a public port (8080) to port 8080 inside the container

The script that it runs expects a file named webcam.jpg in the /data folder inside the container. These images can be captured in whatever software you want, fswebcam is a good package. 

You will then be able to view the stream via: `http://ipaddress:8080`
    
