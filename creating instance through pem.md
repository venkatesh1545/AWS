## Create an AWS EC2 instance Process and Connecting to Mobaxterm through .pem file
### Step 1: Create an AWS EC2 instance
* Go to the AWS Management Console and navigate to the EC2 dashboard
* Click on "Launch Instance" and choose the desired instance type (e.g. t2.micro and choose AWS Linux)
* Choose the instance type
* Create a new Key pair with with choosing .pem file extension
* Launch instance
* Click on Hyper link which is there in Successfully connected 
* Go to Details and copy the ipv4 address 
* Go to Mobaxterm app &rarr; Click on Session &rarr; Click on SSH
* Paste the **ip address** in Host Address and give the username as **"ec2-user"** 
    #### For Checking the username:
    **When the instance was created, click on the checkbox &rarr; Click on connect &rarr; Go to SSh client and there you find **"ubuntu@ec2-54-162-228-147.compute-1"** in example phase here username was **"ubuntu"****

* Click on Advanced SSH client &rarr; Give provate Key which was downloaded. &rarr; click on **ok!**
* You will be Logged in


