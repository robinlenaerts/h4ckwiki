# Kali Linux in Docker
## Introduction
Personally I love to use Kali Linux for its wide range of tools that are pre-installed.
Sometimes I find deploying a full OS in a VM a little too cumbersome and therefor worked on creating my own variant of Kali Linux in Docker.
The biggest advantage for me of having Kali Linux in Docker is to be able to use tools within seconds, especially when I want to test something quickly.

## Usage
My Docker image is based on the Official Kali Linux Rolling repository and includes some pre-installed tools/metapackages:
- OpenSSH Server running on port 22 (root:kali)
- Installed packages (kali-linux-headless, openssh-server, man-db, nano, iputils-ping, gobuster, seclists)

I provide daily builds of this image on [Docker Hub](https://hub.docker.com/r/robincraft007/kali-linux-ssh).

Run this container in Docker: 'docker run -d -p 50022:22 --name kali robincraft007/kali-linux-ssh:<arch>'

Connect over SSH to port 50022 of your Docker host with root:kali and enjoy the Kali Linux toolset!
