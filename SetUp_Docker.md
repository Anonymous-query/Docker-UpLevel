# Commands to Install Docker on Linux Machine

Please execute all commands in the sequence they are given.

```
sudo apt-get update
```
```
sudo apt-get install \apt-transport-https \ca-certificates \curl \software-properties-common 
```
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add 
```
```
sudo add-apt-repository \"deb [arch=amd64] https://download.docker.com/linux/ubuntu \$(lsb_release -cs) \stable"
```
```
sudo apt-get update
```
```
sudo apt-get install docker-ce7
```
#### For Checking the docker version follow the command
```
docker version
```

Reference: https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-docker-ce-1
### Add user to DockerGroup:
```
sudo usermod -aG docker <username>
```

# Commands to Install Docker Machine
```
base=https://github.com/docker/machine/releases/download/v0.14.0 && curl -L $base/docker-machine-$(uname -s)-$(uname -m) >/tmp/docker-machine && sudo install /tmp/docker-machine /usr/local/bin/docker-machine
```

#### For Checking the docker-machine version follow the command
```
 docker-machine version
```
Reference: https://docs.docker.com/machine/install-machine/#install-machine-directly

# Commands to Install Docker Compose
```
sudo curl -L https://github.com/docker/compose/releases/download/v2.29.1/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose
```
```
sudo chmod +x /usr/local/bin/docker-compose
```

#### For Checking the docker-compose version follow the command
```
docker-compose --version
```
Reference: [https://docs.docker.com/compose/install/#install-compose](https://docs.docker.com/compose/install/linux/)
