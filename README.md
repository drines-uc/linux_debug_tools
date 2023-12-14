# Linux Debugging Tools

## netstat
netstat is a networks statistics tool, it helps you answer questions like
Is my service listening?
Is a connection established?
Is the port right?

List all the tcp ports that are running

```netstat -at```

List all the udp ports that are running

```netstat -au```

List all the unix socket i-nodes that are running

```netstat -ax```

List all the tcp ports that services are listening on

```netstat -lt```

List all the udp port that services are listening on

```netstat -lu```

List all the unix socket i-nodes that services are listening on

```netstat -lx```

## strace
strace is a tool to trace system calls and signals, it helps you answer questions like
Is my service stuck?
What is my service doing?
Is there a race condition?

Watch the stack trace of a process

```sudo strace -p <pid>```


## tcpdump
tcpdump is a tool to capture network packets so they can be analyzed with wireshark it can be used to answer questions like
Why is my app not connecting?
Why do my connections keep resetting?

```tcpdump -i <interface> -s 65535 -w test.pcap```


## ip
ip is a tool to show and manipulate routing device and local network policy, it helps answer questions like
What is my network interface?

List all the interfaces that have a link

```ip link show```

List all the ip addresses use on my machine

```ip addr show```

## ps
ps is a tool that lets you inspect the current running processes on your local system, it helps answer questions like
What other processes did that app start
Did my app die?

```ps -ef | grep <>```

## lsof
lsof is a tool to list open files, it helps answer questions like
What files is a process using?
What process is using this file?
What files does s user have open?

Show the processes that are using a particular file or directory

```lsof <file/directory>```

Show the files being used by a particular process

```lsof -p <pid>```

Show the files currently opened by a user

```lsof -u <user>```




