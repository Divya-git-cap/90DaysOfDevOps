# Day 7 Task: Understanding Package Manager and Systemctl

### What is a Package Manager in Linux?

 A package is a set of files, metadata,etc required to install any software. In simple terms, a package manager is a software tool used for package management in Linux for managing the installation, removal, and updation of various software packages. The package manager can be a graphical application like a software center or a command line tool like apt-get or pacman.


### What is a Package?

 A package is a set of files, metadata,etc required to install any software.A package contains all the necessary data required for the installation and maintenance of the software package

### Different Kinds of Package Managers
Different types of package managers are apt(primary oackage manager for ubuntu), dnf(package manager for Fedora), yum(RHEL & Centos), pacman(Archlinux & its derivatives).

## Tasks

1. **Install Docker and Jenkins:**
Run the following commands-To install docker- sudo apt-get update ,sudo apt-get install docker & sudo usermod -aG docker $USER
To install jenkins- sudo apt-get install jenkins

### Systemctl and Systemd

Systemctl is used to examine and control the state of the “systemd” system and service manager. Systemd is a system and service manager for Unix-like operating systems allowing to start, stop & check service status .

## Tasks

1. **Check Docker Service Status:**
   sudo systemctl status docker
3. **Manage Jenkins Service:**
   - Stop the Jenkins service and post before and after screenshots.

4. **Read About Systemctl vs. Service:**
   - Read about the differences between the `systemctl` and `service` commands.
   - Example: `systemctl status docker` vs. `service docker status`.

   For reference, read [this article](https://www.howtogeek.com/devops/how-to-check-if-the-docker-daemon-or-a-container-is-running/#:~:text=Checking%20With%20Systemctl&text=Check%20what%27s%20displayed%20under%20%E2%80%9CActive,running%20sudo%20systemctl%20start%20docker%20).

### Additional Tasks

4. **Automate Service Management:**
   - Write a script to automate the starting and stopping of Docker and Jenkins services.

5. **Enable and Disable Services:**
   - Use systemctl to enable Docker to start on boot and disable Jenkins from starting on boot.

6. **Analyze Logs:**
   - Use journalctl to analyze the logs of the Docker and Jenkins services. Post your findings.

#### Post about your progress and invite your friends to join the #90DaysOfDevOps challenge.

[← Previous Day](../day06/README.md) | [Next Day →](../day08/README.md)
