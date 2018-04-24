FROM microsoft/dotnet

WORKDIR /app
COPY bin/Debug/netcoreapp2.0/publish .

EXPOSE 50051

ENTRYPOINT ["dotnet", "GreeterServer.dll"]