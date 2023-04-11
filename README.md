# 3A_15_Rafli-Alfian-Nilofar_Tugas4

| SystemCommandsOutput.scala |
| ------  |
| ```ruby
import sys.process._
val output = "hadoop fs -ls" !! // notice the �!!� operator
println("result = "+output) 
``` |
| ![image](https://user-images.githubusercontent.com/95726593/231009979-58557000-35b5-45b9-8cdc-a26407abba02.png)
![image](https://user-images.githubusercontent.com/95726593/231009999-eb536917-28fd-4405-97d1-df17f154a07f.png)
![image](https://user-images.githubusercontent.com/95726593/231010015-5bf5b19a-b28a-4cfa-bc73-8a4c1a0925c1.png)|

| SystemCommandsReturnCode.scala |
| ------  |
| import sys.process._
val res = "ls /tmp" ! // notice the �!� operator 
println("result = "+res) // result can be zero or non-zero |
| ![image](https://user-images.githubusercontent.com/95726593/231028674-4c5b7667-1c61-4377-a8d1-4206c710bd26.png)![image](https://user-images.githubusercontent.com/95726593/231028718-932c4486-685a-4ba5-93f3-5670e13d5629.png)|

| Accumulator.py |
| ------  |
| myaccum = sc.accumulator(0)
myrdd = sc.parallelize(range(1,100))
myrdd.foreach(lambda value: myaccum.add(value))
print myaccum.value|
| ![image](https://user-images.githubusercontent.com/95726593/231029612-a6d17169-7f64-4206-a6c1-3ea3dcffcbdd.png) |

| BroadCast.py |
| ------  |
| broadcastVar = sc.broadcast(list(range(1, 100)))
broadcastVar.value |
| ![image](https://user-images.githubusercontent.com/95726593/231029852-4b496b87-d352-4fe8-81e4-19ff6cc6bd73.png) |

| PairRDD.py |
| ------  |
| mylist = ["my", "pair", "rdd"]
myRDD = sc.parallelize(mylist)
myPairRDD = myRDD.map(lambda s: (s, len(s)))
myPairRDD.collect()
#[('my', 2), ('pair', 4), ('rdd', 3)]
myPairRDD.keys().collect()
#['my', 'pair', 'rdd']
myPairRDD.values().collect()
#[2, 4, 3] |
| ![image](https://user-images.githubusercontent.com/95726593/231030025-78df7a0b-8e2c-46c1-937e-50b27b65ed0d.png) |

| LogAnalytics.py |
| ------  |
| import sys
from operator import  add
from pyspark import SparkContext
#Check for number of inputs passed from command line
if __name__ == "__main__":
if len(sys.argv) != 2:
print >> sys.stderr, "Usage: access_log.py <file>"
exit(-1)
#Intialize the Spark Context with app name
sc = SparkContext(appName="Log Analytics")
#Get the lines from the textfile, create 4 partitions
access_log = sc.textFile(sys.argv[1], 4)
#Filter Lines with ERROR only
error_log = access_log.filter(lambda x: "ERROR" in x)
#Cache error log in memory
cached_log = error_log.cache()
#Now perform an action -  count
print �Total number of error records are %s� % (cached_log.count())
#Now find the number of lines with 
print �Number of product pages visited that have Errors is %s� % (cached_log.filter(lambda x: �product� in x).count()) |
| ![image](https://user-images.githubusercontent.com/95726593/231031238-98ec6b4f-c7b4-41e7-ba46-1989a3b1aad3.png) |
