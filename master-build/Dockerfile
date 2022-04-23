FROM node:16.14.2

RUN apt-get update; \
   apt-get install -y wget

# install dotnet sdk
RUN wget https://packages.microsoft.com/config/debian/11/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
RUN dpkg -i packages-microsoft-prod.deb
RUN rm packages-microsoft-prod.deb

RUN apt-get update; \
   apt-get install -y apt-transport-https && \
   apt-get update && \
   apt-get install -y dotnet-sdk-6.0

RUN apt-get update; \
   apt-get install -y apt-transport-https && \
   apt-get update && \
   apt-get install -y aspnetcore-runtime-6.0

RUN apt-get install -y dotnet-runtime-6.0
