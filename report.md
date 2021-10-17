# 1. Project Objectives
The project aims to integrate Mycroft (a voice assistant platform) with computer vision technology to implement an intelligent reasoning system. The system is designed for blind people to have an easier shopping experience. There are two use cases related to this scenario to help blind people find corresponding goods they demand in the supermarket using the designed Easy Shopping system.

## 1.1 Introduction 
In daily life, it is very inconvenient for blind people to travel and live alone, especially when they go to the supermarket to buy goods. It is impossible if they go shopping without other’s help. Therefore, our Easy Shopping system is designed to provide them with a personal shopping assistant to help them locate desired goods and make them enjoy shopping. To some extent, our system can partly replace the eyes. When blind people go to the supermarket, they do not need the assistance from families or staff anymore. 

## 1.2 Use Case Design
According to the introduction above, we design two use cases of this Easy Shopping project for blind people using it for shopping alone.

> Use case 1: Find the item from multiple items. \
User will take a photo of the goods shelf in front of him/her. And then ask Mycroft if the item they want is in this photo. If the item they want is in the photo(in front of the user), Mycroft will also give the user a general position of that item. 

> Use case 2: Get the detailed information of the item in hand.\
User will take a photo of the goods in his/her hand. And then ask Mycroft what is the item in the hand. Mycroft will also give the detailed information of the goods, for example, the brand, the colour.

# 2. Mycroft (voice assistant) installation
## 2.1 Create your Mycroft account
You can go to the My Account page to create your own Mycroft account by using your Facebook account or your Google account or your GitHub account or by signing up with your email address and setting your password.

![The San Juan Mountains are beautiful!](/Users/linyaya/Desktop/reportimg/1.jpg)

After log in, you are directed to your Mycroft Home dashboard, you are able to maintain your profile, skills, and devices here. 

![The San Juan Mountains are beautiful!](/Users/linyaya/Desktop/reportimg/1.jpg)

## 2.2 Install Mycroft
Before installing the Mycroft on your device, you should make sure your operating system is Linux or you have the Linux VM on your machine. If you have not installed the Linux VM yet, you may refer to the steps below to install the VM on your machine.

Steps of installing Ubuntu in VirtualBox:

When you have successfully installed Ubuntu in VirtualBox, you can start to install Mycroft in VirtualBox's base environment on your machine. You can refer to the steps below.
Steps of installing Mycroft(run below commands):

```
sudo apt-get update
sudo apt-get install -y alsa pulseaudio
git clone https://github.com/MycroftAI/mycroft-core.git
cd mycroft-core
./dev_setup.sh -fm
sudo reboot
```

## 2.3 Pair your device
Before pairing your device, you should make sure you already have a Mycroft account and you have logged into your account, if you have not created your Mycroft account, you can refer to the 2.1 to create an account.
Click the Add Device at the home.mycroft.ai account page:

![The San Juan Mountains are beautiful!](/Users/linyaya/Desktop/reportimg/1.jpg)

To add a device in your account, you need a 6-character Registration Code. The Registration Code will be provided when you first run start-mycroft.sh debug to start your Mycroft device.
![The San Juan Mountains are beautiful!](/Users/linyaya/Desktop/reportimg/1.jpg)


If there is no 6-character Registration Code displaying to you in CLI, you should type “pair my device” to get the 6-character Registration Code.

After you get the 6-character Registration Code(pairing code) successfully, you should use this pairing code and provide a meaningful name and location for the Device. This will help you in the future if you have multiple devices.
