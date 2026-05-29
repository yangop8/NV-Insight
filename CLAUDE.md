# CLAUDE.md

## 项目概述

NV-Insight 是 NVIDIA 官方博客的每日洞察快讯项目，跟踪 NVIDIA 最新技术动态，面向网络、嵌入式软件、系统软件方向提供分析观点。

## 数据源

每日分析以下网址的新内容：
- https://blogs.nvidia.com/
- https://developer.nvidia.com/blog/recent-posts/
- https://www.nvidia.cn/networking/ethernet-switching/ （更新频率较低，产品页面有变动时分析）

## 每日工作流程

1. 使用 WebSearch/WebFetch 抓取三个数据源的最新文章
2. 读取 `insights/last-checked.md`，对比已追踪列表，**仅筛选 URL 不在索引中的净新增文章**
3. **如果没有净新增文章，直接报告"今日无新增内容"并结束，不生成空文件**
4. 针对净新增内容撰写洞察快讯，保存为 `insights/YYYY-MM-DD.md`
5. 将新文章（标题 + 日期）追加到 `insights/last-checked.md`
6. 提交并推送到 **main** 分支（不使用功能分支）

### 增量去重规则（关键）

- **去重依据**：文章 URL（去除尾部斜杠和 URL 编码差异后比对）
- **已在 `last-checked.md` 中的文章一律跳过**，不得重复分析
- **每条快讯只分析该文章一次**，后续日期不再重复
- 月度/阶段汇总可引用已追踪文章做综合分析，但每日快讯不得重复
- 如果某日所有新文章均已追踪，**直接跳过该日**，不生成文件

## 快讯撰写规则

- **字数限制**：【快讯内容】100字以内
- **格式固定**：
  ```
  【快讯内容】
  <概括新发布的关键内容>

  【观点】
  <面向网络、嵌入式软件、系统软件方向的分析>

  > 参考文章：[文章标题](具体文章URL)
  ```
- **必须附具体链接**：每条快讯必须附上对应文章的具体 URL（如 `https://blogs.nvidia.com/blog/具体文章路径/`），不得使用数据源首页地址，以便溯源核实、防止幻觉
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
    ├── monthly-summary-YYYY-MM-DD-to-MM-DD.md     # 月度汇总
    ├── incremental-YYYY-MM-DD-to-MM-DD.md          # 阶段增量汇总（去重后）
    ├── YYYY-MM-DD.md                               # 每日快讯（仅含当日净新增）
    └── last-checked.md                             # 已追踪文章索引（去重权威源）
```

## 注意事项

- blogs.nvidia.com 和 developer.nvidia.com 可能返回 403，优先使用 WebSearch 搜索最新文章
- nvidia.cn/networking 为产品页面，更新频率较低，每次检查时对比产品型号/规格变化即可
- GeForce NOW 游戏列表等纯消费类内容可简要提及但不作为观点分析重点
- 月度汇总按自然周拆分，每周独立撰写快讯和观点
- **所有操作在 main 分支进行**，不使用功能分支，确保 `last-checked.md` 始终是最新的增量基准
- **每次运行前必须先读 `last-checked.md`**，严格按 URL 去重，杜绝重复分析
