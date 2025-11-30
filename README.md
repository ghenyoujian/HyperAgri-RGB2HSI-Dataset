# HyperAgri-RGB2HSI-Dataset

---

## 项目简介（Overview）

**HyperAgri-RGB2HSI** 是一个面向农业应用场景的开源高光谱数据集。  
本数据集基于公开可用的农作物 **RGB 图像数据集**，通过自研的 **RGB → 高光谱（HSI）重建算法** 生成对应的高光谱立方体数据，从而构建统一、规范、可复用的农业多模态数据资源。

该数据集旨在为以下研究方向提供基础数据支持：

- 农作物病害识别与分级  
- 杂草 / 作物目标检测与分割  
- 高光谱重建与跨模态生成建模  
- 精准农业中的光谱分析与智能决策  

> 本 GitHub 仓库仅提供数据集说明、结构与许可证信息，**实际数据文件托管于百度网盘**。

---

## 数据集概况（Dataset Summary）

| 项目 | 内容 |
|------|------|
| **数据集名称** | HyperAgri-RGB2HSI |
| **原始 RGB 数据集** | DeepWeeds、Global Wheat Head Dataset 2021 (GWHD 2021) |
| **发布日期** | 2025-12-01 |
| **任务类型** | 图像分类、分割、目标检测、高光谱重建 |
| **数据模态** | RGB、HSI、高光谱标注（可选） |
| **空间分辨率** | 保持原始 RGB 图像分辨率 |
| **光谱通道数** | 31 Bands（400–760 nm） |
| **数据格式** | `.mat` |
| **许可证** | CC BY 4.0（高光谱衍生部分）＋ 上游数据集各自许可证 |

---

## 数据下载（Download）

数据集通过 **百度网盘（Baidu Netdisk）** 提供下载：

- **数据集名称**：`HyperAgri-RGB2HSI-Dataset`
- **下载链接**：  
  https://pan.baidu.com/s/108FijCjdtrMED6J_9UHFtQ?pwd=87y1
- **提取码**：`87y1`

下载后请在本地解压使用，建议保持原始目录结构以避免路径错误。

---

## 目录结构（Directory Structure）

解压数据后，推荐的目录结构如下：

```text
HyperAgri-RGB2HSI/
├─ README.md
├─ LICENSE
├─ deepweeds/
│  ├─ rgb/            # 原始 RGB 图像
│  ├─ hsi/            # 重建后的高光谱数据（.mat）
│  └─ labels/         # 类别标签（杂草类别）
├─ gwhd2021/
│  ├─ rgb/            # 原始小麦穗 RGB 图像
│  ├─ hsi/            # 重建后的高光谱数据（.mat）
│  └─ labels/         # 检测/标注信息
└─ metadata/
   ├─ bands_spec.json # 光谱波段定义
   └─ splits.json     # 数据划分信息（可选）
