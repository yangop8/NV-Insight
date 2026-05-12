# 已追踪文章索引（截至2026年5月12日）

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
- [x] Nemotron 3 Nano Omni Multimodal AI Agents (2026-04-28)
- [x] Spectrum-X Ethernet MRC for Gigascale AI (2026-05-06)
- [x] GeForce NOW May 2026 Games (2026-05-01)
- [x] GFN Thursday May 6 - 61 Games (2026-05-06)
- [x] Gaijin SSO on GeForce NOW (2026-04-24)
- [x] GFN Thursday April 29 New Features (2026-04-29)
- [x] Energy Secretary Chris Wright and Ian Buck Genesis Mission (2026-04-22)
- [x] The Future of AI Is Open and Proprietary (2026-04-17)

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
- [x] Building for the Rising Complexity of Agentic Systems with Extreme Co-Design (2026-05-05)
- [x] How NVIDIA Dynamo 1.0 Powers Multi-Node Inference at Production Scale (2026-05-05)
- [x] Accelerating LLM and VLM Inference for Automotive and Robotics with TensorRT Edge-LLM (2026-04-22)
- [x] Build Next-Gen Physical AI with Edge-First LLMs for Autonomous Vehicles and Robotics (2026-04-22)
- [x] Reimagining LLM Memory: Context as Training Data for Test-Time Learning (2026-04-25)
- [x] Real-Time Performance Monitoring with NCCL Inspector and Prometheus (2026-05-05)
- [x] Achieving Peak Efficiency on GB200 NVL72 with Slurm Block Scheduling (2026-05-07)
- [x] Model Quantization: Post-Training Quantization Using NVIDIA Model Optimizer (2026-05-07)
- [x] Delivering Flexible Performance for Data Centers with NVIDIA MGX (2026-04-18)
- [x] Open Source AI Tool Upgrades Speed Up LLM and Diffusion Models on RTX PCs (2026-04-20)
- [x] Integrate Physical AI Capabilities with NVIDIA Omniverse Libraries (2026-04-08)
- [x] Mitigating Indirect Injection Attacks in Agentic Environments (2026-04-20)
- [x] Build a Secure Local AI Agent with OpenClaw and NemoClaw (2026-04-17)
- [x] Nemotron 3 Nano Omni Powers Multimodal Agent Reasoning (2026-04-28)

## nvidia.cn/networking/ethernet-switching 产品基线（2026-05-12）

当前产品线状态，后续对比此基线检测变更：

### Spectrum-4 系列
- SN5600：64端口 800GbE，51.2Tb/s 吞吐量，2U 机架式，支持 RoCE/Spectrum-X
- 定位：AI 工厂 smart-leaf / spine / super-spine 交换机

### Spectrum-X Photonics（预计 2026 下半年）
- 128端口 800Gb/s 或 512端口 200Gb/s，100Tb/s 总带宽
- 512端口 800Gb/s 或 2048端口 200Gb/s，400Tb/s 总带宽
- 共封装光学（CPO）+ 硅光子引擎
- 较传统方式：4x 更少激光器、3.5x 更高能效、10x 更高网络弹性、5x 更长无中断运行时间

### Spectrum-X MRC（2026-05 新增）
- MRC（Multipath Reliable Connection）：开放 RDMA 传输协议，单连接跨多路径负载均衡
- 支持多平面网络架构（Multiplane），硬件加速跨平面负载均衡
- 通过 OCP 发布开放规范，AMD/Broadcom/Intel/Microsoft/OpenAI 参与
- OpenAI 用于 ChatGPT/Codex 训练，Microsoft/Oracle 大规模 AI 工厂部署

### 配套软件/SDK
- Cumulus Linux / NetQ 5.1（Spectrum-X 参考架构 2.1 认证）
- NVIDIA Ethernet Switch SDK / SAI
- DOCA / BlueField DPU 集成
