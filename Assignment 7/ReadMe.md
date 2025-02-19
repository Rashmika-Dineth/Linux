# Assignment 7 - Virtualization

### Machine specs on Azure:

1. For use of virtualization in Linux its better to use a VM with higher performance.

2. So we create a VM with high performance,

![](./Images/1.png)

### Checking virtualization support on machine:

1. Once the VM is created we can check the virtualization support by cpuinfo, **cat /proc/cpuinfo**

![](./Images/2.png)

2. Am I using 64 bit CPU/system [x86_64/AMD64/Intel64]? IN flags check for **lm**

![](./Images/3.png)

3. Do I have hardware virtualization support?

   - vmx – Intel VT-x, virtualization support enabled in BIOS.
   - svm – AMD SVM, virtualization enabled in BIOS.

   - Since we are using intel based system we only have VMX

![](./Images/4.png)

4.Do I have hardware AES/AES-NI advanced encryption support?

aes – Applications performing encryption and decryption using the Advanced Encryption Standard on Intel and AMD cpus.

![](./Images/5.png)

### # Install kvm-ok on a Debian/Ubuntu

1. sudo apt install cpu-checker

![](./Images/6.png)

2. sudo kvm-ok

![](./Images/7.png)
