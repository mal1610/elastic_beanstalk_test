# Steps to create the new version package bundle
Pre-requisites: Download the sample python package [here](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/GettingStarted.DeployApp.html) into a project folder 

## Instructions
1. In the project folder, access the terminal and run the following commands 
``` 
~/myapp$ unzip python.zip

~/myapp$ nano application.py
```
2. Navigate to the part of the code below and make the required changes
``` html
<body id="sample">
  <div class="textColumn">
    <h1>Sample app in application development by [YOURNAME]</h1>
    <p>Your first AWS Elastic Beanstalk Python Application is now running on your own dedicated environment in the AWS Cloud</p>
    <p>This environment is launched with Elastic Beanstalk Python Platform</p>
  </div>
```
3. Press Ctrl + X once changes are made and enter 'Y' and 'Enter'
4. Run the following commands in the terminal
```
~/myapp$ zip myapp.zip -r * .[^.]*
```
5. Upload the myapp.zip file to Elastic Beanstalk, make a new version upload and select for deployment.
