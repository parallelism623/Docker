#Docker

Containers and Image, What and Why?

Build Image.

```docker
docker build <Options> .
```

Run Container.

```docker
docker run <ID_Image/Name:Tag_Image>
```

Stop and Restart Container.

```docker
//Stop
docker stop <ID_Containers/Name_Container>

//Re-Start
docker start <ID_Containers/Name_Container>
```

Attached and Detached.

```docker
-d : detached

-a : attached
```

Interactive.

```docker
//Run attached
-i: interactive
-t: TTY
docker run -it <ID_Image/Name:Tag_Image>
-a : attached
docker start -i <ID_Container/Name_Container>
```

Remove Containers, Images.

```docker
docker rm/rmi prune: delete all containers/images that is stopped.

docker rm <Specific containers, seperate by space> : delete specific containers
docker rmi <specific images> : delete sepecific images

docker run --rm <> : delete containers immediately after it exit.
```

Image Inspect.

```docker
 docker image: display list images in docker.
 docker image inspect <Images_Name>: display detail information for specific image by images name
```

Containers file copy.

```docker
docker container cp <Src_path> <Dest_path>
```

Name Containers and Tag Images.

```docker
docker run --name <Name_Container> <Images>: set the name for container when it has been created.
```
