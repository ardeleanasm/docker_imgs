## Create directories

```
mkdir r-docker
```

```
cd r-docker
```

## Build

```
docker build -t r-docker .
```


## Run



### Run interactively

```
docker run -ti r-docker
```
### Run in batch mode

```
docker run -ti --mount type=bind,source="$(pwd)",target=/home/docker/scripts r-docker /usr/bin/bash

```

```
docker run -ti --rm r-docker /usr/bin/bash
```


