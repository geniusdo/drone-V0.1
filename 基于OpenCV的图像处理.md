# 基于OpenCV的图像处理

> 任务

创建一个CMake工程，实现对相机采集图像，并对图像进行清晰化，最终以图片形式进行保存

> 计划

1. 使用任意USB相机，实现简单的OpenCV图像采集功能，并尝试对图像进行简单的处理(不局限于清晰化)
2. 查阅资料，初步设计与实现图像清晰算法，并给出评价算法的指标(比如清晰度、速度、消耗的资源等)
3. 尝试对算法与代码进行优化
   - 算法层面：指标上的提升
   - 代码层面：引入多线程、引入C++11特性：如STL、智能指针(对程序的图像存储有用)、lambda表达式等，这些可以增强代码可读性和可扩展性

4. 接下来就开始分工：

   - (1人)学习ROS，将该工程扩展为ROS功能包，并开始学习mavros，初步实现无人机程控飞行

   - (2人)对算法进行进一步优化
     - 将该工程移植到nv板上
     - 系统学习相机(大恒图像官网有资料)，针对nv板进行相机与镜头选型(相机推荐树莓派IMX477-HQ，镜头得针对场景来选)
     - 学习nv官方的deepstream，进行CSI相机图像采集与高速解码、编码，尝试对工程进行GPU加速
     - 写报告与总结(对电赛报告有帮助，认真写！)

> C++学习路线(按顺序学)

1. [C++基础](http://c.biancheng.net/cplus/)

2. [STL](http://c.biancheng.net/stl/)
3. [CMake基础](https://sfumecjf.github.io/cmake-examples-Chinese/)
4. [少量C++11特性](http://c.biancheng.net/cplus/11/)

5. C++ primer 中的C++11特性，以及查缺补漏(书)

6. effective C++(书)

**建议**：先把1，2和3大概看个两三遍，通过工程上手，查缺补漏，然后有空可以翻翻4，5和6，对之前的代码进行优化，不要贪多嚼不烂，很多编程很久的老鸟都未必熟悉上面的全部！

