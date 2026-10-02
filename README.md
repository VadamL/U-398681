How to reproduce:
Open Reg572 in UE 5.7.2
Open Reg581 in UE 5.8.3 (Originally was 5.8.1) either works
After opening the project you should be in TestLevel map which is set as editor and game entry map
Inspect level blueprint:
Start/Play map
Press "J" to spawn actors (50k +- actors should take a few seconds which is expected)
Press "K" to force GC via load map node
Do this in editor and packaged test build with insights running to profile.
Since TestLevel is already set to game entry map, you should be able to just package the project into test build right away. 
