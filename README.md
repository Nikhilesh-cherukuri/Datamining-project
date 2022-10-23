# milestone1


CVAT installation instructions

1. Go to this link https://opencv.github.io/cvat/docs/administration/basics/installation/
I use windows.I went to windows 10 section in the link and downloded the follwing:

  1.Docker Desktop for Windows
  
  2.Git for Windows
  
  3.google chrome (if you don't have it installed before)


2.Install and run the downloaded Docker Desktop for Windows.exe

3. Go to the Step 4 - Download the Linux kernel update package in this link https://learn.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package and dowload the package and install it.

4. go to the windows power shell and run the command: wsl --set-default-version 2

5. Go to the app store and install ubuntu distribution of choice
  i installed ubuntu 22.04.1 LTS

6.After installing the ubuntu setup the language and then create a default UNIX user with name ,username and password.

7.  Now install the Git for Windows.exe then setup the git and launch.

8.  Run the following commands in the Git Bash terminal window

    1.git clone https://github.com/opencv/cvat

    2.cd cvat
    
    3.docker-compose up -d
    
    4.winpty docker exec -it cvat_server bash -ic 'python3 ~/manage.py createsuperuser'
    
    5. Then setup the Username,email address and password
    
    
9.Now go to chrome and open https//:localhost:8080.

