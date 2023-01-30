A system call is a request made by a computer program to the kernal for specific services. system calls give user level programs access to the resources of the operating system.
system calls provide an Application Program Interface (API) through which user level programs can get OS services and API is the only means of communicating with the kernal.

## Services provided by sys calls
1. process creation and management
2. Main memory management
3. File Access, Directory and File system management
4. Device handling (I/O)
5. Protection
6. Networking, etc.

## Types of system calls
1. Process control: end, abort, create, terminate, allocate and free memory.
2. File management: create, open, close, delete, read file, write file, etc.
3. Device management
4. Information maintence
5. Communication

## Examples

#### Process Control
CreateProcess()  
ExitProcess()  
WaitForSingleObject()
fork()  
exit()  
wait()

#### File Manipulation
CreateFile()  
ReadFile()  
WriteFile()  
CloseHandle()
open()  
read()  
write()  
close()

#### Device Manipulation
SetConsoleMode()  
ReadConsole()  
WriteConsole()
ioctl()  
read()  
write()

#### Information Maintenance
GetCurrentProcessID()  
SetTimer()  
Sleep()
getpid()  
alarm()  
sleep()

#### Communication
CreatePipe()  
CreateFileMapping()  
MapViewOfFile()
pipe()  
shmget()  
mmap()

#### Protection
SetFileSecurity()  
InitlializeSecurityDescriptor()  
SetSecurityDescriptorGroup()
chmod()  
umask()  
chown()