## Before You Begin

- Before you launch the automated deployment on cloud, verify the prerequisites.
- The image has a 30 day evaluation period license.

## License Key Prerequisite

- Verify that you have a license to deploy Global IDs Data Ecosystem Management Suite.
- BYOL URL:- https://www.globalids.com/contact-us

## AWS Subscription

- Users should have an active subscription with the ability to launch instances from AWS marketplace.

## Note:- The software will start automatically at start up.

- You can check the software status by executing the script checkServices.sh from the Server location (/home/<username>/server/).
- All components should be in running state.

## To Start the Software Server Manually

- Log in into the linux instance

- Change directory to `/home/<username>/server`

- Run the script `run.sh` by entering the command

```
$ ./run.sh -dv –h:2 &
```

- Wait till the message "Server started successfully" is displayed on the screen.

- Server startup options -h:n [n=Number of habitats] -dv [Disable verification].

## Stop the Software Server

- Log in into the linux instance as a ec2-user

- Change directory to `/home/<username>/server`

- Run the script `stop.sh` by entering the command

```
$ ./stop.sh -k
```

- Server shutdown options -k : This stops the server immediately. All the tasks that are running at that point get terminated.

## Access the Software

Navigate to URL http://<Public_DNS>:45450/new (Recommended to use Google Chrome)

To get the login credentials please communicate with support@globalids.com


