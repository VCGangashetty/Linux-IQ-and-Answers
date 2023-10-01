  1 * how do you disable swap memory through cmd line and it should not get added to the system ?
Ans--a)To disable temporarily:
     We use "sudo swapoff -a" command, It disables immeditely untill next reboot, that is why this is just a temporary solution.
     b)To disable Permanently:
     We remove the swap configurations going to the path `/etc/fstab` and commentout using # for the swap memory and use 'sudo swapoff -a' command and reboot the system.
----------------------------------------------------------------------  
  2 * how to make sure that file system does'nt get mounted upon the reboot ?
Ans--We navigate to `etc/fstab` using vi editor and comment out the below line or delete the line seen below:
     **# /dev/sdb1 /mnt/mydata ext4 defaults 0 2**
----------------------------------------------------------------------  
  3 * have you created a file system and how you ensure those file systems are available after reboot (etc filesystems)?
Ans--No, I haven't created the filesystem, think we can ensure these by maintaing the entries in the `/etc/fstab`.
----------------------------------------------------------------------  
  4 * after mounting EBS to instance, weather that will be still available after reboot ?
Ans--if you want an EBS volume to remain available after a reboot, ensure that it is attached and mounted correctly, either during instance launch or manually, and consider adding an entry to the /etc/fstab file if you want it to be automatically mounted upon each reboot.
----------------------------------------------------------------------  
  5 * init levels implements in linux ?
Ans--NA
----------------------------------------------------------------------  
  6 * CMD check the load of the system ?
Ans--To check the system load we use 'uptime' or 'top' command in linux based systems, these commands give systems current & average load with other related statistics.
----------------------------------------------------------------------  
  7 * CMD check usage of memory / ram of the system ?
Ans--To check the usage of memory (RAM) on a Linux-based system using the command line, you can use several commands, such as 'free', 'top', or 'htop'.
----------------------------------------------------------------------  
  8 * CMD to check how many CPU cores are there in system ?
Ans--use the 'lscpu' command in the command line to check how many CPU cores are available on your Linux system.
----------------------------------------------------------------------  
  9 * Suppose I have 100 servers, each server has username and password, if i want to install packages in all those servers remotely without logging in how i will be able to do this using shell script.
Ans--To remotely install packages on multiple servers without logging in manually to each server, you can use SSH (Secure Shell) along with a shell script to automate the process.
----------------------------------------------------------------------  
  10* Using Top command how will you control all process running.
Ans--NA
----------------------------------------------------------------------  
  11* Write shell script to print all alternative lines
Ans--NA
----------------------------------------------------------------------  
  12* script to sort all file in logs and sort it according to top memory consuming and copy it to another file
Ans--NA
----------------------------------------------------------------------  
  13* runlevel commands explain
Ans--NA
----------------------------------------------------------------------
  14* how you'll find complete details of linux version you are using
Ans--Use command 'cat /etc/os-release' .
----------------------------------------------------------------------
  15* Ps -ef?
Ans--The ps -ef command is used to display a detailed list of all processes currently running on a Linux system.
----------------------------------------------------------------------
  16* Kill -9 processname
Ans- This command is used to kill the running process with the name.
----------------------------------------------------------------------
  17* $? $* $0
Ans-- $?--special variable in bashscripting, used to check the status of previous executed script.
      $*--special variable in bashscripting, used to read all the arguments in single string.
      $0--special variable in bashscripting, used to print the file name of the script.  
----------------------------------------------------------------------
  18* Ssh 
  Ans--Secure shell
----------------------------------------------------------------------
  19* what is port no of ssh,http and https
Ans--ssh-22
     http-80
     https-443
----------------------------------------------------------------------
  20* how to list the process running
Ans--Use command 'ps -ef'
----------------------------------------------------------------------

  21* how to login ec2 if pem key lost
----------------------------------------------------------------------
  22* how to check the memory in  linux server
Ans--free, top and htop commands.
----------------------------------------------------------------------
  23* how to get the IP address of server
Ans--hostname -I is the command to get the IP address.
----------------------------------------------------------------------
  24* how do I find available storage on the server using linux cmds?
Ans--du -h or df -h
----------------------------------------------------------------------
  25* how to identify/find files which are more than 10GB in size ?
Ans--Using find command as find . -type f -size +10G
----------------------------------------------------------------------
  26* Git merge and rebase
  27* ssh, keygen
  28* Cmd and entrypoint ,run
  29* Basic command on Linux
  30* linux server goes down what action you are going to take.
  31* How to start the script at boot level
  32* How to start a service at boot level
  33* What is way to run script on background
  34* How do you check open ports
  35* How you see no of arguments
  36* What's k statement in shell script
  37* How to establish password less connection
  38* Shell script for prime numbers for a given range.
  39* Linux boot process, 20 linux commands with explanation
  40* Linux commands - related to memory and system ram
  41* which scripting you are comfortable with?
  42* script  to find the port number
  43* namespaces in Linux 
  44* linux booting process 
  45* types linux os you have used and what is package manager for Ubuntu 
  46* $? and $!
