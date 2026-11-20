# Vision Model Library

这里收录面向不同游戏画面的视觉模型权重，可用于计算机视觉学习、离线录像分析和边缘设备推理评估。每个版本都有固定下载链接和 SHA-256 校验值。

Curated computer vision weights for offline evaluation and edge inference. The catalog provides downloads, input shapes where available, and validation status.

## 推荐起点

| 画面 | 格式 | 文件 | 推荐依据 |
| --- | --- | --- | --- |
| CS2 | RKNN | [下载](https://github.com/pooh8964xi-cyber/vision-model-library/releases/download/v0.1.0/cs2-team-v5-rk3588.rknn) | 匹配 RK3588 参考设备曾验证的模型摘要 |
| CS2 | ONNX | [下载](https://github.com/pooh8964xi-cyber/vision-model-library/releases/download/v0.1.0/cs2-v8-320-cs2-320-50268e923fa5.onnx) | ONNX Runtime CPU 已通过一次 320 × 320 离线样例推理 |
| VALORANT | ONNX | [下载](https://github.com/pooh8964xi-cyber/vision-model-library/releases/download/v0.1.0/valorant-7-wa-v26s-320x-281cf383b9f5.onnx) | ONNX Runtime CPU 已通过一次 320 × 320 离线样例推理 |
| 穿越火线 | ONNX | [下载](https://github.com/pooh8964xi-cyber/vision-model-library/releases/download/v0.1.0/crossfire-7-cfv26s-320x-1f03e936398e.onnx) | ONNX Runtime CPU 已通过一次 320 × 320 离线样例推理 |

## 浏览模型

首版 v0.1.0 收录 101 个独立权重，覆盖 23 个目录分类。

- [按类别浏览全部下载](MODELS.md)
- [机器可读目录](catalog.json)提供固定版本 URL、文件大小、校验值和已知输入信息。
- [版本附件](https://github.com/pooh8964xi-cyber/vision-model-library/releases/tag/v0.1.0)提供权重、目录快照和 SHA-256 清单。

## 格式与验证

- **ONNX** 可用 ONNX Runtime 检查输入和输出。标为「离线样例」的版本已在 CPU 上以零值输入跑通一次。
- **RKNN** 需要与模型匹配的 Rockchip 芯片及运行时。标为「参考设备」的条目有设备验证记录，其余条目仅核过文件格式。
- **PyTorch .pt** 为归档检查点，已核查容器格式。离线推理可以从 ONNX 开始。

## 使用说明

这些模型面向学习和本地离线研究。请遵守适用的游戏和赛事规则。游戏名用于标识模型适用的画面。模型保留原有权利和许可信息，详见[来源及许可说明](MODEL_TERMS.md)。
