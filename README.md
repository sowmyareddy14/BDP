Loading files into hadoop hdfs from local file system :
hdfs dfs -copyFromLocal localfile /hadooppath

Appending file to the first file :
hdfs dfs -appendToFile localfile /user/hadoop/hadoopfile

View the first lines in the merged file :
hdfs dfs -cat /hadoopfile | head -5

View the last lines in the merged file :
hdfs dfs -cat /hadoopfile | tail -5

Create a new text file and loading into hdfs and appending all three datasets :
hdfs dfs -cat /hadoopfiles | hdfs dfs -put /outputfile
