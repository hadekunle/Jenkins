

Installing Jenkins on EC2 server

Ensure that your software packages are up to date on your instance by uing the following command to perform a quick software update:

``` css
sudo yum update –y
```

Add the Jenkins repo using the following command:
```css
sudo wget -O /etc/yum.repos.d/jenkins.repo \
```

Import a key file from Jenkins-CI to enable installation from the package:
```css
sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key
```


```css
sudo yum upgrade
```

Install Java
```css
sudo amazon-linux-extras install java-openjdk11 -y
```

Install Jenkins
```css
sudo yum install jenkins -y
```

You can check the status of the Jenkins service using the command
```css
sudo systemctl status jenkins
```

Configure Jenkins [here](https://www.jenkins.io/doc/tutorials/tutorial-for-installing-jenkins-on-AWS/#configuring-jenkins)
