# docker-r-r

Docker container to store and ship Reproducible Research documents e.g. R markdown

### Build this image

`docker build -t vladdsm/docker-r-r .`

### Run the container

`docker run -it --rm -v [LOCAL_FOLDER]:/03_output vladdsm/docker-r-r`

### Details

Dockerfile will copy R markdown document to the container image. When container will run document output will be rendered and placed into the folder 03_output. Thanks to the `-v` key this folder will be synchronized to our local folder