# Assignment 1 (6p)

---

## 1. Setting Up C Programming Environment on Linux

### A. Install the GCC Compiler

Most Linux distributions come with the GCC (GNU Compiler Collection) pre-installed. To check if GCC is installed, run:

    - gcc --version

If it's not installed, install it using:

Ubuntu/Debian:

    - sudo apt update

    - sudo apt install gcc

Once installed, verify by running:

    - gcc --version

Since we already have installed gcc compiler we do not need to install the compiler again.

![](./Images/1.png)

### B. Make a small C program "mycalc.c" to ask user 2 numbers, and print the sum

1. For ease of use I created a directory called calculator and Im gonna use this folder to write my c program.

![](./Images/2.png)

2. Create mycalc.c using nano editor.

![](./Images/3.png)

3. Inorder to check our env & other setting, first try to run Hello world app,

   - Update the file
   - Save the file (Ctrl + s)
   - Exit from nano editor (Ctrl + x)

![](./Images/4.png)

4. Compile the file and make mycalc program. (-o mycalc : Output will be mycalc)

   - gcc mycalc.c -o mycalc

5. Now Run the app and check if its working with no issues.

![](./Images/5.png)

6. Now we can modify to add our calculator codes.

![](./Images/6.png)

7. Compile and run the program

![](./Images/7.png)

---

## 2. Part 2 - Setting up node JS server on Linux VM

1. Make the directory myserver and go inside the folder, get the latest update of apt updates,

![](./Images/Part%202/1.png)

2. Install the Node JS and check the version of node and npm, then initiate the node js program,

![](./Images/Part%202/2.png)

3. Install the node package express and update the index.js package (After this you can run index.js)

![](./Images/Part%202/3.png)

4. Following is the basic code of node js server

![](./Images/Part%202/6.png)

5. Update the firewall settings so that the port can be viewed from outside connections,

![](./Images/Part%202/4.png)

6. Run the server and check its working with the public ip address and your port id ( 'http://74.234.40.225:3000/' )

![](./Images/Part%202/5.png)

7. If you get the following msg then the server is running with no issues,

![](./Images/Part%202/7.png)

8. Update the index.js so the **/user** navigation can display user information by **process.env.USER**
   ![](./Images/Part%202/8.png)

9. Check the result with **/user** navigation,

![](./Images/Part%202/9.png)

---

## 3. Part 3 - Install Python 3, pip, and bpytop on a Linux VM

1. Get the updated apt list and install python

![](./Images/Part%203/1.png)

2. Check the python and pip version. (To make sure setup is success)

![](./Images/Part%203/2.png)

3. Install bpytop as a user, (not root user)
   - pip3 install bpytop --user

![](./Images/Part%203/3.png)

Humm!! .. Got an error...

4. Redo using VM inside Linux, (Install the Virtual Environment Package:)
   - sudo apt install python3-venv

![](./Images/Part%203/4.png)

5. Create and activate Virtual Environment:

![](./Images/Part%203/5.png)

6. Now install bpytop inside the VM and run it,

![](./Images/Part%203/6.png)

7. Take a screenshot of the bpytop

![](./Images/Part%203/8.png)
