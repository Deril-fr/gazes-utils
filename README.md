# Gazes-utils

## Why this project ?
I always get bored writing the same commands over and over again when I'm working with Docker.
So I decided to create a script to automate the process. 
And make it easier to use Docker, especially for beginners.
## Installation

```bash
git clone https://github.com/deril-fr/gazes-utils && cd gazes-utils && ./setup.sh
```

## Commands

### Docker-run

#### Description
Start a new container with the specified image, container name and port in daemon mode.

#### Usage
```bash
docker-run <port> <container-name> <image-name>
```
#### Example
```bash
docker-run 8080 my-container my-image
```

### Docker-clean

#### Description
Stop and remove a Docker container.
Pull the latest image.
Start a new container with the updated image, using the same ports if specified and the same container name.
Check if the new and old images are the same.
If they are different, remove the old image.


[WARNING]: Use this only for an unique container and only with images from the same repository.

#### Usage
```bash
docker-clean <container-name> <image-name>
```
#### Example
```bash
docker-clean my-container my-image
```

## License  
[MIT](https://choosealicense.com/licenses/mit/)
