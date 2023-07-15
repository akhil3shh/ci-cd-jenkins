# Jenkins CI/CD pipeline

# Major steps to follow:  
1. Create an AWS EC2 instance, install JDK (v11 in this demo), configure and install Jenkins.  
2. Expose jenkins to port 8080 of the instance and make it accessible by editing the inbound rules.  
3. Create a Dockerfile using node-alpine as the parent image, copy all the source files and expose this to port 8000.  
4. Back to Jenkins, configure the job by adding the build steps; enable GitHub hook trigger for GITScm polling and configuring GitHub by adding a webhook for automatic job scheduling if a trigger is detected.  
5. Finally, to check everything is working as expected head towards http://*ip-address-of-your-aws-instance*:8000 !
