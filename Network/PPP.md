1.工作流程：

（1）创建：通过LCP向对方发送配置选项报文，配置成功，则链路创建完成

（2）认证

（3）协商：用创建阶段协商的结果来配置网络

（4）通信完毕后，发送LCP请求终止和终止确认


2.帧格式：

标志 | 地址 | 控制 | 协议 | 数据 | 校验 | 标志

（1）标志：同HDLC

（2）地址：1B。因为是点对点的，地址没有用，设为广播地址，即11111111

（3）控制：1B。11000000，无编号帧

（4）协议：2B。定义数据字段中携带的数据类型

（5）数据：0 - 1500 B

（6）检验：2B或4B， CRC校验


3.适用场合：

（1）调制解调器

（2） HDLC序列线路

（3）SONET

（4）其它物理层点对点线路


4.特点：

（1）协议简单

（2）支持认证和动态网路配置