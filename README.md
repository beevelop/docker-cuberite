![GitHub Workflow Status](https://img.shields.io/github/workflow/status/beevelop/docker-cuberite/Docker%20Image?style=for-the-badge)
![Docker Pulls](https://img.shields.io/docker/pulls/beevelop/cuberite.svg?style=for-the-badge)
![Docker Stars](https://img.shields.io/docker/stars/beevelop/cuberite?style=for-the-badge)
![Docker Image Size (tag)](https://img.shields.io/docker/image-size/beevelop/cuberite/latest?style=for-the-badge)
![License](https://img.shields.io/github/license/beevelop/docker-cuberite?style=for-the-badge)
[![GitHub release](https://img.shields.io/github/release/beevelop/docker-cuberite.svg?style=for-the-badge)](https://github.com/beevelop/docker-cuberite/releases)
![GitHub Release Date](https://img.shields.io/github/release-date/beevelop/docker-cuberite?style=for-the-badge)
![CalVer](https://img.shields.io/badge/CalVer-YYYY.MM.MICRO-22bfda.svg?style=for-the-badge)
[![Beevelop](https://img.shields.io/badge/-%20Made%20with%20%F0%9F%8D%AF%20by%20%F0%9F%90%9Dvelop-blue.svg?style=for-the-badge)](https://beevelop.com)

# [Cuberite](https://cuberite.org/) for whale lovers

> Cuberite is a Free and Open Source (FOSS) Minecraft-compatible game server. Cuberite is designed with performance, configurability, and extensibility in mind, and also aims to accurately recreate most Minecraft features.

## Quickstart
```bash
docker run --tty -d --name="cuberite" -p 8080:8080 -p 25565:25565 beevelop/cuberite
```

The server should be accessible via Port `25565`. There is a webadmin interface available at `8080` (default login `admin` and password `Swordfish`).

## Configuration
- `ADMIN_USERNAME` (default: `admin`): The username for the webadmin interface
- `ADMIN_PASSWORD` (default: `Swordfish`): The password for the webadmin interface
- `MAX_PLAYERS` (default: `30`): Max. amount of players

Both values can be changed and will be written to the `webadmin.ini` file on launch (this does effectively override the `webadmin.ini` on every start).

## Folders of interest
All necessary file are located at `/opt/cuberite`. 

## Troubleshooting
Feel free to open an issue on GitHub if you encounter any problems with this Docker image.

---

### Use tags where possible, because...

![One does not simply use latest](https://i.imgflip.com/1fgwxr.jpg)