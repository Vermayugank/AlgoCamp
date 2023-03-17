### Step 1: Enable Windows Subsytem
Search Turn Windows features on and off > Windows Subsystem for Linux, check the box, and then click the OK

### Step 2: Install Ubuntu
Create username and password 

### Step 3: Run following commands in Ubuntu terminal

sudo apt-get update           //to update all packages automatically
sudo apt-get upgrade          //to upgrade all packages to their latest versions
sudo apt-get dist-upgrade     //to delete obsolete packages

### Step 4: Run the following command on powershell
wsl --set-version Ubuntu 2

### Step 5: Open up your Docker Desktop, go to settings (top right corner - the gear icon), then select resources, and then select WSL Integration, and make sure that integration with Ubuntu is enabled.

### Step 6: If you don’t want to preface the docker command with sudo, create a Unix group called docker and add users to it. When the Docker daemon starts, it creates a Unix socket accessible by members of the docker group. On some Linux distributions, the system automatically creates this group when installing Docker Engine using a package manager. In that case, there is no need for you to manually create the group.
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker

Restart the ubuntu and docker and run the below command

docker run hello-world


