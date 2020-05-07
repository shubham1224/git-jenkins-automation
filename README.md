# Setup to integrate github and jenkins

*creating multiple jobs in jenkins to automate the thing.*

## job1 : deploy_dev1

    when developer commit the code in local repo from dev1 branch it automatically goes to github dev1 branch.
    job1 keep monitoring the github dev1 branch every minute,if new commit found ,it deploy the page in testing system 

![](Images/img9.jpg)

![](Images/img10.jpg)

![](Images/img1.jpg)

to test use ip of system along with following port.
![](Images/img4.jpg)

## job2 : merge_branch

    If testing  code is certified/approved, then this job is build 
    It goes to github and merge the dev1 branch with master

![](Images/img5.jpg)
![](Images/img2.jpg) 
     
## job3 : deploy_master

    If job2 runs successfully ,this job is triggered
    It deployes the webpage from master branch into production system using docker image.

![](Images/img6.jpg)
![](Images/img7.jpg)
![](Images/img8.jpg)

to test use ip of system along with following port.

![](Images/img3.jpg)     



       


 
