# CPU
（一）开发基本过程概述
第一阶段：查阅资料，确定五段流水线的基本框架
第二阶段：设计MIPS32流水线指令集
第三阶段：指令的实现与模拟仿真验证
第四阶段：数据冲突和控制冲突的解决
第五阶段：数据内存与指令内存的实现
第六阶段：上板验证

第一阶段：查阅资料，确定五段流水线的基本框架
五段流水线主要分为IF、ID、EX、MEM和WB五个阶段，对于同一条指令，五个阶段是顺序执行的，但是对于不同的指令来说，五个阶段又是同时执行的。在这里我选择了使用五个always块的框架，让每一个阶段在上升沿到来的时候都可以被执行，这样就实现了流水线的同时工作。但同时要严格控制好每一个always块的输入输出，使得一个指令可以按顺序正确的运行。每一个阶段的相互关系见下图

在第一阶段介绍一下我使用的各个变量和define文件

第二阶段：设计MIPS32流水线指令集
MIPS32指令集的规范如下

第三阶段：指令的实现与模拟仿真验证
指令的实现与命名参考PDF文件《》，

