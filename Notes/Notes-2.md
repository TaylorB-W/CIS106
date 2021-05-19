# Installing Ubuntu
* What is Virtualization?
  * Virtualization: replication of hardware to simulate a virtual machine inside a physical machine.
  * 2 general types:
    * Server-side virtualization
      - VDI = Virtual Desktop Infrastructure
        - Thick/fat client: full-featured computers that are connected to a network. Functional whether connected to a network or not.
        - Thin client: computer that runs from resources stored on a central server instead of a localized hard drive. Work by connecting remotely to a server-based computing environment where most apps, sensitive data, and memory are stored.
        - Zero client: has no operating system (OS) and no local storage as an endpoint device.  All desktop applications are provisioned and centrally managed from a remote server.
    * Client-side virtualization
        - Software installed on a computer to manage virtual machines
        - Computer needs:
            1. Hypervisor
            2. Hardware that supports virtualization
               - Capable CPU
               - Enough RAM
               - Enough Storage
  * The main difference is the **location** of virtualization.
* Installing Ubuntu In a virtual machine
  1. After VirtualBox is installed, create a virtual machine with these specs:
     * OS: Ubuntu 20.04 64 Bits
     * HDD: 50 GB
     * RAM: 2 GB (2048 MB)
     * Audio Controller: Disabled
     * CPU: 2 Cores
     * Description:
       * **Hostname:** cis106vm
       *  **User:** TaylorB
       *  **Password:** pccc
     * Shared Clipboard: Enabled - Bidirectional
     * Drag n' Drop: Enabled - Bidirectional     
       * I can cut, paste, drag items from host machine to vm and vice versa  
   