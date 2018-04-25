# Install Apache Flume
The following instruction is based on this link https://www.tutorialspoint.com/apache_flume/apache_flume_environment.htm
1. Go to https://flume.apache.org/download.html and download a flume. Note that the link below may be different as it depends on the mirror that the download page directs to.
```
wget http://www-eu.apache.org/dist/flume/1.8.0/apache-flume-1.8.0-bin.tar.gz
```
2. Untar the file and move the extracted files to /opt/flume
```
tar -xzvf apache-flume-1.8.0-bin.tar.gz 
sudo mv apache-flume-1.8.0-bin /opt/flume
```
3. In the .bashrc file, set the home folder, the path, and the classpath for Flume as shown below.
```
export FLUME_HOME=/opt/flume
export PATH=$PATH:$FLUME_HOME/bin
export CLASSPATH=$CLASSPATH:$FLUME_HOME/lib/*
```
4. Make copies of these property files:
```
cp flume-conf.properties.template flume-conf.properties
cp flume-env.sh.template flume-env.sh
```
5. Verify the installation by running this command
```
flume-ng
```
You should see this output:
```
bigdata@ubuntu:~$ flume-ng
Error: Unknown or unspecified command ''

Usage: /opt/flume/bin/flume-ng <command> [options]...

commands:
  help                      display this help text
  agent                     run a Flume agent
  avro-client               run an avro Flume client
  version                   show Flume version info
```

