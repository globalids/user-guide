## Before You Begin

Before you launch the automated deployment on cloud, verify the prerequisites.

The running instance has a 30 day evaluation period.

## License Key Prerequisite

Verify that you have a license to deploy Global IDs Data Ecosystem Management Suite.

BYOL URL: [https://www.globalids.com/contact-us](https://www.globalids.com/contact-us)

## Subscription

Users should have an active cloud subscriptionwith the ability to launch instances from the image.

### Note: The software will start automatically at start up 

You can check the software status by executing the script checkServices.sh from the Server location `(/home/<username>/server/).`

All components should be in running state.

Check the process using the command ps -elf | grep Qai

Three processes will come as output in the console.

## To start the software server manually please follow the steps mentioned below

- Log in into the linux instance
- Change directory to /home/\&lt;username\&gt;/server
- Run the script run.sh by entering the command

```
$ ./run.sh -dv –h:2 &
```

- Wait till the message &quot;Server started successfully&quot; is displayed on the screen.
- Server startup options -h:n [n=Number of habitats] -dv [Disable verification].

  - Change directory to `/home/<username>/qai`

  - Go inside the directory `cd /value-store/app`
  - Run the script `run.sh` by entering the command. `./run.sh &`
  - Go inside the directory `cd /Server/app`
  - Run the script `run.sh` by entering the command. `./run.sh &`
  - Go inside the directory `cd /agent/app`
  - Run the script `run.sh` by entering the command. `./run.sh &`

## Access software UI

- Navigate to URL http://<Public\_DNS>:44373 (Recommended to use Google Chrome)
- To get the login credentials please communicate with support@globalids.com
