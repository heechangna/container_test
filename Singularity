Bootstrap:docker  
From:ubuntu:latest  

%labels
MAINTAINER hna

%environment
RAWR_BASE=/code
export RAWR_BASE

%runscript
echo "This gets run when you run the image!" 
exec /bin/bash /code/rawr.sh "$@"  

%post  
echo "This section happens once after bootstrap to build the image."  
apt-get install vim  
