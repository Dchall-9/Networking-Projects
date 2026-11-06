OVERVIEW

Created a network to create OSPF adjacencies between 4 routers connected to a switch one router is configured to be the DR and another router to never be DR via interface priority


TOPOLOGY

There are 4 routers and 1 switch using single area OSPF


CONCEPTS

OSPF

DR/BDR elections

OSPF interface priorities

OSPF network statements

Wildcark mask


IMPLEMTATION

All routers use process 10

Adjacencies created using network command

DR priority set to 255

One router's priority set to 0

Verified using show commands


VERIFICATION

show ip ospf neighbor command to verify ajacencies

show running-config command to verify priorities and correct ajacencies


