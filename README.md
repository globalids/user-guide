## Start the Software Server

- Log in into the linux instance as a ec2-user

- Change directory to `/home/ec2-user/server`

- Run the script `run.sh` by entering the command

```
$ ./run.sh -dv –h:2 &
```

- Wait till the message "Server started successfully" is displayed on the screen.

- Server startup options -h:n [n=Number of habitats] -dv [Disable verification].

## Stop the Software Server

- Log in into the linux instance as a ec2-user

- Change directory to `/home/ec2-user/server`

- Run the script `stop.sh` by entering the command

```
$ ./stop.sh -k
```

- Server shutdown options -k : This stops the server immediately. All the tasks that are running at that point get terminated.

## Access the Software

Navigate to URL http://<Public_DNS>:45450/new (Recommended to use Google Chrome)

To get the login credentials please communicate with support@globalids.com


