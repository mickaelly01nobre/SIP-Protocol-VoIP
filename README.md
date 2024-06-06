For this example of the SIP protocol, we will use Asterisk and FreePBX. Asterisk is an open-source software that functions as a Private Branch Exchange (PBX), 
while FreePBX is a graphical interface for managing Asterisk. Don't worry, this will be explained in more detail later on.

First, it will be necessary to download Oracle VM VirtualBox, a software that allows you to create and run multiple operating systems on a single physical 
machine (host), such as Linux, Windows, macOS, Solaris, BSD, among others, without the need to reinstall the main operating system of the computer.

Step by step to install Oracle VM VirtualBox:

## Lesson 1

### 1.Update your system

~~~
 $ sudo apt update && sudo apt upgrade
~~~
 ### 2.Installing Oracle VirtualBox via official repository

~~~
echo -e "deb [arch=amd64 signed-by=/usr/share/keyrings/oracle-virtualbox-2016.gpg] https://download.virtualbox.org/virtualbox/debian jammy contrib"|sudo tee /etc/apt/sources.list.d/virtualbox.list
~~~

Next, import the GPG signing key with:

~~~
wget -O- https://www.virtualbox.org/download/oracle_vbox_2016.asc | sudo gpg --dearmor --yes --output /usr/share/keyrings/oracle-virtualbox-2016.gpg
~~~

Update your repositories cache:

~~~
sudo apt update
~~~

Install the necessary dependencies with:

~~~
sudo apt-get install binutils build-essential dkms linux-headers-$(uname -r) make
~~~





