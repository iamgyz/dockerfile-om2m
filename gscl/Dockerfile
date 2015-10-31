# This is the Dockerfile for OM2M/NSCL version 0.8.0
# Author: GYZHNEG <gyzheng@cs.nctu.edu.tw>
# Build command: docker build -t gyzheng/om2m:nscl .

# Base image, Get java7
FROM develar/java

# Maintainer
MAINTAINER gyzheng <gyzheng@cs.nctu.edu.tw>

# Install OM2M
RUN wget http://ftp.yzu.edu.tw/eclipse/om2m/releases/0.8.0/OM2M-0.8.0.zip\
   && unzip OM2M-0.8.0.zip\
   && rm OM2M-0.8.0.zip\
   && rm -rf /OM2M-0.8.0/NSCL

# Define working directory.
WORKDIR /OM2M-0.8.0/GSCL

# Define default command.
CMD ["sh","start.sh"]
