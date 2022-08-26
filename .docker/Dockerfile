#https://hub.docker.com/_/microsoft-dotnet-sdk/
FROM mcr.microsoft.com/dotnet/sdk:6.0-bullseye-slim

# user for vscode
RUN useradd -s /bin/bash -m vscode
# add user vscode to groupadd
RUN groupadd docker && usermod -aG docker vscode

# set vscode as user
USER vscode

# keep the container alive until someone shuts it down
ENTRYPOINT ["sleep", "infinity"]