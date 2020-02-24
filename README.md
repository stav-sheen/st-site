# web-site
a simple dockerfile to present an nginx site
General Info
-------------
The app was built using:
- docker
- Nginx
- AWS free tier


 installation
=============

**prerequisites**:
- docker (if not included with the kubernetes distro already)
- TCP ports 8089/80 open for network browser access

**RUN **
1. clone this branch :

`git clone https://github.com/stav-sheen/st-site.git`

2. build docker image:

 `docker build -t <image_name> .`
3. run the container:

 `docker container run -dit -v /tmp/st-site:/data/site -p 8089:80 <image_name>`
