# CLAUDE.md

## 项目概述

NV-Insight 是 NVIDIA 官方博客的每日洞察快讯项目，跟踪 NVIDIA 最新技术动态，面向网络、嵌入式软件、系统软件方向提供分析观点。

## 数据源

每日分析以下网址的新内容：
- https://blogs.nvidia.com/
- https://developer.nvidia.com/blog/recent-posts/
- https://www.nvidia.cn/networking/ethernet-switching/ （更新频率较低，产品页面有变动时分析）

## 每日工作流程

1. 使用 WebSearch/WebFetch 抓取两个网站的最新文章
2. 读取 `insights/last-checked.md`，对比已追踪列表，筛选出新增文章
3. 针对新增内容撰写洞察快讯，保存为 `insights/YYYY-MM-DD.md`
4. 将新文章追加到 `insights/last-checked.md`
5. 提交并推送到当前工作分支

## 快讯撰写规则

- **字数限制**：【快讯内容】100字以内
- **格式固定**：
  ```
  【快讯内容】
  <概括新发布的关键内容>

  【观点】
  <面向网络、嵌入式软件、系统软件方向的分析>
  ```
- **观点方向**：必须从网络、嵌入式软件、系统软件角度分析
- **无关内容**：如当日内容与三个方向均无关，观点直接写"没有面向网络、嵌入式软件、系统软件的参考价值"
- **参考文章**：在快讯末尾附上引用文章的标题和链接

## 观点关注的技术领域

### 网络
- 数据中心网络架构（NVLink、InfiniBand、RoCE）
- DOCA SDK / BlueField DPU
- Spectrum 以太网交换机系列（Spectrum-4/SN5600、Spectrum-X Photonics）
- 网络安全与零信任架构
- 低延迟网络通信协议
- AI工厂网络拓扑仿真
- 共封装光学（CPO）与硅光子技术

### 嵌入式软件
- Jetson 平台（AGX Thor/Orin）
- 边缘/端侧 AI 推理部署
- 模型量化与内存优化
- 实时操作系统与调度
- 安全关键系统（Safety-critical）认证

### 系统软件
- GPU 驱动与固件
- 多芯片/多节点调度
- 推理引擎内核优化（vLLM、SGLang、TensorRT）
- 开源物理引擎（Newton）
- 运行时安全（沙箱、进程隔离）
- 系统级性能分析与优化

## 文件结构

```
NV-Insight/
├── README.md
├── CLAUDE.md
└── insights/
    ├── monthly-summary-YYYY-MM-DD-to-MM-DD.md   # 月度汇总
    ├── YYYY-MM-DD.md                             # 每日快讯
    └── last-checked.md                           # 已追踪文章索引
```

## 注意事项

- blogs.nvidia.com 和 developer.nvidia.com 可能返回 403，优先使用 WebSearch 搜索最新文章
- nvidia.cn/networking 为产品页面，更新频率较低，每次检查时对比产品型号/规格变化即可
- GeForce NOW 游戏列表等纯消费类内容可简要提及但不作为观点分析重点
- 月度汇总按自然周拆分，每周独立撰写快讯和观点
