# NV-Insight

NVIDIA 官方博客每日洞察快讯，面向**网络、嵌入式软件、系统软件**方向的技术跟踪与分析。

## 信息来源

| 来源 | 网址 | 更新频率 |
|------|------|----------|
| NVIDIA Blog | https://blogs.nvidia.com/ | 每日 |
| NVIDIA Developer Blog | https://developer.nvidia.com/blog/recent-posts/ | 每日 |
| NVIDIA 以太网交换机 | https://www.nvidia.cn/networking/ethernet-switching/ | 较低（产品页面） |

## 快讯格式

每篇快讯固定格式如下：

```
【快讯内容】
<100字以内，概括当日/当周新发布的关键内容>

【观点】
<面向网络、嵌入式软件、系统软件方向的分析>
<如无相关内容，写：没有面向网络、嵌入式软件、系统软件的参考价值>
```

## 目录结构

```
insights/
├── monthly-summary-YYYY-MM-DD-to-MM-DD.md   # 月度汇总（按周拆分）
├── YYYY-MM-DD.md                             # 每日洞察快讯
└── last-checked.md                           # 已追踪文章索引（去重用）
```

## 工作流程

1. 每日抓取各网站的最新文章
2. 对比 `last-checked.md` 已追踪列表，筛选**新增内容**
3. 撰写100字以内快讯（【快讯内容】+【观点】）
4. 观点聚焦**网络、嵌入式软件、系统软件**三个方向，无关则明确标注
5. 更新 `last-checked.md`，提交推送

## 关注方向说明

| 方向 | 关注点 |
|------|--------|
| 网络 | 数据中心网络架构（NVLink/InfiniBand）、DOCA/BlueField DPU、Spectrum以太网交换机（SN5600/Spectrum-X Photonics）、共封装光学/硅光子、网络安全、低延迟通信协议、网络拓扑仿真 |
| 嵌入式软件 | Jetson平台、边缘/端侧AI推理、模型量化、实时系统、安全关键系统认证 |
| 系统软件 | GPU驱动/固件、多芯片调度、内核优化（vLLM/SGLang）、物理引擎、运行时沙箱、系统级性能优化 |
