


We begin with an NMAP scan of the target IP.

![[1.png]]

We discover that a Telnet service is open, on port 23. Let's investigate.

![[2.png]]

Connecting to the service prompts us for a login.

![[3.png]]

Login Root with no passwords works. 

![[4.png]]

Once in, we LS, find flag.txt, and cat it.
