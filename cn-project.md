---
layout: page
permalink: /cn/project/index.html
title: 项目经历
lang: zh
---

# 科研项目

<br>

#### [多杆接卸式星壤钻探机器人](#)

<center>
<img src="/images/projects/multi-rod-prototype.png" alt="多杆接卸式钻探机器人样机 — 四阶段运行序列">
</center>
<p class="img-caption">加杆循环作业样机执行过程剪影</p>

面向地外深层取样任务，独立完成**控制系统构建**、**运动规划**、**力学建模**、**深度学习**四领域全栈研发，通过实验端到端验证。

- **角色** &mdash; 项目主持人 · 硕士课题 · 杰青项目
- **实验室** &mdash; 广东工业大学仿生与智能机器人实验室
- **时间** &mdash; 2023.06 &ndash; 至今

**核心贡献**

1. **控制系统** &mdash; 构建9自由度钻探机器人 EtherCAT + Modbus 双总线测控平台，上位机实现5线程并行架构 + 7态FSM流程管理 + 安全防护
2. **运动规划** &mdash; 将钻杆协同作业建模为RCPSP问题，使用 Petri 网 + MILP + CP-SAT 求解多根钻管全局最优排序（提升 &ge;4.9%）
3. **力学建模** &mdash; 提出多分量耦合机土力学模型（Janssen + Terzaghi + PFRT + Coulomb），实验验证预测偏差 &plusmn;18%，解决跨重力难题
4. **深度学习** &mdash; 构建物理引导的深度学习分类模型，引入物理先验力比特征，跨域迁移识别准确率 F1&nbsp;=&nbsp;0.736（对比基线 +16.7pp）
5. **虚拟仿真** &mdash; 基于 Unity 构建 9 自由度整机数字孪生平台，将 Petri 网 / RCPSP 调度器以 task 级映射到脚本化作业序列（Stage A 首根对接 / Stage B 加杆循环），支持调度算法无风险验证与操作培训

<div class="img-row">
<img src="/images/projects/multi-rod-architecture.png" alt="EtherCAT + Modbus 双总线控制架构">
<img src="/images/projects/multi-rod-prfinet.png" alt="PRFINet — 物理引导深度学习架构">
</div>
<p class="img-caption">左：双总线测控系统架构 &nbsp;&middot;&nbsp; 右：PRFINet 深度学习模型</p>

<center>
<img src="/images/projects/multi-rod-unity-sim.png" alt="Unity 虚拟样机 — 钻进与备杆并发执行序列">
</center>
<p class="img-caption">虚拟样机在仿真中钻进与备杆并发执行</p>

