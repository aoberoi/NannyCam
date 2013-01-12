Nora:NannyCam ankur$ node_modules/.bin/awsbox create -n NannyCam
reading .awsbox.json
attempting to set up VM "NannyCam"
   ... VM launched, waiting for startup (should take about 20s)
   ... Instance ready, setting human readable name in aws
   ... name set, waiting for ssh access and configuring
   ... public url will be: http://54.242.184.2
   ... nope.  not yet.  retrying.
   ... nope.  not yet.  retrying.
   ... nope.  not yet.  retrying.
   ... nope.  not yet.  retrying.
   ... victory!  server is accessible and configured
   ... applying system updates
Loaded plugins: fastestmirror, priorities, security, update-motd, upgrade-helper
Loading mirror speeds from cached hostfile
 * amzn-main: packages.us-east-1.amazonaws.com
 * amzn-updates: packages.us-east-1.amazonaws.com
Cleaning repos: amzn-main amzn-updates
10 metadata files removed
6 sqlite files removed
0 metadata files removed
Loaded plugins: fastestmirror, priorities, security, update-motd, upgrade-helper
Loading mirror speeds from cached hostfile
 * amzn-main: packages.us-east-1.amazonaws.com
 * amzn-updates: packages.us-east-1.amazonaws.com
Setting up Update Process
No Packages marked for Update
   ... and your git remote is all set up
   ... configuring SSL behavior (enable)

Yay!  You have your very own deployment.  Here's the basics:

 1. deploy your code:  git push NannyCam HEAD:master
 2. visit your server on the web: http://54.242.184.2
 3. ssh in with sudo: ssh ec2-user@54.242.184.2
 4. ssh as the deployment user: ssh app@54.242.184.2

 Here are your server's details: {
    "instanceId": "i-51007420",
    "imageId": "ami-63850d0a",
    "instanceState": {
        "code": "16",
        "name": "running"
    },
    "dnsName": "ec2-54-242-184-2.compute-1.amazonaws.com",
    "keyName": "awsbox deploy key (a5f91854e23f3a158c2ef10a925711af)",
    "instanceType": "t1.micro",
    "ipAddress": "54.242.184.2",
    "launchTime": "2013-01-12T16:24:09.000Z",
    "name": "i-51007420"
}
