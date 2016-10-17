# .NET Core on Apprenda

FROM microsoft/dotnet:core
COPY bin/Debug/netcoreapp1.0/publish/. /app
WORKDIR /app

EXPOSE 8085/tcp
ENV ASPNETCORE_URLS http://*:8085

ENTRYPOINT dotnet /app/netcoremvc.dll