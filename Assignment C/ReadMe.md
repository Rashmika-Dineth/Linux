# Programming With C

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

