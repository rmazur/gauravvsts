FROM registry.access.redhat.com/dotnet/dotnet-20-runtime-rhel7
ARG source
WORKDIR /opt/app-root/app
EXPOSE 80
ADD ${source:-obj/Docker/publish} .
CMD ["dotnet", "SampleApp.dll"]