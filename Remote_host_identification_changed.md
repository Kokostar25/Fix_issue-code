# HOW TO FIX WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!
- RUN ssh-keygen -R "you server hostname or ip"
## The Ip you use here is the one on the .ssh/known_hosts in my case it was the EC2 Ip add
## You get this 'Host xx.xx.xx.xx found: line 84'
## /Users/me/.ssh/known_hosts updated.
## Original contents retained as /Users/me/.ssh/known_hosts.old
## Now go to folder where you stored the pem key
- Run ssh -i "yourkey.pem" ubuntu@ec2-xx.xx.xx.xx.compute-1.amazonaws.com
