## To ssh into the ec2 without writing the whole command, we can add ec2 info in ssh config file.
### put the pem file in .ssh folder
### in that directory run `chmod 0400 your-server-identity.pem`
### Then add the info in the `~/.ssh/config` see below snippet for e.g,
```
Host my-server
  HostName 54.157.228.255
  User your-user-name
  IdentityFile ~/.ssh/your-server-identity.pem
  IdentitiesOnly yes
```

### Execute this command (`ssh my-server`), whenever you want to ssh into the ec2, 
