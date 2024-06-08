# Lesson 1: Install Oracle VM VirtualBox in Ubuntu and Configuration

First, it will be necessary to download Oracle VM VirtualBox, a software that allows you to create and run multiple operating systems on a single physical 
machine (host), such as Linux, Windows, macOS, Solaris, BSD, among others, without the need to reinstall the main operating system of the computer.

## Parte 1 : Installation

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

And run one of the commands below to install the desired version of Oracle VM VirtualBox on your Ubuntu or Linux Mint:

To install VirtualBox 7.0, run:

~~~
sudo apt install virtualbox-7.0
~~~

To install VirtualBox 6.1, run:

~~~
sudo apt install virtualbox-6.1
~~~

Once the installation is complete, run the command below to add your user to the vboxusers group:

~~~
sudo usermod -a -G vboxusers $USER
~~~

To remove the version from the official repository:

~~~
### Para remover o VirtualBox 7.0, execute:
sudo apt remove virtualbox-7.0

### Para remover o VirtualBox 6.1, execute:
sudo apt remove virtualbox-6.1
~~~

## Parte 2 - Configuration

After installing Oracle VirtualBox, you need to configure the software to create a virtual machine. Follow the following steps:

1. Search "Oracle VirtualBox" in your computer's search bar and open the software.

2. In the Oracle VirtualBox toolbar, click "Machine".

3. Then select "New" to start creating a new virtual machine.

As shown in the image below:

<div align="center">

![1](https://github.com/mickaelly01nobre/SIP-Protocol-VoIP/assets/171987167/1afa9220-5a93-4eaf-b6e5-6dc20b4f857e)

</div>

Then, a new tab will appear with the fields "Name", "Type" and "Version". Fill in these fields as follows:

* Name: FreePBX
* Type: Linux
* Version: Fedora (64-bit)

As shown below:

<div align="center">
 
![2](https://github.com/mickaelly01nobre/SIP-Protocol-VoIP/assets/171987167/85b4fe0d-3bd4-4be2-bcd4-695e0a96f0e6)

</div>

The next part will be the memory size, which will be allocated 2048. As shown in the figure below:


<div align="center">
 

![3](https://github.com/mickaelly01nobre/SIP-Protocol-VoIP/assets/171987167/a20597e8-f568-42d6-aabc-0d9b891a9012)


</div>

In the next step, the Hard Disk configuration will take place, which is selected "Create a new virtual hard disk now". Exemplified below:

<div align="center">
 

![4](https://github.com/mickaelly01nobre/SIP-Protocol-VoIP/assets/171987167/f1baba93-3f9e-4d60-b0e8-3f7a60e2e360)


</div>

Then click on "Expert Mode". As shown:

<div align="center">
 

![5](https://github.com/mickaelly01nobre/SIP-Protocol-VoIP/assets/171987167/40aba0e4-d126-49fd-9b1a-226bcd7e1539)



</div>




