# 视频制作向导 · v0.6

把「视频制作向导」与「剪映口播与教程视频剪辑」合为一个 Codex Skill。可以从想法开始逐步制作视频，也可以直接处理已经录好的口播或教程、修改已有剪映草稿。

## 安装

在 Codex 中发送：

> 请把 https://github.com/MilesHuang-EDIT/jianying-tutorial-editing 的根目录安装为 Codex skill，安装名用 `video-workflow-guide`。

合并后只需调用 `$video-workflow-guide`。原「剪映口播与教程视频剪辑」中的精剪和可编辑工程交付都可通过这个入口使用。

## 怎么用

**从零开始**

> 用 $video-workflow-guide 帮我做一支给机械臂开发新手看的课程宣传片。我有课程网页、录屏和几段实拍，想先看几个视觉方向。

向导一次展示当前一步。可以混着发素材，已经给过的规格和选择会继续使用。整理素材、分析上传的音乐、设计动作音效和送审前的修改在后台完成。

**直接精剪或改草稿**

> 用 $video-workflow-guide 精剪这期口播。我有原视频和 SRT，去掉口误，保留原声和讲解顺序，交 MP4 和可编辑剪映项目。

> 用 $video-workflow-guide 继续剪这个剪映草稿，只调整第二章的字幕和原声音量。

向导沿用已有素材和规格，从明确的剪辑任务开始。剪映草稿可以在同一个流程里继续精剪、整理和验收。

## 交付

按项目约定交付可播放样段、成片或可编辑工程。需要剪映草稿时可以提前说明，也可以在全片定稿后决定。交付时说明哪些内容能在目标客户端继续修改，以及实际验证过的范围。

制作会按项目调用 OpenMotion、video-shotcraft 或 Agent Motion。动作音效使用 Barty-Bart 的 sound-effects。只在缺少本次需要的工具时提示安装。[按需安装入口](references/install-on-demand.md)

## 开源与依赖

本仓库的工作流与检查脚本采用 [MIT License](LICENSE)。第三方工具、字体与素材适用各自的条款。
