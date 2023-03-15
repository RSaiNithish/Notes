
### Parallel computing vs distributed computing
| Feature      | Parallel Computing  | Distributed Computing |
|--------------|---------------------|------------------------|
| Definition   | Simultaneously processing a single task using multiple processors | Processing multiple independent tasks across multiple processors or computers |
| Data Sharing | High degree of data sharing among processors | Data sharing between processors or computers is limited |
| Communication | High-speed communication between processors | Communication between processors or computers can be slower due to network latency |
| Hardware      | Specialized hardware required | Standard hardware can be used |
| Complexity   | Lower complexity as all processors work towards a single task | Higher complexity as multiple tasks must be coordinated and managed |
| Scalability  | Limited by the number of processors | Highly scalable as more processors or computers can be added |
| Examples     | Rendering a 3D animation, matrix multiplication | Large scale data processing, web applications |

### Hardware architecture of parallel processing
| Architecture   | SISD                           | SIMD                                       | MISD                                       | MIMD                                              |
|----------------|--------------------------------|--------------------------------------------|--------------------------------------------|--------------------------------------------------|
| Definition      | Single Instruction Single Data | Single Instruction Multiple Data | Multiple Instruction Single Data | Multiple Instruction Multiple Data |
| Example         | Traditional CPU                | Graphics Processing Units (GPUs) | Redundant Systems | Cluster of computers                               |
| Data flow       | Sequential                     | Parallel                                  | Parallel                                  | Parallel                                           |
| Instruction flow | Sequential                     | Single instruction is broadcast to all processing units | Multiple instructions are broadcast to all processing units | Multiple instructions can be executed simultaneously |
| Hardware        | Single processor               | Multiple processing units with shared memory | Multiple processing units with separate memory | Multiple processors with separate memory           |
| Synchronization | No synchronization required   | Synchronization required for data consistency | Synchronization required for data consistency | Synchronization required for data consistency     |
| Advantages      | Simple architecture            | High throughput and parallelism             | Fault tolerance                             | High throughput and parallelism                    |
| Disadvantages   | Limited performance            | Limited flexibility and difficult programming | Limited practical applications | Complex architecture and difficult programming     |

### Approaches to Parallel Processing
 - Data parallelism
 - Process parallelism
 - Farmer and worker model

#### Levels of parallelism
1.  Instruction-level parallelism (ILP): This level of parallelism is achieved by executing multiple instructions from a single program simultaneously. This can be done by exploiting the dependencies between instructions and executing them in a different order or by using multiple execution units within a processor.
2.  Thread-level parallelism (TLP): This level of parallelism is achieved by executing multiple threads of execution simultaneously. Threads are independent sequences of instructions that can be executed in parallel on multiple processors or processor cores.
3.  Data-level parallelism (DLP): This level of parallelism is achieved by dividing a large data set into smaller pieces and processing them in parallel. This can be done by using vector processing or by dividing the data among multiple processors.
4.  Task-level parallelism (TAP): This level of parallelism is achieved by dividing a large task into smaller tasks that can be executed in parallel. This can be done by using a parallel programming model, such as OpenMP or MPI, to distribute the work among multiple processors.
5.  System-level parallelism: This level of parallelism is achieved by using multiple computers or nodes in a distributed system to perform a single task. This can be done by using message passing or shared memory mechanisms to communicate between nodes.

## Distributed computing
Distributed computing refers to a computing model in which a group of interconnected computers work together to perform a single task.
1.  Multiple computers: Distributed computing involves multiple computers or nodes working together to perform a task. These nodes can be located in different physical locations and can have different hardware specifications.
    
2.  Communication: Communication is a key aspect of distributed computing. The nodes must be able to communicate with each other to exchange data and coordinate their activities.
    
3.  Shared resources: Distributed computing allows for the sharing of resources such as processing power, memory, and storage. This allows for larger and more complex tasks to be performed than would be possible on a single computer.
    
4.  Fault tolerance: Distributed computing systems are designed to be fault-tolerant, meaning that if one or more nodes fail, the system can still function and complete the task.
    
5.  Scalability: Distributed computing systems can be scaled up or down depending on the needs of the task. Additional nodes can be added to increase processing power, or nodes can be removed when they are no longer needed.
    
6.  Coordination: Distributed computing systems require a way to coordinate the activities of the different nodes. This is typically done using a distributed algorithm or protocol that specifies how the nodes should work together.
    
7.  Security: Distributed computing systems must be designed with security in mind, as data is being exchanged between nodes and can be vulnerable to attack.

#### Distributed computing stack 
1.  Hardware layer: This layer includes the physical devices that make up the distributed system, such as servers, storage devices, and networking equipment.
2.  Operating system layer: This layer includes the software that manages the hardware resources of each node in the system, such as the Linux operating system.
3.  Middleware layer: This layer provides a set of software services that sit between the application layer and the operating system layer. Examples of middleware include message queues, data caching, and distributed file systems.
4.  Application layer: This layer includes the software applications that run on the distributed system, such as web servers, databases, and custom business applications.
5.  User layer: This layer includes the end-users who interact with the applications running on the distributed system, typically through a web browser or other client software.

