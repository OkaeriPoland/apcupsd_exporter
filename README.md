# apcupsd_exporter

![License](https://img.shields.io/github/license/OkaeriPoland/apcupsd_exporter)
![Total lines](https://img.shields.io/tokei/lines/github/OkaeriPoland/apcupsd_exporter)
![Repo size](https://img.shields.io/github/repo-size/OkaeriPoland/apcupsd_exporter)
![Contributors](https://img.shields.io/github/contributors/OkaeriPoland/apcupsd_exporter)
[![Discord](https://img.shields.io/discord/589089838200913930)](https://discord.gg/hASN5eX)

Command `apcupsd_exporter` provides a Prometheus exporter for the
[apcupsd](http://www.apcupsd.org/) Network Information Server (NIS). MIT
Licensed.

## Usage

Available flags for `apcupsd_exporter` include:

```console
$ ./apcupsd_exporter -h
Usage of ./apcupsd_exporter:
  -apcupsd.addr string
        address of apcupsd Network Information Server (NIS) (default ":3551")
  -apcupsd.network string
        network of apcupsd Network Information Server (NIS): typically "tcp", "tcp4", or "tcp6" (default "tcp")
  -telemetry.addr string
        address for apcupsd exporter (default ":9162")
  -telemetry.path string
        URL path for surfacing collected metrics (default "/metrics")
```

### Docker

```console
docker run --name=apcupsd_exporter --network=host okaeri/apcupsd_exporter
```
