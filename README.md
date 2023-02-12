# Home Media Server

LANG=:us:

### Prerequisites.
- A public domain name. Buy one at [https://www.namecheap.com/](https://www.namecheap.com/)
- Use one for free at [https://duckdns.org](https://duckdns.org)
- Docker: [https://docs.docker.com/get-started/](https://docs.docker.com/get-started/)
- Docker Compose: [https://github.com/docker/compose/releases](https://github.com/docker/compose/releases)
- Server platform: [Rocky Linux 8](https://rockylinux.org/download)

# Applications
## monitoring-apps
### [Scrutiny]()
WebUI for smartd S.M.A.R.T monitoring. Scrutiny is a Hard Drive Health Dashboard & Monitoring solution, merging manufacturer provided S.M.A.R.T metrics with real-world failure rates from Backblaze. \
DockerHub:  [linuxserver/scrutiny](https://hub.docker.com/r/linuxserver/scrutiny) \
GitHub: [AnalogJ/scrutiny](https://github.com/AnalogJ/scrutiny#docker)

### [Uptime-kuma](https://demo.uptime.kuma.pet:27000)
Uptime Kuma is an easy-to-use self-hosted monitoring tool. \
DockerHub: [louislam/uptime-kuma](https://hub.docker.com/r/louislam/uptime-kuma) \
GitHub: [louislam/uptime-kuma](https://github.com/AnalogJ/scrutiny#docker)

### [Speedtest](https://speedtest.henrywhitaker.com)
This program runs a speedtest check every hour and graphs the results. \
DockerHub: [henrywhitaker3/speedtest-tracker](https://hub.docker.com/r/henrywhitaker3/speedtest-tracker) \
GitHub: [henrywhitaker3/speedtest-tracker](https://github.com/henrywhitaker3/Speedtest-Tracker)

## Info
Because all the services are setup with `docker-compose` they can all reach each other by their Docker Compose service name. So for example when connecting Sonarr with Jacket or qBittorrent, then Jackett would be available on `http://jackett/api....`, which makes everything a lot easier.

### Edit the .env file
All configuration to this setup, I've put in the `.env` file, so all you have to do is go through it and edit it to fit your needs.
