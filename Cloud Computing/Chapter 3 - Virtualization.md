
## Virtualization
 - Virtualization is a technology that allows multiple operating systems (OS) and applications to run on a single physical server, by abstracting the hardware resources of the server and presenting them as virtual resources to the operating systems and applications.
 - This allows for greater utilization of hardware resources and can lead to cost savings for organizations.
### Benefits:
1.  Cost savings: Virtualization can reduce the need for physical hardware, leading to cost savings on hardware, power, cooling, and maintenance.
2.  Improved resource utilization: By pooling and sharing resources, virtualization can improve the utilization of hardware resources, leading to better performance and scalability.
3.  Increased flexibility and agility: Virtualization allows for the creation of VMs on demand, enabling quick deployment of applications and services.
4.  Enhanced disaster recovery and business continuity: Virtualization allows for easier backup and restoration of virtual machines, leading to better disaster recovery and business continuity planning.
5.  Simplified management: Virtualization can simplify management tasks, such as provisioning, monitoring, and maintenance, by consolidating multiple physical servers into a single virtual infrastructure.

### Hypervisor
A hypervisor, also known as a virtual machine monitor (VMM), is a software layer that creates and manages virtual machines (VMs) on a physical server.
1.  **Types of hypervisors:** There are two types of hypervisors: Type 1 (or bare-metal) hypervisors run directly on the host server's hardware, while Type 2 hypervisors run on top of an existing operating system.
2.  **Virtual Machines:** The hypervisor allows multiple virtual machines to run on a single physical server by abstracting the hardware resources of the server and presenting them as virtual resources to the virtual machines.
3.  **Resource allocation:** The hypervisor is responsible for allocating physical resources, such as CPU, memory, and storage, to the virtual machines as needed.
4.  **Isolation:** Each virtual machine is isolated from other virtual machines running on the same physical server, ensuring that one VM cannot affect the performance or stability of another.
5.  **Security:** Hypervisors can improve security by isolating applications and workloads from each other, as well as from the underlying physical infrastructure.
6.  **Live Migration:** Hypervisors allow for live migration of virtual machines between physical servers without any downtime, enabling better resource utilization and server maintenance.
7.  **Management:** Hypervisors typically provide management tools to manage the virtual infrastructure, including provisioning, monitoring, and maintenance of virtual machines.

## Types
 - Platform virtualization
 - Resource virtualization

### Platform virtualization
1.  **Emulation or Simulation:** Emulation or simulation involves creating a virtual environment that mimics the behavior of another system or hardware. In emulation, the virtual system completely imitates the hardware of the original system, allowing software written for the original system to run on the virtual system.
2.  **Native virtualization and full virtualization**: Native virtualization, also known as type 1 virtualization or bare-metal virtualization, involves running the hypervisor directly on the physical hardware, providing direct access to hardware resources. Full virtualization is a type of native virtualization that emulates a complete hardware environment, allowing multiple operating systems to run on a single physical server.
3.  **Hardware-enabled virtualization:** Hardware-enabled virtualization involves using hardware support for virtualization, such as Intel VT-x or AMD-V, to improve the performance and efficiency of virtualization.
4.  **Partial virtualization**: Partial virtualization involves virtualizing only specific hardware components, such as CPU or memory, rather than emulating the entire hardware environment.
5.  **Paravirtualization**: Paravirtualization involves modifying the guest operating system to work in a virtualized environment, allowing for better performance and efficiency compared to full virtualization.
6.  **Operating system-level virtualization:** Operating system-level virtualization, also known as containerization, involves partitioning a single operating system instance into multiple isolated containers, each with its own set of resources and services.
7.  **Application virtualization:** Application virtualization involves encapsulating an application and its dependencies into a virtual package that can be run on any system without the need for installation or configuration.

