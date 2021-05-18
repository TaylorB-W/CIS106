# Homework: 4  The Linux Filesystem

Watch the video [“Linux Filesystem Explained”](https://www.youtube.com/watch?v=HbgzrKJvDRw) and read the presentation [“How to navigate the filesystem”](http://bit.ly/3t30rMQ) then answer the questions below.

1. **Explain the difference between absolute path and relative path:** 
   Absolute path states the full pathname starting from root. Relative path specifies the pathname beginning with the current directory.


2. **Why Linux uses / instead of \ for its directory paths?**
   According to the video, Linux follows UNIX traditions, which is why it uses the forward slash instead of the backslash like Windows


3. **In Windows, these files are all the same: File FILE file and FiLE. But in Linux this is not the case, Why?**
   Linux cares about capitalization. Each of these would be different files.


4. **What is the Filesystem Hierarchy Standard (FHS) and who maintains it?**
    TThe FHS is the entity that specifies requirements and guidelines for file and directory placement in UNIX-like operating systems. It is maintained by the Linux Foundation.

5. **Explain what type of files are stored in the following directories:**

Directory | What is it used for?
--------- | --------------------
/bin    | Contains binaries which are system programs or applications.
/dev    | Contains devices
/etc    | Contains system wide configurations
/home   | Each user has a home folder. Contains personal files and documents. Also stores application settings
/lib    | Contains Libraries that files use to perform certain functions.     
/opt    | Contains manually installed software from vendors and some software packages found in the repo.
/tmp    | Contains temporary files stored by applications that could be used during a session. In case the application crashes before the file is saved, recent saved copies are stored here.
/var    | Contains files and directories that will grow in size
/proc   | contains pseudo files that contain information about system processes and resources
/usr    | Contains user applications that are non-essential for basic system operation installed applications.

1. **How does a period at the beginning of a file name means (example .bashrc)?**
   A period at the beginning of a file name indicates a hidden file.


2. **Which command would you use to list all the files inside the /usr/share/ directory?**
   ls -a /usr/share



3. **If you are working in the /usr/share/icons directory and want to move to your home directory, which command would you use?**
   * cd
   * cd ~
   * cd $HOME

4. **Explain what these commands do:**

    * **cd .config/.htop** changes the current directory to hidden directory .config/.htop 
    * **cd ../** 
goes back one directory
    * **ls -lX** lists all the files in a long list sorted by file extension



10. **John has a lot of files in the directory /var/www/html/webapp. He wants to long list all the files, including hidden files, by modification time (newest first), and with human-readable file sizes. Which command should he use conjuring that his current working directory is:** 
    
`/home/john/.git/`
* ls -alth ~/john/.git/