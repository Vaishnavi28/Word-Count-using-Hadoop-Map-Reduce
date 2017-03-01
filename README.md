# Word-Count-using-Hadoop-Map-Reduce
Word Count is a common project that prevails in internet using many languages. I have tried to implement word count using Hadoop Map reduce
using HDFS system.

1.	Compiled the Java File:
javac -classpath /home/student4/hadoop-common-2.6.1.jar:/home/student4/hadoop-mapreduce-client-core-2.6.1.jar:/home/student4/commons-cli-2.0.jar WordCount2.java

2.	Created the JAR file:
jar -cvf WordCount2.jar WordCount*.class

3.	Copied input file from local to HDFS system:
hdfs dfs -copyFromLocal wordcountsample.txt /home/wb9452/input/

4.	Executed the jar file:
hadoop jar /home/student4/WordCount2.jar WordCount2 hdfs:///home/wb9452/input/wordcountsample.txt hdfs:///home/wb9452/output10
