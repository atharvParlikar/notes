Ok so there are 3 main types of operating systems
1. monolithic
2. layerd
3. micro-kernal

### Monolithic

my version: monolithic kernal basically means that every fricking shit is handeld by kernal everything from file systems, network, memory, process, drivers everything.

book defination: A monolithic kernel is a type of operating system kernel that contains all the necessary kernel components within a single, unified executable image. In a monolithic kernel design, the entire operating system runs in kernel space, meaning that all system services and device drivers are executed in privileged mode, with direct access to the hardware. This allows the kernel to have a high degree of control over the system and to provide a wide range of services to user-level programs. However, it also means that the kernel is large and complex, and can be more prone to errors and security vulnerabilities. Monolithic kernels are typically used in traditional, general-purpose operating systems such as Linux, Windows, and macOS.

digram:

<img src="https://scaler.com/topics/images/operating-system-structure-image2.webp" height="550">

### Layered Approach
my version: It's like an onion where every layer have some job the deeper you go more
the low level stuff. every layer talks with each other to get stuff done, having all these
layers also makes it VERY modular, now ofcourse that comes at a cost all this
communication can make the os slower.

real defination: A layered kernel is a type of operating system kernel that is structured as a set of interconnected layers, each of which provides a particular set of functions or services. In a layered kernel design, the operating system is divided into a series of discrete layers, each of which has a specific role and communicates with the others through a well-defined interface. This modular approach allows different parts of the kernel to be developed, tested, and maintained independently, and makes it easier to add new features or support for new hardware. However, it also means that the kernel may be less efficient, as there is overhead associated with the communication between layers. Layered kernels are typically used in specialized, real-time or embedded operating systems that require a high degree of modularity and flexibility.

<img src="https://static.javatpoint.com/operating-system/images/layered-structure-of-operating-system.png" height="300">

### Microkernal
Microkernal is a kernal that is near-minumun meaning it implements only the necessary
things that makes up an operating system such as Inter-Process communication,
address space management, thread management.
Everything else such as device drivers, file system management is under user space, doing
this makes the kernal easy to understand and debug.
These userspace services are called servers.

here are some pros and cons of microkernal architecture:
##### pros
-   Smaller size: Because a microkernel only includes the bare minimum necessary to run an operating system, it is generally much smaller in size than a monolithic kernel. This can make it easier to debug and maintain, and can also reduce the attack surface for security vulnerabilities.
-   More modular: Because a microkernel separates the core operating system functions from other services, it is more modular and flexible. This makes it easier to add or remove features, and to write custom implementations of certain services.
-   Better fault isolation: Because each service in a microkernel operates in its own address space, a fault in one service is less likely to affect the stability of the entire system. This can make it easier to diagnose and fix problems, and can also improve the overall reliability of the operating system.

#### cons
-   Slower performance: Because a microkernel relies on message passing between the kernel and user-space servers, it can be slower than a monolithic kernel, which can execute all functions directly within the kernel.
-   More complex: Because a microkernel requires multiple servers to implement the various features of an operating system, it can be more complex to set up and maintain than a monolithic kernel.
-   Limited support: Because microkernels are less common than monolithic kernels, they may have less support from developers and a smaller ecosystem of available tools and software.