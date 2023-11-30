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
