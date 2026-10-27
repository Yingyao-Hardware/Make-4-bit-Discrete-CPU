# My-4-Bit-Discrete-CPU (基于纯分立元件的4位CPU)

> A 4-bit-CPU Core from scratch using discrete transistors (Note: No ICs).
> **我是大一2026级新生，这个项目是我在课余时间制作的。我将独立设计、推演并打板CPU项目。由于预算有限，我只能使用嘉立创每月两次的免费打板额度，且打样过程中也可能出现坏板。但无论成功还是失败，我都会积极地和大家分享整个过程！**
> *(I am a 2026 freshman, and this project is built in my spare time. I will independently design, deduce, and fabricate this CPU. Due to a limited budget, I can only rely on JLC's free PCB prototyping quota (twice a month), and failed boards during the process are inevitable. However, I will actively share the entire journey with you, whether it's a success or a failure!)*

 ## 💬 反馈与交流 (Feedback & Communication)

**作为一名硬件初学者，我的设计水平还有很大的提升空间。如果大家在原理图、PCB走线或代码逻辑上发现任何问题，或者有更好的建议，非常欢迎通过 Issues 向我提出！我会虚心学习，并尽我最大的努力去修正。感谢大家的支持！**
*(As a hardware beginner, my design skills still have much room for improvement. If you find any problems in the schematics, PCB routing, or code logic, or if you have any better suggestions, please feel free to bring them up via Issues! I will humbly learn from them and try my best to make corrections. Thank you for your support!)*

## 🚧 项目状态 (Project Status)
**v0.1-alpha 早期原型版**：目前正在 PCB 打样与实物焊接阶段，可能存在尚未发现的逻辑 Bug，将持续更新。
*(Early Prototype: Currently undergoing PCB fabrication and hardware assembly. There may be undiscovered logic bugs, and updates will be continuous.)*

## 🧩 已完成模块 (Completed Modules)
- **4-bit ALU (加/减法核心)**: 基于逻辑门与分立三极管搭建，独立推演拓扑连线。
  *(4-bit ALU: Built with logic gates and discrete transistors, topology independently deduced.)*
- **4-bit ACC Register (累加寄存器核心)**: 基于 4 个 D 触发器构成的存储单元。
  *(4-bit ACC Register: A storage unit composed of 4 D-Flip-Flops.)*

## 📁 项目文件格式说明 (Project File Formats)
本项目使用 **嘉立创 EDA 专业版 (EasyEDA Pro)** 进行开发。
*(This project is designed using EasyEDA Pro.)*

- **嘉立创 EDA 用户 (For EasyEDA Pro Users)**: 可以直接下载并使用源工程文件（`.epro`），导入到自己的工程中查看或修改。
  *(You can directly download and import the source project file (.epro) into your own EasyEDA Pro workspace for viewing or modification.)*
- **非嘉立创用户 (For Other EDA Users, e.g., Altium, KiCad)**: 由于软件生态限制，你可以使用通用的 **Gerber 文件** 进行生产制造，并使用 **PDF 格式的原理图** 查看电路逻辑。
  *(Due to software ecosystem limitations, you can use the universal Gerber files for manufacturing and view the circuit logic via PDF schematics.)*

## 🛠️ 踩坑日记 (Debugging Log)
- 发现使用 10K 电阻驱动三极管基极会导致无法翻转，已更改为 1K-4.7K 解决扇出问题。
  *(Discovered that using a 10K resistor to drive the transistor base causes failure to toggle. Changed to 1K-4.7K to fix it.)*
