This project is developed using Tuya SDK, which enables you to quickly develop branded apps connecting and controlling smart scenarios of many devices.         For more information, please check Tuya Developer Website.

一、方案标题
医院低成本大规模部署智能输液系统

二、方案应用场景地点：医院输液室；
功能：医院输液室经常有很多人输液，特别是在流感爆发的季节，但是医院人手又不够的情况下下。这个产品就起到了作用，它可以将输液的频率和是否缺液传送到终端，这样就可以实现一人观察整个输液是。不仅这样，它还可以实现缺液自动停止输液，远程控制停止输液。

三、方案说明

1）频率检测：通过红外对管检测液体滴下的输液。因为液体滴下时会折射红外发射管发射出的红外光，从而导致电压信号的变化，因为通过红外对管得到电压信号噪声比较多，所以还需要后续电路进行滤波整形。

2）缺液检测：通过红外对管检测是否缺液。实现原理为：当有液体时，红外发射管发射出的红外光会被液体折射一部分。从而导致红外接收管在有液体和无液体呈现两个不同的电压值。

3）输液停止：缺液停止由减速电机控制。当mcu收到远程停止命令或者缺液检测模块检测到缺液时，电机会正转2秒顶住输液管。


四、框图

红外对管检测输液频率->                        
红外对管检测液位-----> STM32 <-> WIFI模块               
电机控制<----------- 


四、开发计划4月10前完成

1）3月10前准备物料

2）3月10-25日嵌入式开发、云开发

3）3月28日前整体调试。

4) 3月30日前整理文档和过程文件