| Type of Virtualization | Description |
| --- | --- |
| Emulation or Simulation | Creating a virtual environment that mimics the behavior of another system or hardware |
| Native virtualization and full virtualization | Running the hypervisor directly on the physical hardware to emulate a complete hardware environment, allowing multiple operating systems to run on a single physical server |
| Hardware-enabled virtualization | Using hardware support for virtualization, such as Intel VT-x or AMD-V, to improve the performance and efficiency of virtualization |
| Partial virtualization | Virtualizing only specific hardware components, such as CPU or memory, rather than emulating the entire hardware environment |
| Paravirtualization | Modifying the guest operating system to work in a virtualized environment, allowing for better performance and efficiency compared to full virtualization |
| Operating system-level virtualization | Partitioning a single operating system instance into multiple isolated containers, each with its own set of resources and services |
| Application virtualization | Encapsulating an application and its dependencies into a virtual package that can be run on any system without the need for installation or configuration |

| Type of Virtualization | Description | Example | Pros | Cons |
| --- | --- | --- | --- | --- |
| Emulation/Simulation | Emulates hardware or software components to allow execution of code that would not otherwise be possible on a given system. | Wine (emulates Windows API on Linux) | Enables running legacy software or software for different platforms. | Can be slow and inefficient. |
| Native Virtualization | A hypervisor runs on the host OS to create and manage virtual machines. Guest OSs are installed on the virtual machines. | Oracle VirtualBox | High performance, isolation between virtual machines. | Requires significant overhead and resource allocation. |
| Full Virtualization | A hypervisor runs directly on the host's hardware to create and manage virtual machines. Guest OSs are installed on the virtual machines. | VMware ESXi | High performance, high level of isolation and security. | Requires significant overhead and resource allocation. |
| Hardware-Enabled Virtualization | A feature of modern CPUs that allows for more efficient virtualization by offloading some virtualization tasks to hardware. | Intel VT-x or AMD-V | Higher performance, less overhead. | Requires modern CPUs and virtualization support in BIOS. |
| Partial Virtualization | Allows multiple instances of an OS to share the same kernel, but with separate user spaces. | LXC (Linux Containers) | Lightweight and efficient, better performance than full virtualization. | Limited isolation between instances, cannot run different OSs. |
| Paravirtualization | Requires the guest OS to be modified to run on a virtualized environment. | Xen | High performance, lower overhead compared to full virtualization. | Requires guest OS modification, less flexibility. |
| Operating System-Level Virtualization | Allows multiple instances of an OS to share the same kernel and resources. | Docker | Lightweight, efficient, and highly scalable. | Limited isolation between instances, cannot run different OSs. |
| Application Virtualization | Virtualizes applications rather than entire operating systems. | Citrix XenApp | Allows for centralized management and delivery of applications. | Limited flexibility in terms of OS and hardware. |


## Virtualization in cloud
 - Virtualization is a key component of cloud computing
 - Cloud providers use virtualization to create virtual machines and virtual networks to deliver cloud services. 
 - By virtualizing physical servers, storage devices, and networks, cloud providers can create pools of resources that can be dynamically allocated and scaled based on the needs of users or applications.

### Benefits:
1.  **Resource utilization**: Virtualization allows cloud providers to make better use of their physical resources by running multiple virtual instances on a single server.
2.  **Flexibility**: Virtualization allows cloud providers to create virtual machines with different configurations and capacities to meet the specific needs of their customers.
3.  **Scalability**: Cloud providers can quickly and easily add or remove virtual machines as demand for services changes.
4.  Isolation: Virtualization provides a level of isolation between virtual machines, which improves security and reduces the risk of system failures.
5.  **Disaster recovery:** Virtualization makes it easier to replicate virtual machines and move them between physical servers, which can improve disaster recovery capabilities.

### Disadvantages:
1.  **Complexity:** Virtualization can add an additional layer of complexity to a cloud computing environment, which can increase the potential for configuration errors, security vulnerabilities, and performance issues.
2.  **Overhead:** Virtualization can consume additional system resources, such as CPU cycles and memory, which can result in decreased performance for certain workloads.
3.  Single point of failure: If the hypervisor or underlying hardware fails, all of the virtual machines that are running on that system may also fail, leading to potential downtime or data loss.
4.  **License compliance:** Running multiple instances of an operating system or application on a single physical server may violate software licensing agreements, which can lead to legal and financial issues.
5.  **Security:** Virtualization can increase the attack surface of a cloud computing environment, and it may be more difficult to secure multiple virtual instances than a single physical server.