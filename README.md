# DockerSetup
Docker Setup for python scripting. Simple live coding and debugging python app inside container sharing the code directory.
## Installing
1. Copy files from the current repo.
2. Build the image. Replace name_image with the name of the image.Don't forget the dot at end of line.
```bash
docker build -t=name_image .
```
3. Run the container , open a bash into the container and share the code directory between host and container.
Replace the path to the code directory , name_image and name_container.
```bash
docker run --name=name_container -it -v /path/to/code:/app  name_image /bin/bash
```

