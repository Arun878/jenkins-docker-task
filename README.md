# jenkins-docker-task

### The Task was:

#### 1.	Create container image that’s has Jenkins installed  using dockerfile 

#### 2.	When we launch this image, it should automatically starts Jenkins service in the container.

#### 3.	Create a job chain of job1, job2, job3 and  job4 using build pipeline plugin in Jenkins 

#### 4.	 Job1 : Pull  the Github repo automatically when some developers push repo to Github.

#### 5.	 Job2 : By looking at the code or program file, Jenkins should automatically start the respective language interpreter install image container to deploy code ( eg. If code is of  PHP, then Jenkins should start the container that has PHP already installed ).

#### 6.	Job3 : Test your app if it  is working or not.

#### 7.	Job4 : if app is not working , then send email to developer with error messages.

#### 8.	Create One extra job job5 for monitor : If container where app is running. fails due to any reson then this job should automatically start the container again.


### Creating the Dockerfile :
![Dockerfile](https://github.com/Arun878/images/blob/master/Screenshot%20(93).png)

### Now build the Dockerfile with this command:
`docker build --rm -t jenkins-ubuntu .`

### Now run the image using this command:
`docker run -it --privileged -p 8081:8080 -v /:/host jenkins-ubuntu`

### Creating JOB-1:
![JOB_1.1](https://github.com/Arun878/images/blob/master/Screenshot%20(94).png)
![JOB_1.2](https://github.com/Arun878/images/blob/master/Screenshot%20(95).png)

### Creating JOB-2:
![JOB_2.1](https://github.com/Arun878/images/blob/master/Screenshot%20(96).png)
![JOB_2.2](https://github.com/Arun878/images/blob/master/Screenshot%20(97).png)

### Creating JOB-3:
![JOB_3.1](https://github.com/Arun878/images/blob/master/Screenshot%20(98).png)

### Creating JOB-4:
![JOB_4.1](https://github.com/Arun878/images/blob/master/Screenshot%20(99).png)
![JOB_4.2](https://github.com/Arun878/images/blob/master/Screenshot%20(100).png)
![JOB_4.3](https://github.com/Arun878/images/blob/master/Screenshot%20(101).png)

### Creating JOB-5:
![JOB_5.1](https://github.com/Arun878/images/blob/master/Screenshot%20(102).png)

### This is Final Build Pipeline view:
![Final_View](https://github.com/Arun878/images/blob/master/Screenshot%20(103).png)
