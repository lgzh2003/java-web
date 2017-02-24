##Install Maven on Ubuntu
     
###1.Search Maven package
In a terminal, run **apt-cache search maven**, to get all the available Maven package.             
```
$ apt-cache search maven
....
libxmlbeans-maven-plugin-java-doc - Documentation for Maven XMLBeans Plugin
maven - Java software project management and comprehension tool
maven-debian-helper - Helper tools for building Debian packages with Maven
maven2 - Java software project management and comprehension tool
```         
            
###2.Install Maven
Run command **sudo apt-get install maven**, to install the latest Apache Maven.                
```
$ sudo apt-get install maven
```      
          
###3.Verification
Run command **mvn -version** to verify your installation.                             
```
$ mvn -version
Apache Maven 3.0.4
Maven home: /usr/share/maven
Java version: 1.7.0_09, vendor: Oracle Corporation
Java home: /usr/lib/jvm/java-7-openjdk-amd64/jre
Default locale: en_US, platform encoding: UTF-8
OS name: "linux", version: "3.5.0-17-generic", arch: "amd64", family: "unix"
```             
                                                    
Where is Maven installed?                  
The command apt-get install the Maven in /usr/share/maven.                      
```
$ls -ls /usr/share/maven
total 16
4 drwxr-xr-x 2 root root 4096 Dec  7 01:28 bin
4 drwxr-xr-x 2 root root 4096 Dec  7 01:28 boot
0 lrwxrwxrwx 1 root root   10 May 28  2012 conf -> /etc/maven
4 drwxr-xr-x 2 root root 4096 Dec  7 01:28 lib
4 drwxr-xr-x 2 root root 4096 Dec  7 01:28 man
```           
            
The Maven configuration files are stored in /etc/maven

$ls -ls /etc/maven              
```
total 16
 4 -rw-r--r-- 1 root root   184 Jan 21  2012 m2.conf
12 -rw-r--r-- 1 root root 10224 Jan 21  2012 settings.xml
```              
              
              
          



