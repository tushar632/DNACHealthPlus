# DNACHealth+

# About the Tool
DNAC Health+ is a tool to aid with performing crucial monitoring operations on DNA Appliance(s) in standalone/cluster. It is an interactive platform that allows the user to capture the logs, status of health checks, without having to login to the CLI of DNAC.The tool has provision to perform the overall health check at a given instant or schedule checks on a four hourly,daily or weekly basis. Thereby, making the process of log collection and health check easier as well as aiding with early detection of issues. It also helps stay alert and understand the need to fix health parameters before an issue occurrence. Eventually, this results in making the whole experience of troubleshooting enhanced.

# Pre-requisites
1.	To run the application exe, the platform must be a Windows 64-bit. 
2.	The user must hold the Windows administrator account.
3.	The system must have a browser (preferably Firefox or Chrome) installed for GUI access to app. 
4.	Reachability to DNAC and admin access to DNA.
5.  Ensure that there are no active instances of the app.exe on the task manager before running a fresh instance of the app.

# How to Run the application
1. Download and run the app.exe. The app runs at 127.0.0.1 port 5000
2. On the pop up browser window enter all the details relevant to the DNAC cluster(Cli & Gui credentials, Port , Cluster mode, Appliance IP )
3. On successfull login, select from the options available.
  
   i.  Disk space utilization: verifies and reports the status of the file systems mounted on the disk
  
   ii. Health Check : Performs all the checks on the cluster whenever the run button is clicked. Also displays the result of most recent Health check
  
   iii. Four Hourly health check : Allows the user to schedule checks every four hours starting fromt the configured time.
  
    iv.  Daily Health check : Allows the user to schedule checks every day starting fromt the configured time.
  
    v.   Weekly Health Check : Allows the user to schedule checks on a weekly basis starting fromt the configured time
  
    vi. Raise a TAC case: Provides the use with a link to open a new TAC case
    
    vii. Configure email : Allows the user to configure the smtp settings, once configured automated emails will be sent with the relevant summary file.
 
4. Download: Users can download the relevant log files and the excel summary file by clicking on the download button on top right of the window.


# Checks run 4 hourly
VIP Reachability

CPU Load

Rabbitmq Cluster Health

Rabbitmq Cluster Status

Rabbitmq Queue Status

Zookeeper Cluster Health

Zookeeper Cluster Status

# Checks run daily
Docker Status

Kubelet Status
 
Appstack Status

Appstack Service Restart 

Kubelet Node Status

Magctl Node Status

ETCD Cluster Health

Certification Validity

Backup Server

Catalog Server

Docker Stopped Container

Mongo DB Check

Postgres Cluster

Glusterfs

InfluxDB

ISE Check

Disk Space Utilization

Memory Utilization

PS AUX

DNS Reachability

# Checks run weekly
NTP Sync Offset

Interface Status





