# Docker_installation
Installation of Docker


## Steps to install docker 
1. ``sudo apt-get update``
2.   ``sudo apt-get remove docker docker-engine docker.io``
3.   ``sudo apt install docker.io``
4.    ``sudo apt-get install apt-transport-https ca-certificates curl software-properties-common``
5.    ``curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add``   (It should return OK)
6.    ``sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu  $(lsb_release -cs)  stable"``
7.    ``sudo apt-get update``
8.    ``sudo apt-get install docker-ce``

## Steps to install docker compose
1. ``sudo curl -L "https://github.com/docker/compose/releases/download/1.25.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose``
2. ``sudo chmod +x /usr/local/bin/docker-compose``
3. (Optional) To add the user to the sudoer for docker. create docker group. 
   ``sudo groupadd docker``
4. (Optional) To add the user to the sudoer for docker.
   ``sudo usermod -aG docker $USER``
5. In order to apply the user changes, it may be necessary to restart the vm for changes to take effect. On a desktop Linux environment such as Windows, log out of your session completely and then log back in.
