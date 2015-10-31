# dockerfile-om2m
Dockfile for building OM2M nscl/gscl images

## Usage  

### NSCL
```
docker run -it -p 8080:8080 gyzheng/om2m:nscl  
```

### GSCL
```
docker run -it -p 8181:8181 gyzheng/om2m:gscl  
```


## How to build?  
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
