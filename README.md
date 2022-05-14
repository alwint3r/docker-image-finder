# Docker Image Finder

Get a list of all docker images along with the tags.

## Usage

```sh
# Assuming docker-image-finder is in your PATH

docker-image-finder IMAGE_NAME
```

### Example

#### Remove all images with name `ubuntu`

```sh
images=$(docker-image-finder ubuntu)

for img in $images;
do
    docker rmi $img
done
```

