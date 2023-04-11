# 3A_15_Rafli-Alfian-Nilofar_Tugas4

| SystemCommandsOutput.scala |
| ------  |
| import sys.process._
val output = "hadoop fs -ls" !! // notice the �!!� operator
println("result = "+output)  |
| ![image](https://user-images.githubusercontent.com/95726593/231009979-58557000-35b5-45b9-8cdc-a26407abba02.png)
![image](https://user-images.githubusercontent.com/95726593/231009999-eb536917-28fd-4405-97d1-df17f154a07f.png)
![image](https://user-images.githubusercontent.com/95726593/231010015-5bf5b19a-b28a-4cfa-bc73-8a4c1a0925c1.png)|


| SystemCommandsReturnCode.scala |
| ------  |
| import sys.process._
val res = "ls /tmp" ! // notice the �!� operator 
println("result = "+res) // result can be zero or non-zero |
| ![image](https://user-images.githubusercontent.com/95726593/231028674-4c5b7667-1c61-4377-a8d1-4206c710bd26.png)![image](https://user-images.githubusercontent.com/95726593/231028718-932c4486-685a-4ba5-93f3-5670e13d5629.png)|
