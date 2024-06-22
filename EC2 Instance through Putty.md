### Creation of EC2 Instance through Putty Software
Virtual  Machines are nothing but Virtual Servers

EC2 Instance is said to be as **ECC**<br>
**ECC &rarr; Elastic Compute Cloud**<br>
**AMI &rarr; Amazon Machine Image**

### Process to Create Ec2 instance
Steps Required to Create Instance in **AWS Academy**
1. Login to [aws Academy](https://www.awsacademy.com/vforcesite/LMS_Login)
2. Go to **Modules** &rarr; Go to **Sandbox Environment** &rarr; Open **link in new tab**
3. Click on Start Lab and it will open another page close the tab and come back to previous page and **Click on AWS**
4. Open **EC2** instance from recently viewed tabs
5. Click on **Launch instance** button 
6. Give **name and tags** for your Instance Name
7. In **Application and OS Images (Amazon Machine Image)** Select your Linux Provider (for example: Redhat, Linux, Ubuntu, AWS, Windows etc...) 
8. Don't change any thing in Instance Type
9. In **Key Pair Login**, Click on **Create a new Key pair**
10. Enter the Key Pair name (what ever you want) &rarr; Select **".ppK"** file 
11. Make sure that you have selected **RSA** in Key Pair type
12. Click on the **Hyper link**(<i>for example,</i> **"(<u>i-08f7b1a434c34c127</u>)"**) where it is visible in **"Successfully initiated Launch of instance"**
13. Copy your ip address and remember your platform provider
14. Open your Putty Software Application in your System

## If not installed Putty Software
- [Download](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html) putty
- choose 64-bit x86 in MSI('Windows installer')
- open the Putty App
- Paste your Ip Address
- select SSH &rarr; in category Go to **SSH** &rarr; Go to **Auth** &rarr; Go to **credentials** 
- click on credentials
- In **private key file for authentication**, click on **browse** Select the .ppk file from your dowloads folder and click on **"ok"**. that's it.
- give the username as "ubuntu"
- you will be logged in ...