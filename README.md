# virtualization
Virtualization is an additional abstraction layer between network and storage hardware, computing, and the application running on it. Usually you can run a single operating system per machine which can be very inflexible .  A machine with a virtualization layer can create other virtual machines, where you can install additional operating systems.It means os need not be bound to the PC it runs on. The os is abstracted from the hardware in other words os in not installed directly on the hardware. Instead there is a layer in between the physical server and the os installed called the virtualization layer.A few examples of VMware are ESX or ESXi.

Server Virtualization makes it possible for the OS of a physical server to run on virtual layer (the hypervisor). It allows you to run multiple VMs , each with their own OS , on the same physical serverVirtual host is the physical server with the virtualization layer on it . On top of the virtual layer we have different virtual machines .

HYPERVISOR

-Hypervisor creates the virtualization layer that makes server virtualization possible.
-It contains virtual machine manager which manages the multiple virtual machines.

There are two types of hypervisor.
A. TYPE 1 HYPERVISOR
-A Type 1 hypervisor runs directly on the host machine's physical hardware.It is also reffered to as bare-metal hypervisor.
-Type 1 hypervisors are regarded as the most efficient and best-performing hypervisors.
-Hypervisors that run directly on physical hardware are also highly secure. The security flaws and vulnerabilities that are generally present in underlying OS are absent from bare-metal hypervisors because the attack surface of the underlying OS is not present. 
-Hypervisors such as VMware ESXi, Microsoft Hyper-V server and open source KVM and the many Xen variants are examples of Type 1 hypervisors.
B. TYPE TWO HYPERVISOR
-Type 2 hypervisor resides on top of the operating system. 
-Since they cannot directly communicate with the hardware, they are less efficient than the type 1.
-In type 2 hypervisor, the OS takes care of all the hardware. That is why a  type 2 hypervisor can support a wide range of hardware. It is also easy to install.
-Its dis advantage is that any problem in base OS will affect the guest OS and the virtual machine.
-Example of type 2 hypervisor VMware Player, VMware Workstation, and Microsoft Virtual Server .
