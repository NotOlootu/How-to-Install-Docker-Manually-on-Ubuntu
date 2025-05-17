# How-to-Install-Docker-Manually-on-Ubuntu
This guideline is for those that have Ubuntu installed already and are unable to install docker through automatic installation processes.

## Get Ubuntu Version
```
lsb_release -a
```

![image](https://github.com/user-attachments/assets/c14b66e1-353f-450a-a523-e06d62db485e)

## Download Appropriate Docker Files From Official Doker Page

Go to https://docs.docker.com/engine/install/ubuntu/#install-from-a-package

Download the listed files

![image](https://github.com/user-attachments/assets/918b6f93-e92f-46f3-94f1-322f7296e3f9)

## Change The Default Installation Directory of Ubuntu To The Download Directory
Use the command below to mount your local storage

```
cd /mnt
ls
```

You should have something similar to the picture below

![image](https://github.com/user-attachments/assets/38f7d21e-27f8-489d-908b-cfffbc6f1e5c)

Thereafter, use "cd" and "ls" to locate your download directory (where you downloaded the docker files to).

You can watch the video on my twitter page for further guidance on this.

## Copy and Edit The Insallatiion Command In Notepad (To Suit The Version of Docker Files Downloaded)
Copy, paste and edit the command below in a notepad.

Watch this video on my twitter page to confirm how to edit the command line below

```
sudo dpkg -i ./containerd.io_<version>_<arch>.deb \
  ./docker-ce_<version>_<arch>.deb \
  ./docker-ce-cli_<version>_<arch>.deb \
  ./docker-buildx-plugin_<version>_<arch>.deb \
  ./docker-compose-plugin_<version>_<arch>.deb
```

## Run The Edited Command Line

## Installation Status Query
Confirm if the installation was succesful or not, by running the code below

```
sudo service docker start
sudo docker run hello-world
```

# All Done

Reference (https://docs.docker.com/engine/install/ubuntu/#install-from-a-package)

Kindly follow me on [twitter](https://x.com/journeyer_dunya) for more hacks & updates.

