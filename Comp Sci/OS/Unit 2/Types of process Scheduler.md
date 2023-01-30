### process Scheduling
[[process]] scheduling is responsible for selecting a process based on scheduling method as well as removing a running process.
It's very important component of a multiprogramming OS

### what is process scheduler
[[process]] scheduler is a program that manages and schedules processes, based
on given scheduling algorithm
The scheduler's purpose is to implement the virtual machine so that each [[process]] appears to be running on its own computer to the user.

![[Pasted image 20230126151552.png]]

### Types of process Schedulers
1. Long-term Scheduler or Job Scheduler: 
	Long-term scheduler selects processes from the pool (or secondary memory) and then
	mentains them in the primary memory's ready queue.
	The degree of multiprogramming is mostly controlled by the Long-Term scheduler.
	The goal of the long term scheduler is to select the best mix of IO and CPU bound processes from the job pool.
	If the scheduler selects more IO bound processes, all of the jobs may become stuck, the CPU will be idle for the mejority of the time and thus the multiprogramming will be reduced. Hence Long-term scheduler has huge impact on the system.

2. Short-term Scheduler or CPU scheduler

	![[Pasted image 20230126152420.png|500]]
	Short-term scheduler selects a job from the ready queue to then send to CPU for execution.
	To determine which job will be dispatched for execution, a scheduling method is utilized.
	The short-term scheduler's job is crutial in a sence that if it picks a job with large burst-time, all the subsequent jobs in the ready queue will have to wait in ready queue for a long period. This is known as hunger.

3. Medium-term Scheduler

	![[Pasted image 20230126153053.png|450]]
	The switched-out processes are handled by the Medium-term scheduler.
	If a running [[process]] is required some IO time to complete, then it's state must be changed from `running` to `waiting`.
	This is done by Medium-term scheduler, it stops the running processes to make space for other processes.