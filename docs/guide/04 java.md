# Install Java JDK
The following instruction is based on this link https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-get-on-ubuntu-16-04. As of this writing, the version installed is OpenJDK 8. Install JDK instead of JRE to have jps utility.
1. Update the package index
```
sudo apt-get update
```
2. Install the Java Runtime Environment (JDK)
```
sudo apt-get install default-jdk
```
3. Setting the JAVA_HOME Environment Variable
4. To set this environment variable, we will first need to find out where Java is installed. You can do this by executing the same command as in the previous section:
```
sudo update-alternatives --config java
```
5. Copy the path and then open /etc/environment
```
sudo vi /etc/environment
```
6. At the end of this file, add the following line, making sure to replace the highlighted path with your own copied path.
```
JAVA_HOME="/usr/lib/jvm/java-8-openjdk-amd64"
```
7. Save and exit the file and reload it.
```
source /etc/environment
```
8. You can now test whether the environment variable has been set by executing the following command:
```
echo $JAVA_HOME
```