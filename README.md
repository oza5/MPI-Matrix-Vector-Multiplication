##PROJECT DOCUMENTATION


# V-MM.py:
The code can be run using the following command:


$mpirun -n 4 python test.py

-argument following '-n' is a integerthat defines the number of parallel processors to run the code logic on.
-prints out thr runnig time of each node
-code consists of comments.


# StarCluster and Mpich2 Configurations:
Following are the configurations that the StarCluster on our EC2 instance is running on. These values can be changed in the ".starcluster/Config" file under [aws info]:

###########
[aws info]
AWS_ACCESS_KEY_ID =#your_aws_access_key_id
AWS_SECRET_ACCESS_KEY = #your_secret_access_key
AWS_USER_ID=#your userid

[key mykey]
KEY_LOCATION=~/.ssh/mykey.rsa

[cluster smallcluster]
KEYNAME = mykey
CLUSTER_SIZE = 8
CLUSTER_USER = sgeadmin
CLUSTER_SHELL = bash
NODE_IMAGE_ID = ami-3393a45a
NODE_INSTANCE_TYPE = t1.micro
MASTER_INSTANCE_TYPE = t1.micro
PLUGINS = mpich2
##########







