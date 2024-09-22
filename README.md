# ci-cd-configurations-files  (successfully deploy codepipeline)

## Commands: We have used in Our Video

$ sudo apt update 

$ https://docs.aws.amazon.com/codedeploy/latest/userguide/resource-kit.html  # go to this link and copy "bucket name" and "Region identifier" and edit in below link 

$ wget https://Bucket-name.s3.Region-identifier.amazonaws.com/latest/install


##### Next up, we need to change the permission on the install file we will get after running the command above.

$ chmod +x ./install

##### Finally, to install the codedeploy-agent, run this command:

$ sudo ./install auto > /tmp/logfile

###### Here we are logging the output of the installation to the /tmp/logfile file. To check if the codedeploy-agent is running, enter this command:

$ sudo service codedeploy-agent status

###### If it is not running, enter this command to start the codedeploy-agent service:

$ sudo service codedeploy-agent status


