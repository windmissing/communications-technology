1.原理

（1）多路访问：多个站点平等接入共享介质

（2）载波监听：发送帧前要监听访问介质，空闲时才发送

（3）冲突检测：发送时仍要监听访问介质

（4）若冲突，延时一段时间，重新发送


2.以太网帧格式

目标地址 | 源地址 | 类型/长度 | 数据 | 校验

（1）目的地址：6B。单播（0*******），多播（1*******），广播（11111111）

（2）源地址：6B。单播地址

（3）类型/长度：2B。

以太网：类型，>1500，记录上层协议

IEEE802.3：长度，<=1500

（4）数据

以太网：46 - 1500B

IEEE802.3：38 - 1492B
（5）校验：4B。CRC


3.适用场合

传统以太网的共享总结拓扑结构