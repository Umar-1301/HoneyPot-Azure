# Guide

## Prerequisites

* Azure account ( you can get £200 in free credit which is more than enough for a few tries at this )
* Familiarity with Azure basics ( or you can learn through this )


### Step 1: Create the VM

![image](https://github.com/user-attachments/assets/546ee03e-e225-488e-837e-8b2257d4aab5)
![image](https://github.com/user-attachments/assets/33fefd67-cef2-45a5-b286-7a5f3d40ea62)

### Step 2: Create Log Analytics Workspace

![image](https://github.com/user-attachments/assets/dfe0d4d4-6fd2-4c36-88f6-ae7ca843a23d)

### Step 3: Configure Microsoft Defender for cloud

![image](https://github.com/user-attachments/assets/5dea5d29-e9c4-4db5-91a7-6e95f2c25cc5)
![image](https://github.com/user-attachments/assets/6a7dc74a-3ec5-45c3-96c3-581b98bbfb59)

### Step 4: Connect VM to LAW

![image](https://github.com/user-attachments/assets/4459d869-1f45-4a8f-9ef1-799e1e87bf9e)
![image](https://github.com/user-attachments/assets/1657d7cf-69a2-4922-aa8b-6052d0403520)

### Step 5: Add sentinel to the correct resource group

![image](https://github.com/user-attachments/assets/0a76268d-5f80-43ed-a476-960ce41b4377)

### Step 6: Initialise RDP connection

![image](https://github.com/user-attachments/assets/11a74be0-d1e0-44a6-992f-4131ecd62981)


### Step 7: Alter Firewall config on VM

![image](https://github.com/user-attachments/assets/bb0c1dda-10a5-46b4-92b7-391c8c27e58c)
![image](https://github.com/user-attachments/assets/430f6cbc-3bca-4e77-aa3c-d11ec6cf090b)
![image](https://github.com/user-attachments/assets/4128a545-0fb8-48aa-9bca-f6d56e95200a)

### Step 8: Create IP Geolocation account - generate a key and insert into script

![image](https://github.com/user-attachments/assets/1e8b88cb-8003-4554-859e-e7c8e8cdf42d)
![image](https://github.com/user-attachments/assets/ece1a005-6e1f-4f76-9848-b0b0cf0d9c16)


### Step 9: Copy log into notepad on own PC

- The script will generate a log at ' c:\ProgramData\failed_rdp.log'
![image](https://github.com/user-attachments/assets/eb82e39f-e415-4d0e-9284-8657c2f24210)

### Step 10: Create sample log in azure

![image](https://github.com/user-attachments/assets/9b3c0137-4d57-4164-8fdf-82b298c74307)
![image](https://github.com/user-attachments/assets/ab0d6c8c-bd63-45db-ac9a-9cf8f61dbcb0)

### Step 11: Wait 10 minutes and run query in custom log

![image](https://github.com/user-attachments/assets/bcfe0b6e-bda6-4e94-b377-09930a6f3b15)
- Clean up the result with some code
![image](https://github.com/user-attachments/assets/214026d7-497e-4596-8f8c-8e50bcf718da)

### Step 12: Go to sentinel to now see the events
![image](https://github.com/user-attachments/assets/b5f2eb5b-a593-4d29-8126-456f7980b634)

### Step 13: Create playbook to get the map
![image](https://github.com/user-attachments/assets/210e5eb2-7446-4fe8-9cc7-48d34b1f6ea7)




## Results

Initially: 
![image](https://github.com/user-attachments/assets/86936938-8b63-44f7-acc9-d91681a0a29a)

End of Day: 
![image](https://github.com/user-attachments/assets/a6010759-5b78-457a-b237-a2aff3b1ac29)

Next Day: 
![image](https://github.com/user-attachments/assets/102d49d4-3123-4e37-beec-fa60db5d3505)









