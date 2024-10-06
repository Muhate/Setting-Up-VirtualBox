# Setting Up VirtualBox on Windows

### 1. Description

This project aims to demonstrate how to install Oracle VirtualBox on Windows machine, so that it's easy to follow other guides in this repository.

### 2. Objectives

- Set VirtualBox to run all the home lab projects on.


### 3. Tools and Technologies Used

- **VirtualBox**: Used for creating virtual machines for the lab environment;
- **Windows 11**: Used as a monitored system;

### 4. Installation Steps
First of all, we need to download the executable file of Oracle VirtualBox, so we go <a href="https://www.virtualbox.org/wiki/Downloads">here</a> and we choose the file according to our operating system, her we will be choosing windows. We download the virtualbox executable itself and the VirtualBox Extension Pack, as shown in the image below.

![image](https://github.com/user-attachments/assets/3926968f-b96a-4154-a676-5d24cf2b8e30)

After successfully downloading the files, we will see them on the Download folder as shown below.

<p align="center">
<img width="342" alt="image" src="https://github.com/user-attachments/assets/e3e4a01d-7945-436d-8a1c-c19a3cee6999">
</p>

We'll start by the VirtualBox-version-Win installation, clicking twice and following the steps shown in the image below.

<p align="center">
<img width="500" alt="VirtualBox installation steps" src="https://github.com/user-attachments/assets/5f338569-26cd-4300-9656-93d8eaa29763">
</p>

After successfully installing VirtualBox, it's now time to install the Oracle_VirtualBox_Extension_Pack-version, by double clicking it and following the steps shown below, in the image.

<p align="center">
<img width="600" alt="Oracle_VirtualBox_Extension_Pack installation steps" src="https://github.com/user-attachments/assets/5f72b2d7-1ac1-45e3-8342-3d80b478476e">
</p>

In Virtualbox there are several types of networks, the most used being the bridged adapter and the Nat Network. In our case we will use the Nat Network type because in the Bridged Adapter type it would be necessary to change the machine's network settings each time we use a different network. The NAT Network must be created in VirtualBox, for that we open the VirtualBox and follow the steps in the image below.

<p align="center">
<img width="500" alt="NAT Network creation" src="https://github.com/user-attachments/assets/4c712f19-c8ff-46d8-93b5-7ba6fe62939c">
</p>


### 5. **Conclusion**
   - This project successfully demonstrated the installation of Oracle VirtualBox and its Extension Pack. Next, we briefly present some types of networks in VirtualBox, at the end we learn how to create the NAT Network, which best adapts to our labs, by allowing VMs to communicate with each other and also with the host machine. If any questions arise or you receive any errors while following this guidance, please contact me using the information below.

### 6. **Contact Information**
   - **Name**: Rogério Muhate
   - **Email**: rbmuhate@gmail.com
   - **LinkedIn**: [LinkedIn Profile](https://www.linkedin.com/in/rmuhate)
