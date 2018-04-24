FROM microsoft/dotnet

WORKDIR /app
COPY bin/Debug/netcoreapp2.0/publish .

ENTRYPOINT ["dotnet", "GreeterClient.dll"]