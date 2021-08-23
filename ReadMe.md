If there is an error like -- Error: Package: jenkins-2.307-1.1.noarch (jenkins)
Run below two commands to resolve the above ERROR
1- amazon-linux-extras install epel -y
2- yum update -y
and then below commands 
yum install jenkins
systemctl status jenkins
systemctl start jenkins
systemctl status jenkins


** tail -3 /etc/profile
export JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.302.b08-0.amzn2.0.1.x86_64
export PATH=$JAVA_HOME/bin:$PATH
export MAVEN_HOME=/usr/share/maven
**

[root@ip-172-31-* ec2-user]# echo $JAVA_HOME
/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.302.b08-0.amzn2.0.1.x86_64
[root@ip-172-31-* ec2-user]# echo $MAVEN_HOME
/usr/share/maven
