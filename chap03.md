# 6. Process

`ps`		Report a snapshot of the current processes.

`top`		Display system tasks

`kill`		Send a signal to a process

`killall`

`nice`/`renice`	Run a program with modified scheduling priority

`time`		Time a simple command or give resource usage

`uptime`	System Load Average

`bg` 	Place jobspec into the background, as if it had been started with `&'. If jobspec is not supplied, the current job is used.

`fg` 	Bring jobspec into the foreground and make it the current job. If jobspec is not supplied, the current job is used.

`jobs`	The first form lists the active jobs. The -l option lists process IDs in addition to the normal information; the -p option lists only the process ID of the job's process group leader. The -n option displays only jobs that have changed status since last notfied. If jobspec is given, output is restricted to information about that job. If jobspec is not supplied, the status of all jobs is listed.

`suspend`	Suspend the execution of this shell until it receives a SIGCONT signal. The -f option means to suspend even if the shell is a login shell.
When job control is active, the kill and wait builtins also accept jobspec arguments.

`screen`	http://www.ibm.com/developerworks/aix/library/au-gnu_screen/