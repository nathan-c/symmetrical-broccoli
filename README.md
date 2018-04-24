Basic example of using docker to host the grpc example for C# behind an NGINX load balancer.

To run:
```
cd csharp
dotnet build
dotnet publish
docker-compose build
docker-compose up --scale app=4 -d
dotnet run --project GreeterClient
```


Pulled together with grpc example from https://github.com/grpc/grpc and nginx config from https://www.nginx.com/blog/nginx-1-13-10-grpc/