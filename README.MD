# Docker Command Line commands

## Build Docker image

```
docker build -t buildtools2019:latest -m 6GB .
```

## To run (And build the code)

```
docker run -v D:\Source\Docker_SOURCE\Docker_SOURCE:c:\Docker_SOURCE --name Docker_SOURCE buildtools2019 msbuild c:\Docker_SOURCE\Application.sln /p:Configuration=Release /p:Platform=WIN32
```

## To Rebuild in container

```
docker start -a Docker_SOURCE
```
