# docker-scuttlebot
Run an ssb-server (scuttlebot server) in a Docker container

To run a Pub you need to have a static public IP, ideally with a DNS record (i.e.`<hostname.yourdomain.tld>`)

This fork of ktorn/docker-scuttlebot adds a docker-compose file for easier deployment.

## Build from source

#### 1. Clone this repo

From GitHub:
`git clone https://github.com/alexpaths/docker-scuttlebot.git`

#### 2. Build the container

```sh
cd docker-scuttlebot
docker build -t scuttlebot .
```

## Run the container

#### 1. Create a directory on the docker host for persisting the scuttlebot server's data
```sh
mkdir ~/sbot-data
```

#### 2. Run the container
```sh
docker-compose up -d
```
