### To build the docker image
docker build -t metrics-extractor .

### To use the docker image in quay.io
docker run -e OC_CLUSTER_URL=https://api.xyz.com:6443 -e OC_TOKEN=sha256~elK -v /tmp:/output quay.io/bjoydeep/metrics-extractor:latest

### To get into the image and debug
docker run -it metrics-extractor /bin/bash
