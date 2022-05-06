# Train-Network-Analysis


## Initial Network
Notice how there are some disconnected components of the network. So in the next step we plan on cleaning the network.
![image](https://user-images.githubusercontent.com/71708571/167182183-8145db9b-8a67-41ac-a51b-9975e64d10a8.png)


## Cleaning the network and plotting the data on map
The disconnected components are removed and the data is plotted on the map of India for better understanding and better visualization.
![image](https://user-images.githubusercontent.com/71708571/167183535-7dc67404-b7ae-48ae-ad79-f76f6e948207.png)


## Analyzing the network for better understanding of the network
Most of the trains start from the following stations:
```
Howrah Junction 72
Lokmanyatilak T 58
New Delhi 57
Yesvantpur Junction 50
Chennai Central 48
Patna Junction 41
Ajmer Junction 39
Ahmedabad Junction 38
Pune Junction 37
Secunderabad Junction 37
```
Most of the trains end on the following stations:
```
Howrah Junction 70
New Delhi 59
Lokmanyatilak T 58
Chennai Central 52
Yesvantpur Junction 48
Secunderabad Junction 40
Mumbai Cst 40
Ajmer Junction 38
Ahmedabad Junction 37
Pune Junction 37
```
Most influential cities according to betweenness centrality:
```
Howrah Junction 0.14932789676937633
Lokmanyatilak T 0.09710570891297024
New Delhi 0.09494905859032046
Chennai Central 0.0777087234192908
Yesvantpur Junction 0.0669207087234779
Secunderabad Junction 0.05511580608712789
Delhi 0.051055552435616956
Patna Junction 0.051030223245565956
Ajmer Junction 0.0487748806036205
Chennai Egmore 0.04410742143336501
```
Visualization of major cities according to betweenness centrality:
![image](https://user-images.githubusercontent.com/71708571/167185940-e470bacb-6a8c-4613-a878-2cced21631e6.png)
Most influential cities according to eigen vector centrality:
```
Howrah Junction 0.24527293880932532
New Delhi 0.2202230626362209
Chennai Central 0.212237555112324
Lokmanyatilak T 0.1992816217852631
Ahmedabad Junction 0.18108179151045078
Yesvantpur Junction 0.17672900514425904
Ajmer Junction 0.171202505532886
Pune Junction 0.1638834803214224
Jammu Tawi 0.15981791529989423
Mumbai Cst 0.15840696192192677
```
Most influential cities according to closeness centrality:
```
Howrah Junction 0.48671328671328673
New Delhi 0.47218453188602444
Chennai Central 0.46837146702557203
Lokmanyatilak T 0.46461949265687585
Yesvantpur Junction 0.4484536082474227
Ajmer Junction 0.4461538461538462
Patna Junction 0.44387755102040816
Mumbai Cst 0.44387755102040816
Ahmedabad Junction 0.44274809160305345
Jammu Tawi 0.44274809160305345
```


## Community Detection
Using networkx library's in-built function greedy_modularity_communities():
```
Total 11 number of communities detected in the network
```
Visualization of the communities:
![image](https://user-images.githubusercontent.com/71708571/167187131-b03a3a68-6c76-4031-bad4-9a6ff79cb814.png)
