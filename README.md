# Overview: Lab 1 Installing VirtualBox and Server 2022
Welcome to the first lab of my home lab series! This section of my home lab documentation focuses on the process of installing VirtualBox and setting up a Windows Server 2022 virtual machine within the VirtualBox environment. It outlines the steps for downloading and installing VirtualBox, followed by the creation of a virtual machine to host Windows Server 2022. The project also covers the configuration of basic server settings and prepares the server for further roles, such as Active Directory and domain controller setup. This task serves as the foundation for building a virtualized lab environment that mimics real-world IT infrastructure, ideal for practicing administrative tasks and learning server management techniques.

## Objectives
This repository documents a comprehensive home lab project focused on installing and configuring VirtualBox and Windows Server 2022. The key objectives include:

- Demonstrating the setup and installation process of VirtualBox as a virtualization platform.
- Installing and configuring Windows Server 2022 in a virtualized environment.
- Creating a foundation for further experiments involving Active Directory, system administration, and IT operations.

## Documentation
In this documentation, I will outline the initial steps of setting up my Active Directory home lab. This includes downloading and preparing the essential tools: VirtualBox and Windows Server 2022.

To start, we’ll download VirtualBox from the official website at https://www.virtualbox.org/wiki/Downloads. Since I’m using a Macbook PC, I will be selecting the version for MacOS hosts.
<img width="1435" alt="Screenshot 2025-02-16 at 4 52 26 PM" src="https://github.com/user-attachments/assets/e5bf03ca-3003-4af5-83f9-f4f37ed2a21b" />  
1. Next, we’ll download Windows Server 2022 from the official Microsoft Evaluation Center at https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022.
<img width="1435" alt="Screenshot 2025-02-16 at 4 54 15 PM" src="https://github.com/user-attachments/assets/05e4a5b7-03d0-4aca-9848-93eefa362315" />  
2. To access the free trial, you’ll need to provide your information during the registration process. The trial period lasts for 180 days.
<img width="1435" alt="Screenshot 2025-02-16 at 4 55 44 PM" src="https://github.com/user-attachments/assets/e464b041-cc5a-4c9c-b693-036f2e3bdeab" />  
3. After filling our information, we can finally download the ISO which will be the 64-bit edition (English).
<img width="1256" alt="Screenshot 2025-02-16 at 5 11 47 PM" src="https://github.com/user-attachments/assets/ce324dde-ceb2-4818-ade9-e27a5058d15c" />  
4. Finally our ISO download should appear in our downloads folder.
   <br/>
   <img width="431" alt="Screenshot 2025-02-16 at 5 43 07 PM" src="https://github.com/user-attachments/assets/c75e648d-bfbe-4d3c-8408-89f32ec1f9ab" />  
6. After everything has finished downloading, we can launch VirtualBox and begin configuring the settings for Windows Server 2022. Once VirtualBox is open, navigate to the "Machine" tab at the top and select "New" to create a new virtual machine.
![image](https://github.com/user-attachments/assets/6f107815-8fb6-47e9-9b23-10232c4bacc4)  
7. First, we’ll name our virtual machine "Windows Server 2022 Lab." Next, we’ll locate the ISO image in our Downloads folder. To do this, click the dropdown menu under "ISO Image" and select "Other." From there, we can browse to the Downloads folder and select the Windows Server ISO.
<img width="1436" alt="Screenshot 2025-02-13 at 4 36 08 PM" src="https://github.com/user-attachments/assets/b0436641-9f62-49da-b426-d1cab857e71a" />
<br/>
8. Next, click on "Skip Unattended Installation." Then, proceed to configure the hardware settings for the virtual machine.
<img width="1436" alt="Screenshot 2025-02-13 at 4 36 53 PM" src="https://github.com/user-attachments/assets/e5c59f8d-9434-42bb-8bea-a56e0a74668c" />

<br>

9. By default, the base memory is set to 2048 MB, which should be sufficient for running the virtual machine. However, we can allocate more dependomg on the PC ram for our virtual machine home lab. 
<img width="1436" alt="Screenshot 2025-02-13 at 4 40 13 PM" src="https://github.com/user-attachments/assets/245fc460-38cd-4e82-b900-3c721babb264" />
<br/>
10. For the “Hard disk” configurations everything should be good, just make sure we have “Create a Virtual Hard Disk Now” then click “Finish”.

<img width="1436" alt="Screenshot 2025-02-13 at 4 42 55 PM" src="https://github.com/user-attachments/assets/2c484ebf-6000-41c3-b2d4-c2ba4cc11d51" />

<br>

11. Click Finish
    
<img width="1436" alt="Screenshot 2025-02-13 at 4 43 12 PM" src="https://github.com/user-attachments/assets/f794ae9d-c650-4cbe-b2bc-6848021f6190" />
<br>

12.Now, we’ll boot up the virtual machine by clicking the "Start" button. A prompt for the Microsoft Server Operating System Setup will appear. Click "Next," then select "Install Now" to begin the installation process.

 <img width="1436" alt="Screenshot 2025-02-13 at 4 44 01 PM" src="https://github.com/user-attachments/assets/03467cfd-e7e5-4403-8369-5d70f4fa49e0" /> 
 <br>
13. Now, we’ll boot up the virtual machine by clicking the "Start" button. A prompt for the Microsoft Server Operating System Setup will appear. Click "Next," then select "Install Now" to begin the installation process.


![68747470733a2f2f692e696d6775722e636f6d2f6c786f6a6a68722e706e67](https://github.com/user-attachments/assets/7f029446-51e6-407b-8114-73b26d2e0159)
<br>

14. Click "Install Now" to begin the installation process.
    
![68747470733a2f2f692e696d6775722e636f6d2f47346f625869432e706e67](https://github.com/user-attachments/assets/1097f7ac-91cd-43dd-b2ac-3f16fe893e45)
<br>

16. In the operating system selection screen, choose "Windows Server 2022 Standard Evaluation (Desktop Experience)," then click "Next" to continue.
    
![68747470733a2f2f692e696d6775722e636f6d2f644b7a6f6a37352e706e67](https://github.com/user-attachments/assets/5fadbf7c-d509-4fc7-9bd6-e58de2416d90)
<br>

17. Accept the terms and click "Next." In the next step, when prompted to choose the type of installation, select "Custom" to proceed.
    
![68747470733a2f2f692e696d6775722e636f6d2f6a74736c3153482e706e67](https://github.com/user-attachments/assets/96bad4df-42a7-4773-9569-aae3aa17cd78)











   

