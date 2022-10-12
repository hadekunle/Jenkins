
Ensure that your software packages are up to date on your instance by uing the following command to perform a quick software update:

```
sudo yum update –y

```

Add the Jenkins repo using the following command:
```
sudo wget -O /etc/yum.repos.d/jenkins.repo \

```

Import a key file from Jenkins-CI to enable installation from the package:
```
sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key

```


```
sudo yum upgrade

```

Install Java
```
sudo amazon-linux-extras install java-openjdk11 -y

```

Install Jenkins
```
sudo yum install jenkins -y
```