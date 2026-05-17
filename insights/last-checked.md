# 已追踪文章索引（截至2026年5月17日）

此文件用于记录已分析过的文章和产品页面状态，避免每日洞察重复覆盖。每日新增分析时更新此列表。

## blogs.nvidia.com 已追踪

- [x] GTC 2026 Live Updates (2026-03-16)
- [x] GTC 2026 Virtual Worlds Powering Physical AI Era (2026-03-16)
- [x] NVIDIA and Thinking Machines Lab Gigawatt Partnership (2026-03-10)
- [x] Physical AI Open Models and Frameworks (2026-03-16)
- [x] Driving Impact: Automotive Ecosystem Physical AI (2026-03-16)
- [x] Omniverse DSX Blueprint for AI Factory Digital Twins (2026-03-16)
- [x] State of AI Report 2026 (2026-03-09)
- [x] GeForce NOW March 2026 Games (2026-03-05)
- [x] GeForce NOW at GDC 2026 (2026-03-12)
- [x] National Robotics Week 2026 (2026-03-31)
- [x] GeForce NOW April 2026 Games (2026-04-02)
- [x] Jensen Huang at 3DEXPERIENCE World (2026-04-09)
- [x] Roche Scales NVIDIA AI Factories for Drug Discovery (2026-03-16)
- [x] GeForce NOW May 2026 Games (2026-05-01)
- [x] The Future of AI Is Open and Proprietary (2026-05-05)
- [x] NVIDIA Spectrum-X Ethernet MRC (2026-05-06)
- [x] Cisco and NVIDIA Advance Security for Enterprise AI Factories (2026-05-07)
- [x] Powering the Next American Century: Energy Secretary and NVIDIA (2026-05-07)
- [x] NVIDIA, Energy Leaders Accelerating Power-Flexible AI Factories (2026-05-07)
- [x] NVIDIA, Telecom Leaders Build AI Grids to Optimize Inference (2026-05)
- [x] NVIDIA Unveils New Open Models, Data and Tools to Advance AI (2026-05-13)
- [x] NVIDIA and Google Cloud Collaborate to Advance Agentic and Physical AI (2026-05-13)
- [x] HPE and NVIDIA Debut AI Factory Stack (2026-05-13)
- [x] NVIDIA DGX SuperPOD Sets the Stage for Rubin-Based Systems (2026-05-13)
- [x] NVIDIA Research Breakthroughs Put Advanced Robots in Motion / ICRA (2026-05)

## developer.nvidia.com 已追踪

- [x] Inside the NVIDIA Vera Rubin Platform (2026-03-16)
- [x] Design, Simulate, and Scale AI Factory with NVIDIA DSX Air (2026-03-16)
- [x] Building a Zero-Trust Architecture for Confidential AI Factories (2026-03-23)
- [x] Newton Adds Contact-Rich Manipulation for Industrial Robotics (2026-03-13)
- [x] Scale Synthetic Data with NVIDIA Cosmos World Foundation Models (2026-03-13)
- [x] NVIDIA RTX Innovations for Game Development (2026-03-12)
- [x] Stream High-Fidelity Spatial Computing with CloudXR 6.0 (2026-03-25)
- [x] Designing Protein Binders Using Proteina-Complexa (2026-03-25)
- [x] MiniMax M2.7 Advances Scalable Agentic Workflows (2026-04-11)
- [x] Bringing AI Closer to Edge and On-Device with Gemma 4 (2026-04-02)
- [x] Achieving Single-Digit Microsecond Latency for Capital Markets (2026-04-02)
- [x] CUDA Tile Programming for BASIC (2026-04-01)
- [x] Optimize Supply Chain Decision Systems Using NVIDIA cuOpt Agent Skills (2026-04-30)
- [x] Speed Up Unreal Engine NNE Inference with NVIDIA TensorRT for RTX Runtime (2026-04-30)
- [x] Building for the Rising Complexity of Agentic Systems with Extreme Co-Design (2026-05-04)
- [x] How to Build In-Vehicle AI Agents with NVIDIA: From Cloud to Car (2026-05-05)
- [x] Model Quantization: Post-Training Quantization Using NVIDIA Model Optimizer (2026-05-07)
- [x] Building the AI Grid with NVIDIA: Orchestrating Intelligence Everywhere (2026-05)

## nvidia.cn/networking/ethernet-switching 产品基线（2026-05-17）

当前产品线状态，后续对比此基线检测变更：

### Spectrum-4 系列
- SN5600：64端口 800GbE，51.2Tb/s 吞吐量，2U 机架式，支持 RoCE/Spectrum-X
- 定位：AI 工厂 smart-leaf / spine / super-spine 交换机

### Spectrum-X Photonics（预计 2026 下半年）
- 128端口 800Gb/s 或 512端口 200Gb/s，100Tb/s 总带宽
- 512端口 800Gb/s 或 2048端口 200Gb/s，400Tb/s 总带宽
- 共封装光学（CPO）+ 硅光子引擎
- 较传统方式：4x 更少激光器、3.5x 更高能效、10x 更高网络弹性、5x 更长无中断运行时间

### Spectrum-6 系列（2026 新增）
- SN6810：128端口 800GbE，102.4Tb/s 吞吐量，CPO 硅光子集成（32 个 1.6Tb/s 光引擎，Micro Ring Modulator）
- SN6800：512端口 800GbE，409.6Tb/s 吞吐量
- 能效约为传统可插拔光模块方案的 5 倍
- Cisco N9100 交换机搭载 Spectrum-6 芯片供货

### 配套软件/SDK
- Cumulus Linux / NetQ 5.1（Spectrum-X 参考架构 2.1 认证）
- NVIDIA Ethernet Switch SDK / SAI
- DOCA / BlueField DPU 集成
- MRC（Multipath Reliable Connection）协议：开放 OCP 规范，多路径 RDMA 传输，已部署于 OpenAI/Microsoft/Oracle
