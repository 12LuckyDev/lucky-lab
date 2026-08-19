# lucky-lab

Docker Compose setup for services running on a Raspberry Pi.

The project uses a single root compose.yaml which combines multiple independent Compose files using include.

## Structure

```text
lucky-lab/
├── compose.yaml
├── data/
├── dozzle/
│ └── compose.yaml
├── photoprism/
│ └── compose.yaml
├── nginx/
│ └── compose.yaml
└── lucky-radio/
├── lucky-mpd/
│ └── compose.yaml
├── lucky-radio-web/
│ └── compose.yaml
└── lucky-radio-api/
└── compose.yaml
```

## Services

- [Nginx](https://hub.docker.com/_/nginx)
- [Dozzle](https://hub.docker.com/r/amir20/dozzle)
- [MariaDB](https://hub.docker.com/_/mariadb)
- [PhotoPrism](https://hub.docker.com/r/photoprism/photoprism)
- lucky-radio:
  - [lucky-mpd](https://github.com/12LuckyDev/lucky-mpd)
  - [lucky-radio-api](https://github.com/12LuckyDev/lucky-radio-api)
  - [lucky-radio-web](https://github.com/12LuckyDev/lucky-radio-web)