**技术栈** &mdash; `EtherCAT` `Modbus` `Qt / C++` `PyTorch` [`OR-Tools`](https://developers.google.com/optimization) `Petri Net` `SQLite` `Optuna` `Unity` `C#`

**成果** &mdash; 实物样机1台、Unity 虚拟样机1套、发明专利2项（授权1）、软著1项、ICIEA会议论文1篇、SCI论文2篇

<br>

---

#### [真空低温钻具测温系统](#)

<center>
<img src="/images/projects/vacuum-cryogenic-drill.png" alt="集成热电偶的水冰钻样机">
</center>
<p class="img-caption">集成热电偶的水冰钻样机</p>

<div class="img-row">
<img src="/images/projects/thermocouple-install.png" alt="螺旋钻头热电偶嵌入">
<img src="/images/projects/temp-scanner-board.png" alt="多通道温度巡检仪电路板">
</div>
<p class="img-caption">左：螺旋钻头热电偶嵌入 &nbsp;&middot;&nbsp; 右：多通道温度巡检仪</p>

承接航天院所委托，完成&minus;190&nbsp;&deg;C 真空环境下月球水冰钻测温系统的**方案设计**、**硬件软件开发**与**机械改造全链路交付**。

- **角色** &mdash; 系统总设 · 项目主持人
- **委托方** &mdash; [北京卫星制造厂（529厂）](http://www.spacechina.com/)
- **时间** &mdash; 2025.07 &ndash; 至今

**核心贡献**

1. **方案设计** &mdash; 针对真空低温极端工况，提出10路极微热电偶嵌入缠绕复合方案，配套滑环电连接与防磨结构
2. **硬件开发** &mdash; 基于 STM32G030 + ZAM6218 设计多通道温度巡检仪，Modbus / RS-485 通信
3. **软件开发** &mdash; 跨平台采集软件，支持100&nbsp;Hz高频采集、500万数据点处理、多点校准拟合与CSV导入导出
4. **热学校核** &mdash; 基于热阻-热容等效原理构建钻具热模型，配合 [SolidWorks](https://www.solidworks.com/) Simulation 完成热-结构耦合校核

**技术栈** &mdash; `STM32` `ZAM6218` `Modbus RTU` `RS-485` `Tauri` `Web Serial API` `热阻-热容建模`

**成果** &mdash; 测温水冰钻样机1套、测温系统1套、软著1项、发明专利1项

<br>

---

#### [紧凑型 EtherCAT 伺服驱动器](#)

<div class="img-row">
<img src="/images/projects/motor-driver.png" alt="紧凑型伺服驱动器 PCB">
<img src="/images/projects/motor-driver-assembled.png" alt="装配完成的伺服驱动器">
</div>
<p class="img-caption">左：三相逆变器 PCB &nbsp;&middot;&nbsp; 右：装配完成的驱动器（含EtherCAT模块）</p>

面向无刷电机的紧凑型高性能伺服驱动器，作为多杆钻探机器人的执行器控制单元。实现FOC矢量控制与EtherCAT实时通信，支持多轴协同运动。

- **角色** &mdash; 硬件与固件开发
- **时间** &mdash; 2024.09 &ndash; 至今
- **平台** &mdash; STM32、三相MOSFET逆变器、磁编码器（SPI）、EtherCAT从站模块

**核心贡献**

1. **硬件设计** &mdash; 设计紧凑型4层PCB，集成三相逆变器、电流采样、磁编码器接口、EtherCAT通信模块与OLED显示
2. **FOC算法** &mdash; 实现Park/Clarke变换的磁场定向控制，20 kHz PWM电流环，支持力矩/速度/位置级联控制模式
3. **EtherCAT集成** &mdash; 通过SPI接口的EtherCAT从站实现确定性实时通信，支持钻探机器人多轴同步运动
4. **标定与诊断** &mdash; 开发电机参数自识别、编码器标定程序，以及命令行调试终端

**技术栈** &mdash; `STM32` `FOC` `EtherCAT` `FreeRTOS` `SPI` `CAN` `PCB设计`

**成果** &mdash; 功能驱动板1块，已集成至钻探机器人控制系统

<br>

---

#### [航天员便携折叠式手持钻机](#)

<center>
<img src="/images/projects/portable-folding-drill.png" alt="便携折叠式手持钻机样机">
</center>

面向航天员取芯作业的可折叠手持钻台，具备自动进给、紧凑三折结构和极端环境耐受能力。

- **角色** &mdash; 机械设计与驱动系统选型
- **委托方** &mdash; [北京卫星制造厂（529厂）](http://www.spacechina.com/)
- **时间** &mdash; 2025.03 &ndash; 2025.06
- **关键工作** &mdash; 绳驱自动进给模块、三折式架体设计、电机/驱动选型（Maxon + Elmo）、仿真强度与刚度校核
- **成果** &mdash; 工程样机1台，通过地面测试验证

<br>

---

# 实习经历

<br>

#### [中国空间技术研究院 · 北京卫星制造厂（529厂）](http://www.spacechina.com/)

**工程系统研发实习生** &nbsp;&middot;&nbsp; 2025.06 &ndash; 2025.09

- 承担钻具在真空低温环境下的测温系统软硬件开发
- 独立设计热电偶集成方案并完成真空罐实验装调
- 编写上位机采集软件，支持多通道实时可视化
- 负责三维建模、试验协调及技术文档撰写

<br>

#### 广州质量监督检测研究院 · 机电消防检验部

**质量检测部门实习生** &nbsp;&middot;&nbsp; 2023.08 &ndash; 2023.09

- 使用光学测厚仪测量电缆绝缘与护套材料厚度
- 按国标进行拉伸、抗开裂、热老化及延展性等性能测试
- 在标准环境下测量电阻，整理实验数据并参与质检报告撰写
