# Setup

## Prerequisites

- Docker: [download Docker for Desktop from docker.com](https://www.docker.com/products/docker-desktop/).
  - If running on M1/M2 Mac enable the “Use Rosetta for x86/amd64 emulation on Apple Silicon” in the "Features in development" of Docker settings ([blog post by Randolph](https://www.docker.com/products/docker-desktop/))
- Pull the latest Microsoft SQL Server 2022 image for docker: docker pull mcr.microsoft.com/mssql/server:2022-latest

- Download the StackOverflow database: [hosted by Brent Ozar](https://www.brentozar.com/archive/2015/10/how-to-download-the-stack-overflow-database-via-bittorrent/)

  - Unpack the `7z` archive and copy `mdf` and `ldf` files into a directory that can be mounted into a container by Docker

- Adjust the path to the SQL Server data directory mount in `compose.yml`
