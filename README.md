# Embodied-Learning-Operator-ELO-
具身学习操控器
该机械臂摇操系统采用 AS5600 磁编码器和 ESP32 控制平台构建。
系统通过四路磁编码器实时采集关节角度变化，ESP32 对数据进行处理后以蓝牙广播方式发送至上位机或移动终端。
终端接收数据并将关节角映射至三维仿真环境，实现摇操系统与虚拟模型的同步交互。
This robotic arm teleoperation system is built using AS5600 magnetic encoders and the ESP32 control platform.
The system collects real-time joint angle changes through four magnetic encoder channels, and the ESP32 processes the data and broadcasts it via Bluetooth to a host device or mobile terminal.
The terminal receives the data and maps the joint angles into a 3D simulation environment, achieving synchronized interaction between the teleoperation system and the virtual model.

该机械臂控制系统在启动阶段实现物理世界向仿真世界的状态映射；
在工作阶段，当在仿真环境中输入目标关节角时，系统可将指令由仿真世界映射回物理世界，从而驱动真实机械臂动作。
同时支持通过鼠标拖拽与键盘指令对机械臂进行控制。
During the initialization phase, the robotic arm control system maps the state of the physical world to the simulation environment.
During operation, when a target joint angle is entered in the simulation environment, the system maps the command back to the physical world to drive the real robotic arm.
The system also supports robotic arm control through mouse dragging and keyboard input.
