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