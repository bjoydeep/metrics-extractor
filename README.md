docker build -t metrics-extractor .


docker run -e OC_CLUSTER_URL=https://api.xyz.com:6443 -e OC_TOKEN=sha256~elK -v /tmp:/output metrics-extractor


#docker run -it metrics-extractor /bin/bash
