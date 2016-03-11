# dockerfile-om2m
Dockfile for building OM2M v0.8 nscl/gscl images  

https://hub.docker.com/r/iamgyz/om2m 

## Usage  

### 1. Using default configuration  
If you just want to run from default configuration files in `NSCL(GSCL)/configuration`  

#### NSCL  
```
docker run --rm -it -p 8080:8080 iamgyz/om2m:nscl  
```
#### GSCL  
```
docker run --rm -it -p 8181:8181 iamgyz/om2m:gscl  
```


### 2. Using custom configuration  
Put your configuration directory in current path  
#### NSCL  
```
docker run --rm -it -p 8080:8080 -v "$(pwd)/configuration":/NSCL/configuration iamgyz/om2m:nscl  
```

#### GSCL  
```
docker run --rm -it -p 8181:8181 -v "$(pwd)/configuration":/GSCL/configuration iamgyz/om2m:gscl  
```







## How to re-build docker image from docker-file    
### NSCL  
```
cd nscl/  
./build_nscl.sh
```

### GSCL
```
cd gscl/  
./build.gscl.sh
```  
