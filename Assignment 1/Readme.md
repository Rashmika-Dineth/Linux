# Assingment 1 - Virtual Machine creation

1. Create a new Azure account for yourself using your HAMK student ID (email) portal.azure.com & login.

![](Images/img1.JPG)

2. Select Create a resource from Azure services,

![](Images/img2.JPG)

3. Select Virtual machine from services and click Create

![](Images/img3.JPG)

4. You can create resource group name and virtual machine name, Select the Region (Closest Region selected), and Select the "Ubuntu Server 24.04 LTS gen 2 Server published by Canonical"

![](Images/img4.JPG)

5. Set the machine virtual machine size to Standard_B2ls_v2 and use SSH public key for authentication type.

![](Images/img5.JPG)

6. Add a user name and for authentication and select all inbound ports then press Next.

![](Images/img6.JPG)

7. Select the "Standard SSD" disk type (Not premium) as it will reduce the billing and make sure that **"Delete with VM"** is clicked so it will delete the disk with VM.

![](Images/img7.JPG)

8. Continue with the following network settings,

![](Images/img8.JPG)

9. Update the auto shoutdown time so you do not have to pay for shutdowntime of the server. And click Review and Create.

![](Images/img9.JPG)

10. Once the validation passed it will show the summary of the if everything seems good create the vm.

![](Images/img10.JPG)

11. When creating the VM it will generate the SSH key and save it in a place that only you have access.

![](Images/img11.JPG)

12. Save this key ".pem" file for future use. I save it under Keys folder in my documents.

![](Images/img12.JPG)

13. Once the creation is success you will see the success image as below,

![](Images/img13.JPG)

14. Once you go inside this VM you will see the Overview details as below,

![](Images/img14.JPG)

15. Now you need to set the DNS inorder to communicate with the VM,

![](Images/img15.JPG)

16. Press configure and set the DNS name,

![](Images/img21.JPG)

17. In Navigation select Connect => Connect to set up network,

![](Images/img16.JPG)

18. You can select the Most common **"Native SSH"** method,

![](Images/img17.JPG)

19. First copy the path of the key file Ex: "C:\Users\rashm\Documents\Keys\linux-lab_key_0117.pem". You can do this by **Shift+ right mouse click on the key file => copy as path**. Then paste it in option 3 and Copy and execute SSH command. **ssh -i "C:\Users\rashm\Documents\Keys\linux-lab_key_0117.pem" azuredineth@74.234.40.225**

![](Images/img18.JPG)

20. Open the cmd and enter the above value,

![](Images/img19.JPG)

21. Enter yes for question "Are you sure you want to continue connecting?" Then it will connect to the Azure VM in local.

![](Images/img20.JPG)

22. You can shutdown the VM by command, "sudo shutdown now"

![](Images/img22.JPG)

23. You can confirm the server is not up by checking the status in the Overview tab.

![](Images/img23.JPG)

---

## Connect with PuTTY

1. Restart the server VM.

![](Images/img24.JPG)

2. Install the Putty Software and open puTTYgen

![](Images/img25.JPG)

3. Load the key (.pem) file to the puTTYgen

![](Images/img26.JPG)

4. Save the private key, so we can use the generated PuTTY key, now close PuTTYgen and open PuTTY.

![](Images/img27.JPG)

5. Copy the public IP from the VM and save it in PuTTY.

![](Images/img28.JPG)

6. Select the key under Connection => SSH => Auth => Credentials => Private key file for authentication

![](Images/img29.JPG)

7. Now press open to open the terminal window

![](Images/img30.JPG)

8. Now give the username that you gave in the VM and press Enter. Now you are in...

![](Images/img31.JPG)

9. You can shut down the VM by the same way did in terminal.

![](Images/img32.JPG)
