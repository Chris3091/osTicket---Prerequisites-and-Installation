<img width="511" height="291" alt="image" src="https://github.com/user-attachments/assets/99798902-d0b9-4790-b189-43360e960888" />


# osTicket---Prerequisites-and-Installation
In this lab, I will install osTicket which is an open-source software used for help desk ticketing. This will be completed using a VM created in Azure. 

# Environments and Technologies Used

Microsoft Azure (Virtual Machines/Compute)

Remote Desktop

Internet Information Services (IIS)

# Windows Services Used
 
Windows 11

# List of Prequisities

Microsoft Azure virtual machine

osTicket v1.15.8

Installing Active Directory in one of the virtual instances

Heidi SQL

MySQL

PHP Manager

VC Redist

Rewrite Module

# Installation Steps

First, I to created a resource group in Azure (os-Ticket) in which our VM will be installed into. Once the VM is running, I can make all the necessary installations to get osTicket installed. I'm using a VM build with Windows (Windows Server 2025 Datacenter Azure Edition) and it is using a core of 2 with 42GB of RAM which should be sufficient for this lab to supply with enough computing power. The location is in East US (Zone 1).

<img width="1763" height="844" alt="image" src="https://github.com/user-attachments/assets/132c2277-4121-4d24-8041-5763f4a423fe" />

Next, You have to copy the public IP address that from the VM and put it into remote desktop. I need connect to this newly created VM using the Remote Desktop Connection which is a default Windows program and use the username and password that I inputed the VM.

<img width="542" height="312" alt="image" src="https://github.com/user-attachments/assets/2d489f0e-c832-4be0-8ace-c15666086200" />

Then, proceed to select yes then you should be on the virtual desktop. I will be masking the username and password for this part of the lab.

<img width="511" height="485" alt="image" src="https://github.com/user-attachments/assets/dcfcf0da-e278-408c-8976-e08fda3f0c91" />

Once Inside the virtual machine. The first thing you should see is the server manager when you connect to the virtual desktop.

<img width="1452" height="592" alt="image" src="https://github.com/user-attachments/assets/09f9cb54-cff0-47f4-aa1d-b3272e719132" />

Next, I used the os-ticket installation file from earlier in the course i copied and pasted it. Then , I put it in the virtual desktop and downloaded the file so, I can proceed to the next step.

<img width="872" height="101" alt="image" src="https://github.com/user-attachments/assets/8427916a-c68c-40cf-9470-9a900b487e89" />

Next, we are going to do the IIS. we have to go the control panel in the command bar. We are going to open the control and click programs ten, click uninstall program ( click the turn window features on or off)

<img width="812" height="538" alt="image" src="https://github.com/user-attachments/assets/bfa374de-6070-40f6-be1a-9ca26692bb8c" />
<img width="699" height="420" alt="image" src="https://github.com/user-attachments/assets/44d6fb36-8be9-44e7-b1de-423e79a7854e" />

Once, you click that your screen should like mine (it might not it might depends on your OS your using). Then, your going to click next and then role based, then click next and next again for the select server roles.

<img width="997" height="708" alt="image" src="https://github.com/user-attachments/assets/390ebad4-222e-4b14-8c5d-c102aacd5572" />

It should look something like this. You have make Active Directory Domain Service is checked because mine was unchecked.

<img width="985" height="688" alt="image" src="https://github.com/user-attachments/assets/023c0538-1a94-4322-9ff0-d58cb572407e" />

Next, you want to install IIS with CGI you will have to go to server manager then click add roles or features then, click next, go to web server IIS click web server, then application development then, click CGI

<img width="990" height="685" alt="image" src="https://github.com/user-attachments/assets/4bb88067-c04c-4327-96b3-591d74011166" />

<img width="446" height="437" alt="image" src="https://github.com/user-attachments/assets/90a3f87e-2836-41b2-a4f5-fa1385559d05" />

Next, you want to click install then wait a few minutes for the CGI can be installed.

<img width="253" height="238" alt="image" src="https://github.com/user-attachments/assets/d89b013e-6a48-4899-8eac-fd7bdf0e487d" />

Next, We are going to install PHP manager for IIS, so we are going back to the ostick installation file and clicking the PHP Manager.

<img width="1337" height="558" alt="image" src="https://github.com/user-attachments/assets/30eeb993-f011-41ed-8b41-20ffe311427c" />

<img width="735" height="546" alt="image" src="https://github.com/user-attachments/assets/4d7f30b5-795a-4532-9446-939a2e2ae7dd" />

That is what you will see when you open PHP Manager, then you click next and click agree then it will automatically install and that's how PHP manager will installed.

<img width="640" height="531" alt="image" src="https://github.com/user-attachments/assets/443154f7-59b7-4c92-869c-c77c9b8bd3e4" />

Next, we going to install rewrite, so we are going back to the osticket file installation and clicking rewrite.

<img width="665" height="536" alt="image" src="https://github.com/user-attachments/assets/3df9f9ed-34fc-46d2-962f-3b674d8b2407" />

Then, you will click I agree and then click install and it will begin to install and you will then see this scrren letting you know rewrite is installed

<img width="631" height="530" alt="image" src="https://github.com/user-attachments/assets/ff1bb817-f920-419e-bc31-026b89946a0f" />

Next, we are going to proceed to the next step and that is to create a directory called PHP. You will go to the directory files then, click this PC, next click window C and make your own folder.

<img width="780" height="382" alt="image" src="https://github.com/user-attachments/assets/1aacae1f-6043-4b9a-a31d-65261df51823" />

Next, we are going to unzip PHP in the os ticket installion file folder and to do that we will have to extract all info in that folder and we will put it in the PHP folder





