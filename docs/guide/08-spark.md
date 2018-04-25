# Install Apache Spark
The following instruction is based on this link https://medium.com/@josemarcialportilla/installing-scala-and-spark-on-ubuntu-5665ee4b62b1
1. Go to https://spark.apache.org/downloads.html and download a pre-built for Hadoop 2.7 version of Spark (preferably Spark 2.0 or later). Then download the .tgz file. Note that the link below may be different as it depends on the mirror that the download page directs to.
```
wget http://www-eu.apache.org/dist/spark/spark-2.3.0/spark-2.3.0-bin-hadoop2.7.tgz
```
2. Untar the file and move the extracted files to /opt/spark
```
tar -xzvf spark-2.3.0-bin-hadoop2.7.tgz
sudo mv spark-2.3.0-bin-hadoop2.7 /opt/spark
```
3. Open the spark shell to verify the setup is successful.
```
cd /opt/spark/bin
./spark-shell
```
4. Test it with:
```
println(“Spark shell is running”)
```
5. Exit the shell
```
:q
```