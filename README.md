# dockerfile-om2m
Dockfile for building OM2M nscl/gscl images

## Usage  

### NSCL
```
docker run --rm -it -p 8080:8080 -v "$(pwd)/configuration":/NSCL/configuration iamgyz/om2m:nscl  
```

### GSCL
```
docker run --rm -it -p 8181:8181 -v "$(pwd)/configuration":/GSCL/configuration iamgyz/om2m:gscl  
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
