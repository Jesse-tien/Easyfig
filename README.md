# 无脑简单学术专业绘图工具——Easyfig 使用说明【已更新至3.7.0版本！】

## 一、它能干啥？

我开发的这个工具名字叫Easyfig，字面意思“容易画图”，它能干啥？简单说，就是给没有编程基础、商学院管科专业学生使用，用于快速做数值仿真的工具，可以绘制的数值仿真形式包括：

**（1）单个参数的分析**

> ![img](https://pica.zhimg.com/80/v2-27b56b2631a5d0c1413a517caee3e211_1440w.png?source=ccfced1a)
>
> 图：示例论文 Blockchain adoption and mode selection strategies for remanufacturing supply chain under cap-and-trade policy, Computers & Industrial Engineering, 192, 2024, 110246, https://doi.org/10.1016/j.cie.2024.110246.

**（2）两个参数同时分析-最优模式所在区域绘制**

> ![img](https://pic1.zhimg.com/80/v2-c81c3830d01d5346c4854d206595ffa6_1440w.png?source=ccfced1a)
>
> 图：示例论文 Blockchain adoption and mode selection strategies for remanufacturing supply chain under cap-and-trade policy, Computers & Industrial Engineering, 192, 2024, 110246, https://doi.org/10.1016/j.cie.2024.110246.

**（3）两个参数同时分析-各个区域利润函数之间的详细大小关系**

> ![img](https://pic1.zhimg.com/80/v2-67707b0662a9dec78b724d51f485aa26_1440w.png?source=ccfced1a)
>
> 图：示例论文 E-retailer information sharing with suppliers online selling mode, Information Sciences 622 (2023) 1252-1272. https://doi.org/10.1016/j.ins.2022.10.094.

**（4）两个参数同时分析-三维图**

> ![img](https://pic1.zhimg.com/80/v2-f979c89165160166d03ca8d2584adc6d_1440w.png?source=ccfced1a)
>
> 图：示例论文 Recycling mode selection and carbon emission reduction decisions for a multi-channel closed-loop supply chain of electric vehicle power battery under cap-and-trade policy, Journal of Cleaner Production 375 (2022) 134060.https://doi.org/10.1016/j.jclepro.2022.134060.

---

## 二、如何安装和启动？

第一步：安装Python；第二步：引入我开发的easyfig包。

### 2.1 安装Python【如果电脑已经安装3.8版本以上的Python，则此步跳过】

进入官网[https://www.python.org/](https://www.python.org/) ，点击Downloads，安装最新版本Python即可（例如3.13.1）。

![img](https://picx.zhimg.com/80/v2-38a0157b458b7462ba1aa7392ac191d5_1440w.png?source=ccfced1a)

图：Python官网

### 2.2 安装easyfig

对于Windows用户，按下组合键，Win+R，输入cmd打开命令窗口（黑的），然后在命令窗口内输入： 

> **pip install easyfig==3.7.0**

回车即可，如图所示，等待安装完成。（**注意：1.要联网；2.关掉梯子VPN**）如果中途出现红字，说明因网络原因安装失败，检查网络，并重新做此步即可。

> ![img](https://picx.zhimg.com/80/v2-18168731ddb4910ea2ff20487854e036_1440w.png?source=ccfced1a)
>
> 图：Win+R，输入``cmd``回车

### 2.3 启动easyfig

**对于Windows用户，按下组合键“Win+R”，输入“easyfig”直接回车即可！如果是Windows 11，直接在电脑自带的搜索框中搜索“easyfig”也可以打开，非常方便（如图）！还可以建立桌面快捷方式，具体见视频。**

> ![img](https://picx.zhimg.com/80/v2-953e7ea598b69cfe48c6b16cbdafec43_1440w.png?source=ccfced1a)
>
> 图：Windows 11 打开easyfig快速方法

下面是视频演示：【或者[点击此处播放](https://vdn3.vzuu.com/HD/ea259b7e-cff6-11ef-b075-6e0de0aa0e6e-v8_f2_t1_ub9zZUlv.mp4?auth_key=1787227745-0-0-754ec0dccac8444121524775997f739e&amp;bu=09fd86c2&amp;c=avc.8.0&amp;disable_local_cache=1&amp;expiration=1787227745&amp;f=mp4&amp;pu=e59e796c&amp;v=tx&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu)】

> <video class="_1k7bcr7" preload="metadata" playsinline="" webkit-playsinline="" x-webkit-airplay="deny" src="https://vdn3.vzuu.com/HD/ea259b7e-cff6-11ef-b075-6e0de0aa0e6e-v8_f2_t1_ub9zZUlv.mp4?auth_key=1787227745-0-0-754ec0dccac8444121524775997f739e&amp;bu=09fd86c2&amp;c=avc.8.0&amp;disable_local_cache=1&amp;expiration=1787227745&amp;f=mp4&amp;pu=e59e796c&amp;v=tx&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu" style="object-fit: contain;"></video>
>
> 视频：安装和启动easyfig

---

## 三、如何使用？【 针对完全没学过Python的同学，无脑使用界面即可】

本工具独创UI界面向导，无需输入代码，即可完成仿真绘图！

我们以学术论文：

Yanliang Zhang, Jingrui Zhang, Yanjie Zhou, Huadong Zhao, Yanpei Cheng, Blockchain adoption and mode selection strategies for remanufacturing supply chain under cap-and-trade policy, Computers & Industrial Engineering, 192, 2024, 110246, [https://doi.org/10.1016/j.cie.2024.110246](https://doi.org/10.1016/j.cie.2024.110246).

为例，进行演示。

作者提出了四种模式，利润函数分别为：
$$
\begin{equation} \pi_r^{NW}=E p_{e} + \frac{k \left(\alpha \delta \left(c_{n} + e_{n} p_{e}\right) - c_{r} - e_{r} p_{e}\right)^{2}}{8 \left(\alpha \delta \left(- \alpha \delta + 1\right) + k\right)^{2}}\tag{1} \end{equation}
$$

$$
\begin{equation} \pi_r^{BW}=E p_{e} + \frac{k \left(- b - c_{r} + \delta \left(c_{n} + e_{n} p_{e}\right) - e_{r} p_{e}\right)^{2}}{8 \left(- \delta^{2} + \delta + k\right)^{2}}\tag{2} \end{equation}
$$

$$
\begin{equation} \pi_r^{NS}=E p_{e} + \frac{\left(2 \alpha \delta + k\right) \left(\alpha \delta \left(c_{n} + e_{n} p_{e}\right) - c_{r} - e_{r} p_{e}\right)^{2}}{8 \left(\alpha \delta \left(- \alpha \delta + 2\right) + k\right)^{2}}\tag{3} \end{equation}
$$

$$
\begin{equation} \pi_r^{BS}=E p_{e} + \frac{\left(2 \delta + k\right) \left(- b - c_{r} + \delta \left(c_{n} + e_{n} p_{e}\right) - e_{r} p_{e}\right)^{2}}{8 \left(- \delta^{2} + 2 \delta + k\right)^{2}}\tag{4} \end{equation}
$$

参数默认赋值为：

![img](https://picx.zhimg.com/80/v2-83657c702ca10f0a78799341f48eabe8_1440w.png?source=ccfced1a)

### 3.1 表达式快速输入的技巧

首先，在“表达式输入”框中，输入四个表达式，格式为：

```
表达式名称 = 表达式
```

其中，`表达式名称`可以写单词、汉字以及空格，也可以写LaTex形式（**LaTeX部分的两侧需要用\$包裹**）。例如：“模式A”、“\$Mode_A\$”、“利润 \$\pi_r^{NW}\$”等。**比较随意，表达式名称决定了图例是啥**。对于LaTex的写法，请见**附录A**。

`表达式`**书写要求：**

（1）数学符号只能由英文字母、下划线（表示下角标）和数字组成，并且数字不能开头，希腊字母写对应的英文单词（**千万注意不是LaTeX！**），特别地， λ **要写为“lamda”**。例如：“p_e”、“alpha”、“q_2”等，特殊符号可以点击界面上的“ Ω... ”按钮键入；

（2）运算符号写法：加为`+`，减为`-`，乘为`*`，除为`/`，注意次方写成`^`或`**`都可以，优先运算用小括号`()`。可以看出，这和我们平时正常书写公式没啥太大区别。

> ![img](https://picx.zhimg.com/80/v2-4eaf81c78b291f973beb86e22dfe2598_1440w.png?source=ccfced1a)
>
> 图：打开符号面板

下面是一组正确的示范：

```
$\pi_r^{NW}$ = E*p_e+(k*(alpha*delta*(c_n+e_n*p_e)-(c_r+e_r*p_e))^2)/(8*(k+alpha*delta*(1-alpha*delta))^2)
Hollow word = E*p_e + ( k*(delta*(c_n+e_n*p_e)-(c_r+e_r*p_e+b))^2 )/( 8*(k+delta-delta^2)^2)
NS下的利润$\pi$ = E*p_e + ((k+2*alpha*delta)*(alpha*delta*(c_n+e_n*p_e)-(c_r+e_r*p_e))^2 )/( 8*(k+alpha*delta*(2-alpha*delta))^2)
这个工具 yyds = E*p_e + ( (k+2*delta)*(delta*(c_n+e_n*p_e)-(c_r+e_r*p_e+b))^2 )/( 8*(k+2*delta-delta^2)^2)
```

**对于特别长的公式，尤其括号嵌套特别多时，手写公式很痛苦！好在easyfig给我们提供了工具！**点击界面上的“打开LaTeX转换器”，即可进入该工具。**注意：该工具只负责转换"="的右边部分！"="左边需要用户自己起名。**

（1）对于Mathtype输入的Word公式，需要选择“通用LaTex”选项，输入LaTex代码，点击“转换”即可。注意：第一次使用，后台会安装插件，安装好后，会提示“安装\`antlr4-python3-runtime==4.xx\`成功，请重新启动easyfig即可!”，按照要求，重启easyfig即可。

（2）对于Mathematica的结果，右键选择“复制为”，点击“LaTeX”，类似地，将内容粘贴到输入框中，但要选择“Mathematica LaTex”，点击“转换”，复制结果即可。

> ![img](https://pica.zhimg.com/80/v2-e58ff42e038247146d4376da58635d0e_1440w.png?source=ccfced1a)
>
> 图：Mathematica LaTex

为了方便大家理解，关于上述功能的视频演示如下（2.0.0版本，新版本操作一样，增加了matlab代码转sympy的功能）：【或者[点击此处播放](https://vdn3.vzuu.com/HD/cdd987d6-cff7-11ef-8e3b-fe5fec143453-v8_f2_t1_Hxye2XeN.mp4?auth_key=1787227745-0-0-697a04c7d93bd0156c0a492e420c70ce&amp;bu=09fd86c2&amp;c=avc.8.0&amp;disable_local_cache=1&amp;expiration=1787227745&amp;f=mp4&amp;pu=e59e796c&amp;v=tx&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu)】

> <video class="_1k7bcr7" preload="metadata" playsinline="" webkit-playsinline="" x-webkit-airplay="deny" src="https://vdn3.vzuu.com/HD/cdd987d6-cff7-11ef-8e3b-fe5fec143453-v8_f2_t1_Hxye2XeN.mp4?auth_key=1787227745-0-0-697a04c7d93bd0156c0a492e420c70ce&amp;bu=09fd86c2&amp;c=avc.8.0&amp;disable_local_cache=1&amp;expiration=1787227745&amp;f=mp4&amp;pu=e59e796c&amp;v=tx&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu" style="object-fit: contain;"></video>
>
> 视频：如何快速输入公式？借助转换工具

### 3.2 单参数数值分析

单参数数值分析需要在“绘制仿真折线图”界面中进行。输入公式完成后，点击“公式识别”，当下面的运行信息显示“公式识别成功！”时，进行下一步：分析参数选取。具体操作请看我演示视频：【或者[点击此处播放](https://vdn3.vzuu.com/HD/ae89b958-cff9-11ef-9fe3-360077e0e5a0-v8_f2_t1_2W9aMLGn.mp4?auth_key=1787227745-0-0-aff00d7063cbc378b70d72f7ddaa8ef2&amp;bu=09fd86c2&amp;c=avc.8.0&amp;disable_local_cache=1&amp;expiration=1787227745&amp;f=mp4&amp;pu=e59e796c&amp;v=tx&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu)】

> <video class="_1k7bcr7" preload="metadata" playsinline="" webkit-playsinline="" x-webkit-airplay="deny" src="https://vdn3.vzuu.com/HD/ae89b958-cff9-11ef-9fe3-360077e0e5a0-v8_f2_t1_2W9aMLGn.mp4?auth_key=1787227745-0-0-aff00d7063cbc378b70d72f7ddaa8ef2&amp;bu=09fd86c2&amp;c=avc.8.0&amp;disable_local_cache=1&amp;expiration=1787227745&amp;f=mp4&amp;pu=e59e796c&amp;v=tx&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu" style="object-fit: contain;"></video>
>
> 视频：单参数数值曲线外观设置

**文件的保存与打开**：easyfig支持将设定好的图像数据保存。点击“保存...”，可以以.py或.txt的格式将你的画图数据保存下来；当以后想修改这个画图时，点击“打开...”，选择你之前保存的.py或.txt文件，即可恢复之前的工作。具体操作请见视频演示：【或者[点击此处播放](https://vdn6.vzuu.com/HD/23b5c49c-cffa-11ef-96de-16b14928db12-v8_f2_t1_FjAFE1qz.mp4?pkey=AAX0xFvkAjl91OXXs7i4mXjscpUarJUCACQUq2mb0cbUjclQVh6KEWY2Pb-C_tJX3g0-8SpfcK8hyCunREVpmt6d&amp;bu=09fd86c2&amp;c=avc.8.0&amp;expiration=1787231345&amp;f=mp4&amp;pu=e59e796c&amp;v=ks6&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu)】

> <video class="_1k7bcr7" preload="metadata" playsinline="" webkit-playsinline="" x-webkit-airplay="deny" src="https://vdn6.vzuu.com/HD/23b5c49c-cffa-11ef-96de-16b14928db12-v8_f2_t1_FjAFE1qz.mp4?pkey=AAX0xFvkAjl91OXXs7i4mXjscpUarJUCACQUq2mb0cbUjclQVh6KEWY2Pb-C_tJX3g0-8SpfcK8hyCunREVpmt6d&amp;bu=09fd86c2&amp;c=avc.8.0&amp;expiration=1787231345&amp;f=mp4&amp;pu=e59e796c&amp;v=ks6&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu" style="object-fit: contain;"></video>
>
> 视频：保存与打开操作

### 3.3 双参数分析-最优模式分析

具体请看视频演示：【或者[点击此处播放](https://vdn6.vzuu.com/HD/fada60c2-cffa-11ef-bd0d-32480b71c768-v8_f2_t1_9k2wSS1p.mp4?pkey=AAXjiCsAonumZOXxk9BUpkixThXv4aIbpYeTIAp02TTOwm5Eb7Czj5CdoTgckhKvJMMxVms3cLjq3G_IkoEyQEpX&amp;bu=09fd86c2&amp;c=avc.8.0&amp;expiration=1787231345&amp;f=mp4&amp;pu=e59e796c&amp;v=ks6&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu)】

> <video class="_1k7bcr7" preload="metadata" playsinline="" webkit-playsinline="" x-webkit-airplay="deny" src="https://vdn6.vzuu.com/HD/fada60c2-cffa-11ef-bd0d-32480b71c768-v8_f2_t1_9k2wSS1p.mp4?pkey=AAXjiCsAonumZOXxk9BUpkixThXv4aIbpYeTIAp02TTOwm5Eb7Czj5CdoTgckhKvJMMxVms3cLjq3G_IkoEyQEpX&amp;bu=09fd86c2&amp;c=avc.8.0&amp;expiration=1787231345&amp;f=mp4&amp;pu=e59e796c&amp;v=ks6&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu" style="object-fit: contain;"></video>
>
> 视频：双参数分析-最优模式分析

### 3.4 双参数分析-详细区域分析

请看视频演示：【或者[点击此处播放](https://vdn6.vzuu.com/HD/97e962b8-cffc-11ef-b938-fe5fec143453-v8_f2_t1_0retzLUs.mp4?pkey=AAUOMk-Aloj9Xu834KSog8pkJ2PiO6ylaSa3CxhadBNUULjY5RsYY2M3gbr-KdNrhJpJql-4pDzWqCcCzS3mWhvS&amp;bu=09fd86c2&amp;c=avc.8.0&amp;expiration=1787231345&amp;f=mp4&amp;pu=e59e796c&amp;v=ks6&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu)】

> <video class="_1k7bcr7" preload="metadata" playsinline="" webkit-playsinline="" x-webkit-airplay="deny" src="https://vdn6.vzuu.com/HD/97e962b8-cffc-11ef-b938-fe5fec143453-v8_f2_t1_0retzLUs.mp4?pkey=AAUOMk-Aloj9Xu834KSog8pkJ2PiO6ylaSa3CxhadBNUULjY5RsYY2M3gbr-KdNrhJpJql-4pDzWqCcCzS3mWhvS&amp;bu=09fd86c2&amp;c=avc.8.0&amp;expiration=1787231345&amp;f=mp4&amp;pu=e59e796c&amp;v=ks6&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu" style="object-fit: contain;"></video>
>
> 视频：双参数分析-详细区域分析

### 3.5 双参数分析-三维图分析

请看视频演示：【或者[点击此处播放](https://vdn6.vzuu.com/HD/534e7ee4-cffd-11ef-8143-22248896a882-v8_f2_t1_bKALETgd.mp4?pkey=AAWrAjy-g84aFusZ85qHYX-4VkB8noYBWBysnUnKN1NygkQGmlytGOx1yZjB5dIt02THc5WWQiFemVuU17g-2JkP&amp;bu=09fd86c2&amp;c=avc.8.0&amp;expiration=1787231345&amp;f=mp4&amp;pu=e59e796c&amp;v=ks6&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu)】

> <video class="_1k7bcr7" preload="metadata" playsinline="" webkit-playsinline="" x-webkit-airplay="deny" src="https://vdn6.vzuu.com/HD/534e7ee4-cffd-11ef-8143-22248896a882-v8_f2_t1_bKALETgd.mp4?pkey=AAWrAjy-g84aFusZ85qHYX-4VkB8noYBWBysnUnKN1NygkQGmlytGOx1yZjB5dIt02THc5WWQiFemVuU17g-2JkP&amp;bu=09fd86c2&amp;c=avc.8.0&amp;expiration=1787231345&amp;f=mp4&amp;pu=e59e796c&amp;v=ks6&amp;pp=ChMxNDAxNjIzODY1NzM5NTc5MzkyGGMiC2ZlZWRfY2hvaWNlMhMxMzY5MDA1NjA4NTk5OTA0MjU3PXu830Q%3D&amp;pf=Web&amp;pt=zhihu" style="object-fit: contain;"></video>
>
> 视频：双参数分析-三维图分析

---

## 四、Easyfig高阶用法【针对Python编程同学，作为Python第三方包编程使用】

推荐用Jupyter，可以直接编程使用，能够更细致地设置图片细节。

```python
from easyfig import *   # 固定写法
%config InlineBackend.figure_format = 'retina' # 在 Jupyter 中显示高清图片

# 如果想快速上手，推荐使用make_example()函数生成示例代码，直接修改！
make_example("data_lines")
```

### 4.1 根据数据绘制曲线【data_lines函数】

```python
# 以方括号（列表、numpy数组均可）形式给出数据，并给这组数据起个名字：
data = {
    '景区1旅游人次': [1230, 45789, 2600, 320, 991480, 65780, 89990, 70001, 6423, 415000, 340, 102],
    '景区2旅游人次': [800, 34000, 1690, 139, 76788, 453565, 87898, 64302, 3423, 325001, 127, 13],
    '景区3旅游人次': [5230, 65789, 7600, 820, 1091480, 85780, 99995, 90001, 9423, 705000, 640, 707],
}

# 给横轴添加刻度标签，注意要和data长度一致！
label_x = ['2020-1', '2020-2', '2020-3', '2020-4',  '2020-5', '2020-6',  '2020-7',  '2020-8',  '2020-9',  
           '2020-10',  '2020-11',  '2020-12']

# 自定义xy轴名称：
x_name = '月总旅游人次'
y_name = '月份'

# 保存路径
save_dir = 'data_sigle.tiff'

# 图例的方位，可以选填的内容有'best','northeast','northwest','southwest','southeast','east','west','south','north','center'。
# 默认值为'best'，表示自动安排至合适的位置。
location = 'best'
# 图例的列数，默认为1列，即竖着排布。
ncol = 1

fsize = 14 # 图片中字号的大小，默认值为14。
figsize = [7, 5] # 图片的大小，写成`[宽, 高]`的形式。

# 横轴刻度标签旋转角度。用于刻度为年份，横着挤不下的情况，可以设成45度，错开排布。默认不旋转，即0度。
xt_rotation = 45

# 横轴名字标签旋转角度，默认值0，基本不需要动。
xrotation = 0
# 纵轴名字标签旋转角度，默认值90，字是正的。如果y轴的名字较长，不好看，可以设成0，字是竖倒着写的，紧贴y轴。
yrotation = 90 

# 一组线的形状，如实线'-'，点横线'-.'，虚线'--'，点线':'。
linestyles = ['-', '-.','--'] 
linewidth = 1.2 # 线粗。

markers = ['o','s', '*'] # 线上的标记符号,关于标记符号的详细说明 https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
markersize = 3.5 # 标记符号的大小，默认3.5。
# 四条线的颜色
colors = ['blue','red','green']

isgrid = False # 是否要网格。要就填True，不要就是False，默认不要。
# x/y轴刻度值距离横轴的距离
xpad = 3
ypad = 3
# x/y轴名字标签距离横轴刻度的距离。
xlabelpad = 3
ylabelpad = 3

# 自定义坐标轴字体大小
xlabelsize = 39 # 横轴字大小，默认'auto'，自动和fsize一样大
ylabelsize = 9 # 纵轴字大小，默认'auto'，自动和fsize一样大
legendsize = 17 # 图例字大小，默认'auto'，自动和fsize一样大

# 传给data_lines函数 (不要改！)
# Passed to the data_lines function (Don't change!).
plt = data_lines(data, label_x=label_x, x_name=x_name, y_name=y_name, save_dir=save_dir, location=location, ncol=ncol,
           fsize=fsize, figsize=figsize, xt_rotation=xt_rotation, xrotation=xrotation, yrotation=yrotation, 
           linestyles=linestyles, linewidth=linewidth, markers=markers, markersize=markersize, colors=colors,
          isgrid=isgrid, xpad=xpad, ypad=ypad, xlabelpad=xlabelpad, ylabelpad=ylabelpad, 
            xlabelsize=xlabelsize, ylabelsize=ylabelsize, legendsize=legendsize)
plt.title('旅游数据') # 还可以个性化加东西
plt
```

<img src="https://pic1.zhimg.com/80/v2-f6195f7bd0153728988a7018b58e0bf6_1440w.png?source=ccfced1a" alt="img" style="zoom: 50%;" />

### 4.2 数值仿真符号函数的曲线【draw_lines函数】

```python
# 定义符号 
# Define symbols
c_n, c_r, delta, e_n, e_r, p_e, E, k, b, alpha = symbols('c_n, c_r, delta, e_n, e_r, p_e, E, k, b, alpha')

# 四个表达式
# Four expressions
expressions = {
    r'$\pi_r^{NW}$': E*p_e+(k*(alpha*delta*(c_n+e_n*p_e)-(c_r+e_r*p_e))**2)/(8*(k+alpha*delta*(1-alpha*delta))**2), 
    r'$\pi_r^{BW}$': E*p_e + ( k*(delta*(c_n+e_n*p_e)-(c_r+e_r*p_e+b))**2 )/( 8*(k+delta-delta**2)**2), 
    r'$\pi_r^{NS}$': E*p_e + ((k+2*alpha*delta)*(alpha*delta*(c_n+e_n*p_e)-(c_r+e_r*p_e))**2 )/( 8*(k+alpha*delta*(2-alpha*delta))**2),
    r'$\pi_r^{BS}$': E*p_e + ( (k+2*delta)*(delta*(c_n+e_n*p_e)-(c_r+e_r*p_e+b))**2 )/( 8*(k+2*delta-delta**2)**2),
}

# 参数赋值
# Parameter assignment
assigns = {c_n: 0.2, c_r: 0.1, delta: 0.8, e_n: 1, e_r: 0.6, p_e: 0.1, E: 2, k: 1.1, alpha:0.9}

# 要分析的参数，及其取值范围
# The parameters to be analyzed and their value ranges.
the_var = b
ranges = [0, 0.08, 0.01]  # [起始值, 终止值, 间隔]。 [Starting value, ending value, interval].

# xy轴的名字
# The names of the x-axis and y-axis.
x_name = r'(a) Parameter $b$'
y_name = r'$\pi_r$'

# 图片保存路径、文件名
# Picture save path and file name.
save_dir = r'mutiple_line.tiff'

# 图例的方位，可以选填的内容有'best','northeast','northwest','southwest','southeast','east','west','south','north','center'。
# 默认值为'best'，表示自动安排至合适的位置。
location = 'best' 

# 图例的列数，默认为1列，即竖着排布。
ncol = 1
# 图片中字号的大小
fsize = 14
# 图片的大小，写成`[宽, 高]`的形式。
figsize = [5, 4]

xt_rotation = 0 # 横轴刻度标签旋转角度。用于刻度为年份，横着挤不下的情况，可以设成45度，错开排布。默认不旋转，即0度。
# xrotation/yrotation: x/y轴名字标签旋转角度。
xrotation = 0
yrotation = 90

linestyles = ['-','-.','--', ':'] # 线的风格，实线'-'，点横线'-.'，虚线'--'，点线':'。
linewidth = 1.0 # 线粗。
markers = ['o','s', '*', 'P'] # 线上的标记符号,关于标记符号的详细说明 https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
markersize = 3.5 # 标记符号的大小，默认3.5。
# 四条线的颜色
colors = ['black','blue','red','green']

# 是否要网格。要就填True，不要就是False
isgrid = False

# 分别为x/y轴刻度值距离横轴的距离。
xpad = 3
ypad = 3

# 分别为x/y轴名字标签距离纵轴刻度的距离。
xlabelpad = 13
ylabelpad = 2

# 自定义坐标轴字体大小
xlabelsize = 39 # 横轴字大小，默认'auto'，自动和fsize一样大
ylabelsize = 9 # 纵轴字大小，默认'auto'，自动和fsize一样大
legendsize = 17 # 图例字大小，默认'auto'，自动和fsize一样大


# 传给draw_lines函数 (不要改！)
# Passed to the draw_lines function (Don't change!).
draw_lines(expressions=expressions, assigns=assigns, the_var=the_var, ranges=ranges, x_name=x_name, y_name=y_name, 
           save_dir=save_dir, location=location, ncol=ncol, fsize=fsize, figsize=figsize, xt_rotation=xt_rotation,
          xrotation=xrotation, yrotation=yrotation, linestyles=linestyles, linewidth=linewidth, markers=markers,
          markersize=markersize, colors=colors, isgrid=isgrid, xpad=xpad, ypad=ypad, xlabelpad=xlabelpad, ylabelpad=ylabelpad,
           xlabelsize=xlabelsize, ylabelsize=ylabelsize, legendsize=legendsize)
```

<img src="https://picx.zhimg.com/80/v2-4f11d55eff6a90bf46c7655f8ae626f4_1440w.png?source=ccfced1a" alt="img" style="zoom: 50%;" />

### 4.3 同时分析两个参数，绘制三维曲线【draw_3D函数】

```python
# 定义符号 
# Define symbols
c_n, c_r, delta, e_n, e_r, p_e, E, k, b, alpha = symbols('c_n, c_r, delta, e_n, e_r, p_e, E, k, b, alpha')

# 四个表达式
# Four expressions
expressions = {
    r'$\pi_r^{NW}$': E*p_e+(k*(alpha*delta*(c_n+e_n*p_e)-(c_r+e_r*p_e))**2)/(8*(k+alpha*delta*(1-alpha*delta))**2), 
    r'$\pi_r^{BW}$': E*p_e + ( k*(delta*(c_n+e_n*p_e)-(c_r+e_r*p_e+b))**2 )/( 8*(k+delta-delta**2)**2), 
    r'$\pi_r^{NS}$': E*p_e + ((k+2*alpha*delta)*(alpha*delta*(c_n+e_n*p_e)-(c_r+e_r*p_e))**2 )/( 8*(k+alpha*delta*(2-alpha*delta))**2),
    r'$\pi_r^{BS}$': E*p_e + ( (k+2*delta)*(delta*(c_n+e_n*p_e)-(c_r+e_r*p_e+b))**2 )/( 8*(k+2*delta-delta**2)**2),
}

# 参数赋值
# Parameter assignment
assigns = {c_n: 0.2, c_r: 0.1, delta: 0.8, e_n: 1, e_r: 0.6, p_e: 0.1, E: 2, k: 1.1}

# 要分析的参数，及其取值范围
# The parameters to be analyzed and their value ranges.
the_var_x = alpha
start_end_x = [0.7, 0.8]  # [起始值, 终止值]。 [starting value, ending value].
the_var_y = b
start_end_y = [0, 0.08]  # [起始值, 终止值]。 [starting value, ending value].

# xy轴的名字
# The names of the x-axis and y-axis.
x_name = r'$\alpha$' 
y_name = r'$b$'
z_name = r'$\pi_r$' 

# 图片保存路径、文件名
# Picture save path and file name.
save_dir = r'muti_3d.tiff'

# 曲面的透明度。取值范围0到1，浮点数。0表示全透明，1表示完全不透明。
color_alpha = 0.8 
# 图例的方位，可以选填的内容有'best','northeast','northwest','southwest','southeast','east','west','south','north','center'。
# 默认值为'best'，表示自动安排至合适的位置。

location = 'best' 
# 图例的列数，默认为1列，即竖着排布。
ncol = 4
# 图片中字号的大小
fsize = 14
# 图片的大小，写成`[宽, 高]`的形式。默认为`[7, 5]`。
figsize = [7, 5]
# xrotation/yrotation: x/y轴名字标签旋转角度，默认值0，基本不需要动。
xrotation = 0
yrotation = 0
# Z轴名字标签旋转角度，默认值90，字是正的。如果Z轴的名字较长，不好看，可以设成0，字是竖倒着写的，紧贴Z轴
zrotation = 90
# 是否要网格。要就填True，不要就是False
isgrid = True

# 在多面图中用于按顺序制定每个面的颜色（包含标记符号的颜色）。
colors = ['yellow','blue','red','green']
# 曲面上线框的颜色。若为None，则曲面上不画线。当该参数不为None时，参数`linestyles`，`linewidth`和`density`才起作用。
edgecolor = 'black'
linestyles = ['-','-.','--', ':'] # 实线'-'，点横线'-.'，虚线'--'，点线':'。
linewidth = 0.5 # 线粗。
density = 50 # 曲面上画线的密度，也就是曲面横纵方向各画多少根线。默认100。

# 仰角 (elevation)。定义了观察者与 xy 平面之间的夹角，也就是观察者与 xy 平面之间的旋转角度。
elevation = 15
# 方位角 (azimuth)。定义了观察者绕 z 轴旋转的角度。它决定了观察者在 xy 平面上的位置。
azimuth = 45

# 左、下、右、上的图片留白，默认分别为0,0,1,1。不需要动，除非不好看。
left_margin = 0
bottom_margin = 0
right_margin = 1
top_margin = 1

# 分别为/y/z轴刻度值距离横轴的距离。
xpad = 1
ypad = 1
zpad = 5

# 分别为/y/z轴名字标签距离纵轴刻度的距离。
xlabelpad = 2
ylabelpad = 2
zlabelpad = 12

# 自定义坐标轴字体大小
xlabelsize = 39 # 横轴字大小，默认'auto'，自动和fsize一样大
ylabelsize = 9 # 纵轴字大小，默认'auto'，自动和fsize一样大
zlabelsize = 'auto' # 纵轴字大小，默认'auto'，自动和fsize一样大
legendsize = 19 # 图例字大小，默认'auto'，自动和fsize一样大


# 传给draw_3D函数 (不要改！)
# Passed to the draw_3D function (Don't change!).
draw_3D(expressions=expressions, assigns=assigns, the_var_x=the_var_x, start_end_x=start_end_x, the_var_y=the_var_y, 
        start_end_y=start_end_y, x_name=x_name, y_name=y_name, z_name=z_name, 
        save_dir=save_dir, color_alpha=color_alpha, location=location, ncol=ncol, fsize=fsize, figsize=figsize, 
        xrotation=xrotation, yrotation=yrotation, zrotation=zrotation, isgrid=isgrid, colors=colors, 
        edgecolor=edgecolor, linestyles=linestyles, linewidth=linewidth, density=density, elevation=elevation, azimuth=azimuth, 
        left_margin=left_margin, bottom_margin=bottom_margin, right_margin=right_margin, top_margin=top_margin,
        xpad=xpad, ypad=ypad, zpad=zpad, xlabelpad=xlabelpad, ylabelpad=ylabelpad, zlabelpad=zlabelpad,
       xlabelsize=xlabelsize, ylabelsize=ylabelsize, zlabelsize=zlabelsize, legendsize=legendsize)
```

<img src="https://pic1.zhimg.com/80/v2-207bb9d59c8f35e4940cf0b06573ceb4_1440w.png?source=ccfced1a" alt="img" style="zoom:50%;" />

### 4.4 基于最大利润的模式比较【draw_max_area函数】

```python
# 定义符号 
# Define symbols
c_n, c_r, delta, e_n, e_r, p_e, E, k, b, alpha = symbols('c_n, c_r, delta, e_n, e_r, p_e, E, k, b, alpha')

# 四个表达式
# Four expressions
expressions = {
    r'$\pi_r^{NW}$': E*p_e+(k*(alpha*delta*(c_n+e_n*p_e)-(c_r+e_r*p_e))**2)/(8*(k+alpha*delta*(1-alpha*delta))**2), 
    r'$\pi_r^{BW}$': E*p_e + ( k*(delta*(c_n+e_n*p_e)-(c_r+e_r*p_e+b))**2 )/( 8*(k+delta-delta**2)**2), 
    r'$\pi_r^{NS}$': E*p_e + ((k+2*alpha*delta)*(alpha*delta*(c_n+e_n*p_e)-(c_r+e_r*p_e))**2 )/( 8*(k+alpha*delta*(2-alpha*delta))**2),
    r'$\pi_r^{BS}$': E*p_e + ( (k+2*delta)*(delta*(c_n+e_n*p_e)-(c_r+e_r*p_e+b))**2 )/( 8*(k+2*delta-delta**2)**2),
}

# 参数赋值
# Parameter assignment
assigns = {c_n: 0.2, c_r: 0.1, delta: 0.8, e_n: 1, e_r: 0.6, p_e: 0.1, E: 2, k: 1.1}

# 要分析的参数，及其取值范围
# The parameters to be analyzed and their value ranges.
the_var_x = alpha
start_end_x = [0.7, 0.8]  # [起始值, 终止值]。 [starting value, ending value].
the_var_y = b
start_end_y = [0, 0.08]  # [起始值, 终止值]。 [starting value, ending value].

# xy轴的名字
# The names of the x-axis and y-axis.
x_name = '$\\alpha$ \n (b) With blockchain' 
y_name = r'$b$'  

# 图片保存路径、文件名
# Picture save path and file name.
save_dir = r'max_area.tiff' 

# 四个表达式分别达到最大时显示的标签、区域背景颜色和区域图案。
# The labels, regional background colors and regional patterns displayed when the four expressions reach their maxima respectively.
texts = [r'NW', r'BW', r'NS', r'BS']  
colors = ['#dae3f3', '#fbe5d6', '#e2f0d9', '#ededed']
patterns = [' ', '+', '\\', '-']

# 其他设置
text_fsize_add = 2 # 区域标签字号增量。 Increment of regional label font size.
figsize=[5, 4] # 图片大小：宽5高4。 icture size: width 5, height 4.
xrotation=0 # x轴标签名旋转角度（0为不旋转）。 Rotation angle of x-axis label name (0 means no rotation).
yrotation=0 # y轴标签名旋转角度（0为不旋转）。 Rotation angle of y-axis label name (0 means no rotation).
linewidths=0.1 # 线粗0.1. Line thickness: 0.1.

# x/y轴名字标签距离横轴刻度的距离
xlabelpad = 3
ylabelpad = 17

# 自定义坐标轴字体大小
xlabelsize = 8 # 横轴字大小，默认'auto'，自动和fsize一样大
ylabelsize = 29 # 纵轴字大小，默认'auto'，自动和fsize一样大

# 标签背景色和位置偏移自定义设置，默认'auto'自动
pattern_colors = ['#dae3f3', 'white', 'none', 'auto']  # 分别为NW,BW,NS,BS设置标签背景色，'auto'为自动，'none'为透明
pattern_moves = [(+0.005, +0.01), (+0, -0.005), (0, 0), (0, 0)]  # 分别为NW,BW,NS,BS设定区域标签较原来的偏移量，(x方向，y方向)


# 传给draw_max_area函数（不要改！）
# Passed to the draw_max_area function (Don't change!).
draw_max_area(expressions=expressions, assigns=assigns, 
              the_var_x=the_var_x, start_end_x=start_end_x, 
              the_var_y=the_var_y, start_end_y=start_end_y, 
              x_name=x_name, y_name=y_name, 
              fsize=14, texts=texts, text_fsize_add=text_fsize_add,
              save_dir=save_dir, figsize=figsize, colors=colors, patterns=patterns,
              xrotation=xrotation, yrotation=yrotation, linewidths=linewidths,
             xlabelsize=xlabelsize, ylabelsize=ylabelsize, pattern_colors=pattern_colors, 
              pattern_moves=pattern_moves, xlabelpad=xlabelpad, ylabelpad=ylabelpad)
```

<img src="https://picx.zhimg.com/80/v2-73a1a71ffd7657f11f0378c9039aa3f4_1440w.png?source=ccfced1a" alt="img" style="zoom:50%;" />

### 4.5 不同区域各个函数大小关系呈现【draw_detail_area函数】

```python
# 定义符号 
# Define symbols
c_n, c_r, delta, e_n, e_r, p_e, E, k, b, alpha = symbols('c_n, c_r, delta, e_n, e_r, p_e, E, k, b, alpha')

# 四个表达式
# Four expressions
expressions = {
    r'$\pi_r^{NW}$': E*p_e+(k*(alpha*delta*(c_n+e_n*p_e)-(c_r+e_r*p_e))**2)/(8*(k+alpha*delta*(1-alpha*delta))**2), 
    r'$\pi_r^{BW}$': E*p_e + ( k*(delta*(c_n+e_n*p_e)-(c_r+e_r*p_e+b))**2 )/( 8*(k+delta-delta**2)**2), 
    r'$\pi_r^{NS}$': E*p_e + ((k+2*alpha*delta)*(alpha*delta*(c_n+e_n*p_e)-(c_r+e_r*p_e))**2 )/( 8*(k+alpha*delta*(2-alpha*delta))**2),
    r'$\pi_r^{BS}$': E*p_e + ( (k+2*delta)*(delta*(c_n+e_n*p_e)-(c_r+e_r*p_e+b))**2 )/( 8*(k+2*delta-delta**2)**2),
}

# 参数赋值
# Parameter assignment
assigns = {c_n: 0.2, c_r: 0.1, delta: 0.8, e_n: 1, e_r: 0.6, p_e: 0.1, E: 2, k: 1.1}

# 要分析的参数，及其取值范围
# The parameters to be analyzed and their value ranges.
the_var_x = alpha
start_end_x = [0.7, 0.8]  # [起始值, 终止值]。 [starting value, ending value].
the_var_y = b
start_end_y = [0, 0.08]  # [起始值, 终止值]。 [starting value, ending value].

# xy轴的名字
# The names of the x-axis and y-axis.
x_name = '$\\alpha$ \n (b) With blockchain' 
y_name = r'$b$'  

# 图片保存路径、文件名
# Picture save path and file name.
save_dir = r'max_area_detail.tiff' 

# 每个关系区域的标签前缀、编号样式、背景颜色和图案。
# The label prefix, numbering style, background color and pattern of each relational area.
prefix=r'Region'  # 前缀。可以是"区域"也可以是"Region"，默认"Region"。
numbers='roman' # 序号标记风格。有三种可选："roman", "letter" 和"number"，分别表示罗马数字、大写英文字母和阿拉伯数字。Numbering style. There are three options: "roman", "letter", and "number".
colors = ['#dae3f3', '#fbe5d6', '#e2f0d9', '#ededed', 'yellow', '#adb9ca', 'white']
patterns = [' ', '+', '\\', '-', '//', '|', 'o']

# 其他设置
text_fsize_add = -2 # 区域标签字号增量。 Increment of regional label font size.
figsize=[7, 4] # 图片大小：宽5高4。 icture size: width 5, height 4.
xrotation=0 # x轴标签名旋转角度（0为不旋转）。 Rotation angle of x-axis label name (0 means no rotation).
yrotation=0 # y轴标签名旋转角度（0为不旋转）。 Rotation angle of y-axis label name (0 means no rotation).
linewidths=0.1 # 线粗0.1. Line thickness: 0.1.

# x/y轴名字标签距离横轴刻度的距离
xlabelpad = 3
ylabelpad = 17


# 自定义坐标轴字体大小
xlabelsize = 8 # 横轴字大小，默认'auto'，自动和fsize一样大
ylabelsize = 29 # 纵轴字大小，默认'auto'，自动和fsize一样大
legendsize = 9 # 图例字大小，默认'auto'，自动和fsize一样大

# 标签背景色和位置偏移自定义设置，默认'auto'自动
pattern_colors = ['#dae3f3', 'white', 'none', 'auto']  # 分别为NW,BW,NS,BS设置标签背景色，'auto'为自动，'none'为透明
pattern_moves = [(+0.005, +0.01), (+0, +0.005), (0, 0), (0, 0)]  # 分别为NW,BW,NS,BS设定区域标签较原来的偏移量，(x方向，y方向)


# 传给draw_detail_area函数（不要改！）
# Passed to the draw_detail_area function (Don't change!).
draw_detail_area(expressions=expressions, assigns=assigns, 
                the_var_x=the_var_x, start_end_x=start_end_x, 
                the_var_y=the_var_y, start_end_y=start_end_y, 
                x_name=x_name, y_name=y_name, 
                fsize=14, text_fsize_add=text_fsize_add,
                save_dir=save_dir, figsize=figsize, colors=colors, patterns=patterns,
                xrotation=xrotation, yrotation=yrotation, linewidths=linewidths,
                prefix=prefix, numbers=numbers, xlabelsize=xlabelsize, ylabelsize=ylabelsize, legendsize=legendsize, 
              pattern_colors=pattern_colors, pattern_moves=pattern_moves, xlabelpad=xlabelpad, ylabelpad=ylabelpad)
```

<img src="https://pic1.zhimg.com/80/v2-fe7081df64749d15b517a61f48900c36_1440w.png?source=ccfced1a" alt="img" style="zoom:50%;" />

---

## 附录

### A. 附录A: LaTeX的使用口诀

> **下标下划线**，**上标冒尖尖**。 
>
> **希腊字母前**，**加上反斜线**。 
>
> **上下标字母多，花括号不能少**。  

适用范围：“表达式输入”的等号**左侧**（同时也是**图例**）、“x轴名称”、“y轴名称”、“z轴名称”、最大值区域标注。**用“\$   \$”括起来的地方，系统会识别为LaTeX**，如图：

![img](https://picx.zhimg.com/80/v2-5ea6f57da4fd4871681770a8ec0cbcdc_1440w.png?source=ccfced1a)

![img](https://picx.zhimg.com/80/v2-9ca281a2cdc4c4e6b1b5f2786961d0ac_1440w.png?source=ccfced1a)

![img](https://picx.zhimg.com/80/v2-1ecbb732574eb9c5639e5d84140acf95_1440w.png?source=ccfced1a)

> **下标下划线（\_）**，**上标冒尖尖**（^）。 【例如：\$p_a\$ 对应 $p_a$ ,\$a^b\$ 对应 $a^b$】
> 
> **希腊字母前**（如alpha），**加上反斜线**（\\）。 【例如：\$\alpha_1\$ 对应 $\alpha_1$，\$\gamma\$ 对应 $\gamma$】
> 
> **上下标字母多，花括号不能少**。【例如：\$\alpha\_{ab}\$ 对应 $\alpha_{ab}$, \$A\_{12}^{cd}\$ 对应 $A_{12}^{cd}$】

除了LaTeX需要注意外，还需要注意的是，如果坐标轴标注里想**换行**，在换行处直接打`\n`。例如：

```
$b$ \n (a) Parameter $b$
```

对应效果为：

![img](https://pica.zhimg.com/80/v2-6c5a43f02c3f7b4f33ce55a002e35783_1440w.png?source=ccfced1a)

### B. 附录B：颜色的表示

![img](https://picx.zhimg.com/80/v2-e9f4dcd2b84b7a159011000ff185f98a_1440w.png?source=ccfced1a)

针对需要进行颜色设置的地方，easyfig提供了颜色筛选器：

![img](https://picx.zhimg.com/80/v2-f004e43717e2a954f7546b7310ac68c0_1440w.png?source=ccfced1a)

当然，也可以输入特定颜色对应的单词去设置颜色，颜色及名称如下：

![img](https://picx.zhimg.com/80/v2-5f9910351cd67a4193ee9fdd7e42b388_1440w.png?source=ccfced1a)

![img](https://pic1.zhimg.com/80/v2-9c352749a9a644fb1aa65be668b833f2_1440w.png?source=ccfced1a)

甚至，你还可以利用截图工具，例如[Snipaste](https://zh.snipaste.com/)等，获取某个颜色的16进制值，如`#e9ac7d` ，直接粘贴到颜色名称下拉列表框内，即可为所欲为地设置颜色啦~

![img](https://picx.zhimg.com/80/v2-3e53fd470142698870a4f74250b81fca_1440w.png?source=ccfced1a)

![img](https://pic1.zhimg.com/80/v2-dabd9e3cf548a68f304abad7ae7cdf1f_1440w.png?source=ccfced1a)

### C. 附录C：线形的表示

![img](https://pic1.zhimg.com/80/v2-c7e56411c20cb9d1c5df256d0d732c0d_1440w.png?source=ccfced1a)

easyfig支持多种线形（线型），不局限于系统给出的下拉列表那些，用于可以自己输入。

以下是一些常见的线形及其对应的表示：

- '-'或'solid'：实线
- '--'或'dashed'：虚线
- ':'或'dotted'：点线
- '-.'或'dashdot'：点划线
- 'None'：无连接线，只显示标记
- (0, (5, 10))：短虚线
- (0, (10, 10))：长虚线
- (0, (5, 10, 15, 10))：长短虚线
- (0, (5, 10, 1, 10))：点划线
- (0, (1, 1))：密集虚线
- (0, (20, 10))：稀疏虚线
- (5, (10, 10))：**偏移虚线**

![img](https://pica.zhimg.com/80/v2-99be6a18e407ba2d9b7af2110935b7ea_1440w.png?source=ccfced1a)

### D. 附录D：区域条纹的表示

![img](https://picx.zhimg.com/80/v2-e12f4e2452613ab58f2af3e4223e66d0_1440w.png?source=ccfced1a)

对于"绘制模式比较图"和"绘制关系区域图"功能，easyfig支持多种区域条纹形状。本系统支持的区域条纹及其效果如下：

包括：

```
'xx', '--', '..', '||', '..', 'oo', '++', '**', '\\\\\\\\', '////', '-', 'x', '|', '.', 'o', '+', '*', '\\\\', '//', '---', 'xxx', '|||', '...', 'ooo', '+++', '***', '\\\\\\\\\\\\', '//////'。
```

![img](https://picx.zhimg.com/80/v2-1c155998b48b09776de1febdc10b9b4a_1440w.png?source=ccfced1a)

![img](https://picx.zhimg.com/80/v2-89d799b03a8d208579bb21d6b8bc6817_1440w.png?source=ccfced1a)

图案可重复使用以增加密度，例如\*\*、\*\*\*、\*\*\*\*\*。

![img](https://pic1.zhimg.com/80/v2-ab8cb54014812759ac4253633bf86f11_1440w.png?source=ccfced1a)

### E. 附录E：标记点形状

![img](https://picx.zhimg.com/80/v2-245e124ef34f60555d8ae21600ce2d25_1440w.png?source=ccfced1a)

对于"绘制仿真折线图"功能，easyfig支持多种标记点形状，例如，无标记点为None 。本系统支持的标记点及其效果如下：

![img](https://pic1.zhimg.com/80/v2-232e8bdc82cd425a30078925f94ce55e_1440w.png?source=ccfced1a)

![img](https://picx.zhimg.com/80/v2-0a35150035b535efb55ea1b7550a5223_1440w.png?source=ccfced1a)

### F. 附录F：3D图的视角

![img](https://pic1.zhimg.com/80/v2-bd831177af3449b72d9e425d98d7b11d_1440w.png?source=ccfced1a)

- 仰角 (elevation)：定义了观察者与 xy 平面之间的夹角，也就是观察者与 xy 平面之间的旋转角度。当elevation为正值时，观察者向上倾斜，负值则表示向下倾斜。默认15度。可根据美观与否微调。
- 方位角 (azimuth)：定义了观察者绕 z 轴旋转的角度。它决定了观察者在 xy 平面上的位置。azim 的角度范围是 −180 到 180 度，其中正值表示逆时针旋转，负值表示顺时针。默认45度。可根据美观与否微调。

![img](https://picx.zhimg.com/80/v2-f5b038dfd8b4ff26eae9fce0e5866470_1440w.png?source=ccfced1a)



## 更新日志

> 新版本2.5.0更新日志： 
>
> （1）修复了Mathematica分式/根式嵌套转换出错的Bug； 
>
> （2）增加Matlab代码转Sympy代码的功能； 
>
> （3）更改要分析的变量时，其他已赋值好的参数取值不变；
>
> （4）其他体验上的优化（如增大默认字号、默认保存双击即打开的文件）。
>
>  新版本3.7.0更新日志： 
>
> （1）data\_lines函数可在一张图中绘制长度不同的曲线。

项目链接：https://github.com/Jesse-tien/Easyfig

pip官方链接：https://pypi.org/project/easyfig/3.7.0/
