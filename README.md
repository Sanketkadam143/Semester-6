# Semester-6
SPPU Computer TE-Sem 2 Assignments
Steps for WordCount Execution program

/* 

run daemons
$ start-all.sh
$ start-dfs.sh

Pass@123
*/

$ mkdir words

$ javac -classpath hadoop-core-1.2.1.jar words/WordCount.java

$ jar -cvf words.jar -C words/ .

$ hadoop fs -mkdir /words

$ hadoop fs -put fruits.txt /words

$ hadoop jar words.jar WordCount /words /output

~$ hadoop fs -ls /output

~$ hadoop fs -cat /output/part-r-00000

//replace output with any name
