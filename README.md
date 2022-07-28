## Usage

Please not you must have docker-ce and docker-compose already installed but if not see the bottom for the installation instructions.


Simply clone this repository and run:

```bash
git clone https://github.com/dustinwloring1988/docker-win10

docker-compose up -d
```


## What To Do Next


Try to Nmap the windows box using the following:
```bash
sudo nmap -Pn -p 3389 172.17.0.2
```

### or 

Install an RDP client of your choice for Linux. A popular one is RDesktop:

```bash
sudo apt-get install rdesktop
```

Finally, we can access the Windows VM:
```bash
sudo rdesktop 172.17.0.2
```


## Creds - For the Windows box

The Windows box that we have installed has two built-in accounts:

### Username: vagrant Password: vagrant

### Username: Administrator Password: vagrant

## Install Docker and Docker-Compose

```bash
sudo apt-get update

sudo apt-get install apt-transport-https ca-certificates curl gnupg-agent software-properties-common

curl -fSSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add

sudo apt-key fingerprint 0EBFCD88

sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

sudo apt update

sudo apt install docker-ce -y

sudo apt install docker-compose

sudo systemctl start docker

sudo systemctl enable docker
```
