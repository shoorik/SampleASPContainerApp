# SampleASPContainerApp

This is a simple MVC ASP app which is used to demonstrate containers. To see the solution with dockerfile, select the 'completed' branch.

## To build image from Docker

```
docker build --tag shoorik/getting-started-aspnetcore:0.0.1 .
```

## To run new container from image (on port 5000)

```
docker run --detach --publish 5000:80 --name getting-started-movies shoorik/getting-started-aspnetcore:0.0.1
```

## To publish image to repository

```
docker login
docker push shoorik/getting-started-aspnetcore:0.0.1
```