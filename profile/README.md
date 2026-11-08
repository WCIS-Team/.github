<div align="center">

# WCIS-Team
https://wcis-team.github.io/WCIS-FPAI-wiki/

**2026 全国大学生嵌入式芯片与系统设计竞赛 · FPGA 创新设计赛道（FPAI）**

基于复旦微 FMQL30TAI / FPAI30TAI「悟净」开发板，探索 CPU + FPGA + NPU 异构协同的多模态边缘交互。

[![赛事官网](https://img.shields.io/badge/%E8%B5%9B%E4%BA%8B%E5%AE%98%E7%BD%91-fpgachina.cn-blue)](http://fpgachina.cn/)
[![赛道](https://img.shields.io/badge/%E8%B5%9B%E9%81%93-FPAI-2DA44E)](http://fpgachina.cn/)
[![目标平台](https://img.shields.io/badge/%E7%9B%AE%E6%A0%87%E5%B9%B3%E5%8F%B0-FMQL30TAI%C2%B7%E6%82%9F%E5%87%80-8250DF)](https://github.com/WCIS-Team/WCIS-FPAI-wiki)

</div>

## 参赛作品（上交项目）

**[fmql30tai-sdi-npu-face-recognition](https://github.com/WCIS-Team/fmql30tai-sdi-npu-face-recognition)** —— FMQL30TAI 平台上的 **SDI 视频采集 + NPU 人脸识别**工程：板端安装器、PS/NPU 应用源码、FPGA 源（自研 RTL）与构建复现记录。

| 环节 | 模型 | 上游 |
|---|---|---|
| 人脸检测 | YuNet | [OpenCV Zoo](https://github.com/opencv/opencv_zoo) |
| 特征比对 | MobileFaceNet | [InsightFace](https://github.com/deepinsight/insightface) |
| 活体防伪 | MiniFASNet 双模型 | [MiniVision Silent-Face-Anti-Spoofing](https://github.com/minivision-ai/Silent-Face-Anti-Spoofing) |

> 本仓库为公开源码版：厂商受限资源与完整安装载荷不随 Git 分发，边界与第三方许可见仓库 [README](https://github.com/WCIS-Team/fmql30tai-sdi-npu-face-recognition#readme) 与 [THIRD_PARTY_NOTICES](https://github.com/WCIS-Team/fmql30tai-sdi-npu-face-recognition/blob/main/THIRD_PARTY_NOTICES.md)。

旧PS控制中心 https://github.com/WCIS-Team/HA4FPAI/tree/archive-2026-11-06

## 主要仓库

| 仓库 | 简介 |
|---|---|
| [WCIS-FPAI](https://github.com/WCIS-Team/WCIS-FPAI) | 参赛工程主仓库：FMQL30TAI 多模态边缘 AI 终端的源码、文档与 wiki（参赛作品源仓库） |
| [HA4FPAI](https://github.com/WCIS-Team/HA4FPAI) | 板载语音控制栈：不装 Home Assistant 本体，sherpa-onnx 语音链 + Rust NLU（klar）+ 自建执行器，开发板既是控制器也是被控设备 |
| [WCIS-FPAI-wiki](https://github.com/WCIS-Team/WCIS-FPAI-wiki) | 文档库与目录导航：工程路线、状态源与验证边界 |
| [Qwen3-0.6B4icraft430tai](https://github.com/WCIS-Team/Qwen3-0.6B4icraft430tai) | Qwen3-0.6B 移植到 iCraft 30TAI（ZG330/FMQL30TAI）：图重写、编译脚本、板端驱动与实测 |
| [ERNIE-4.5-0.3B-PT4icraft430tai](https://github.com/WCIS-Team/ERNIE-4.5-0.3B-PT4icraft430tai) | ERNIE-4.5-0.3B-PT 移植到 iCraft 30TAI（ZG330） |
| [Qwen2_0.5B_zg3.36.1_axi_demo](https://github.com/WCIS-Team/Qwen2_0.5B_zg3.36.1_axi_demo) | 厂商 Qwen2-0.5B demo 镜像（iCraft 3.36.1），并入我方板端部署改动 |
| [mddocs-path-i18n](https://github.com/WCIS-Team/mddocs-path-i18n) | Markdown 目录树的路径级本地化：翻译文件与目录名，并修复全部链接 |
| [WCIS-FPAI-repos](https://github.com/WCIS-Team/WCIS-FPAI-repos) | WCIS 归档根 |

## 赛事信息

- **赛事**：2026 全国大学生嵌入式芯片与系统设计竞赛
- **赛道**：FPGA 创新设计赛道（FPAI）
- **官网**：<http://fpgachina.cn/>
- **目标平台**：复旦微 FMQL30TAI / FPAI30TAI「悟净」开发板（CPU + FPGA + NPU）
