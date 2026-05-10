# 已追踪文章索引（截至2026年5月10日）

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
- [x] The Future of AI Is Open and Proprietary (2026-03-25)
- [x] NVIDIA and Partners Showcase the Future of AI-Driven Manufacturing at Hannover Messe 2026 (2026-04-20)
- [x] NVIDIA Partners With AI Infrastructure Ecosystem to Unveil Reference Design for Giga-Scale AI Factories (2026-05-06)
- [x] Powering the Next American Century: US Energy Secretary Chris Wright and NVIDIA's Ian Buck on the Genesis Mission (2026-05-07)
- [x] GeForce NOW May 2026 Games (2026-05-07)

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
- [x] How to Build In-Vehicle AI Agents with NVIDIA: From Cloud to Car (2026-05-05)
- [x] Winning a Kaggle Competition with Generative AI–Assisted Coding (2026-05-05)
- [x] Model Quantization: Post-Training Quantization Using NVIDIA Model Optimizer (2026-05-07)
- [x] Real-Time Performance Monitoring and Faster Debugging with NCCL Inspector and Prometheus (2026-05-07)

## nvidia.cn/networking/ethernet-switching 产品基线（2026-05-10）

当前产品线状态，后续对比此基线检测变更：

### Spectrum-4 系列
- SN5600：64端口 800GbE，51.2Tb/s 吞吐量，2U 机架式，支持 RoCE/Spectrum-X
- 定位：AI 工厂 smart-leaf / spine / super-spine 交换机

### Spectrum-X Photonics（预计 2026 下半年）
- 128端口 800Gb/s 或 512端口 200Gb/s，100Tb/s 总带宽
- 512端口 800Gb/s 或 2048端口 200Gb/s，400Tb/s 总带宽
- 共封装光学（CPO）+ 硅光子引擎
- 较传统方式：4x 更少激光器、3.5x 更高能效、10x 更高网络弹性、5x 更长无中断运行时间

### Spectrum-XGS（新增，2026-05-10 确认）
- Spectrum-X 平台的 scale-across 扩展技术
- 支持跨分布式数据中心互联，将多个数据中心整合为统一 AI 超级工厂
- 距离自适应拥塞控制、精确延迟管理、端到端遥测
- NCCL 性能提升近一倍
- 已作为 Spectrum-X 平台的一部分正式上线

### 配套软件/SDK
- Cumulus Linux / NetQ 5.1（Spectrum-X 参考架构 2.1 认证）
- NVIDIA Ethernet Switch SDK / SAI
- DOCA / BlueField DPU 集成
