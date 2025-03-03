# Assignment 8

## Task:

### Create a firewall for your server that loads when the server starts.

1. Enable and Configure the Firewall to Start on Boot,

![](./Images/1.png)

Update the packages and install ufw

![](./Images/2.png)

Enable ufw on startup

### Define the following services for the firewall:

1. Openssh server : This allow SSH (port 22) traffic

Allow OpenSSH:

![](./Images/3.png)

2. http and https server

![](./Images/4.png)

3. Define the firewall so that all connections blocked by the firewall are logged.

![](./Images/5.png)

4. Define a log for all known and allowed services.

![](./Images/6.png)

5.  Create rules for the firewall that can prevent at least SYN flood type attacks. - This rate-limits SSH to prevent brute-force login attempts.
    ![](./Images/7.png)

        - This limits new TCP connections to 1 per second with a burst of 3

    ![](./Images/8.png)

6.  Find out what other common types of attacks you can prevent with your firewall. - ICMP (Ping) Flooding: Prevent ping floods by limiting ICMP requests:
    ![](./Images/9.0.png)
    ![](./Images/9.1.png)
    ![](./Images/9.2.png)
    Check ping command
    ![](./Images/9.3.png)

            - Port Scanning : Prevent port scans using:

        ![](./Images/10.png)

7.  Define at least one rule identified in this study for the firewall.

- Defined above

Check the settings

![](./Images/11.png)
