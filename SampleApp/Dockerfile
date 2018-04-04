FROM registry.access.redhat.com/dotnet/dotnet-20-runtime-rhel7
ARG source
WORKDIR /app
EXPOSE 80
COPY ${source:-obj/Docker/publish} .
ENTRYPOINT ["dotnet", "SampleApp.dll"]