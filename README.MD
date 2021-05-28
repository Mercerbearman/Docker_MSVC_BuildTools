# Docker Command Line commands

## Build Docker image

```
docker build -t buildtools2019:latest -m 6GB .
```

## To run (And build the code)

```
docker run -v D:\Source\Docker_SPIDR\Docker_SPIDR:c:\Docker_SPIDR --name Docker_SPIDR buildtools2019 msbuild c:\Docker_SPIDR\SPIDR.sln /p:Configuration=Release /p:Platform=WIN32
```

## To Rebuild in container

```
docker start -a Docker_SPIDR
```
