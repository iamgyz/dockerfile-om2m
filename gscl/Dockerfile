# This is the Dockerfile for OM2M/NSCL version 0.8.0
# Author: GYZHNEG <gyzheng@cs.nctu.edu.tw>
# Build command: docker build -t gyzheng/om2m:nscl .

# Base image, Get java7
FROM develar/java

# Maintainer
MAINTAINER gyzheng <gyzheng@cs.nctu.edu.tw>

# Install OM2M
COPY ./GSCL /GSCL

# Define working directory.
WORKDIR /GSCL

# Define default command.
ENTRYPOINT ["sh"]
CMD ["start.sh"]
