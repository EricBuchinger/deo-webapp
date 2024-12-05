FROM mcr.microsoft.com/dotnet/sdk:8.0-alpine3.20 AS build
WORKDIR /build
COPY . .
RUN dotnet publish -o /app/publish/

FROM mcr.microsoft.com/dotnet/aspnet:8.0-alpine3.20 AS final
WORKDIR /app
COPY --from=build /app/publish .

ENV DOTNET_HTTP_PORTS=80
#ENV ASPNETCORE_URLS=http://*:3000

ENTRYPOINT ["/app/Deo.Backend"]
EXPOSE 80/tcp

