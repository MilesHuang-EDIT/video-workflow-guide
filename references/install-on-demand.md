# 按需安装入口

如果 Codex 提示缺工具，可以直接回复「请告诉我缺哪一个、影响哪一步。请先继续能完成的部分，需要代装时告诉我怎么确认」。刚开始了解项目、选规格和整理素材时，可以先走[第一次使用指南](../docs/getting-started.md)。

| 会话里提到的名字 | 它通常在哪一步用到 |
| --- | --- |
| OpenMotion | 从画面设计试做到可播放的动效样段 |
| video-shotcraft | 制作指定镜头，或继续维护已有的 Remotion 工程 |
| Agent Motion | 给一段口播做跟着讲解内容出现的画面和图解 |
| sound-effects | 给机械动作、按钮点击等配专门的声音 |
| 剪映 | 打开或继续编辑剪映草稿，验证交付的工程 |

## 基本规则

向导使用入口 `$video-workflow-guide`。安装与连接只针对本次确实需要的工具。

先决定本次路线，再检查所需工具。优先使用会话已提供的 Skill、用户指定目录或当前工程已配置的 checkout。做有限的相关路径查找。无法找到时只提示本次缺失项，保留已找到的版本和有效授权。

提示内容包括：缺什么、在本片负责什么、官方安装入口、下一步怎么继续。用户已经安装就不再推荐；同一缺失问题不重复催促。用户请求代装后，使用对应官方安装工作流；安装失败据实报告，不能说依赖已就绪。

## OpenMotion

用于从视觉参考到可播放样段的迭代，或继续已有 OpenMotion 工程。优先复用会话中的 Skill、插件和已工作的连接。缺失时指向 [OpenMotion 官方安装说明](https://github.com/nexu-io/openmotion#install)，按实际客户端选择方式。用户请求代装后按当前官方说明执行。检查能否打开和播放实际工程。需要导出时另确认渲染器及其媒体依赖。

## Agent Motion

用于口播语义动效及分配给它的人物段落。它是包含项目内 skill 的完整工程，不能只拷贝一份 SKILL.md 就宣称安装完成。

- [官方项目与下载入口](https://github.com/erduo1998-cell/agent-motion)
- [官方首次使用说明](https://github.com/erduo1998-cell/agent-motion/blob/main/docs/getting-started.md)

缺失时可以直接告诉用户：

> 这次口播包装需要 Agent Motion，目前未找到它。请从上面的官方入口安装；你也可以复制下面这句话让我协助安装，完成后继续当前视频。

可复制的请求：

> 请从 https://github.com/erduo1998-cell/agent-motion 为我安装 Agent Motion，先读它的 AGENTS.md 和官方安装说明，按其流程配置并检查环境。保留我的素材与现有工程，安装后继续当前视频任务。

其官方说明当前使用 Node22+ 和项目内 `node scripts/bootstrap.mjs`；实际执行前读取当时版本，不把本文摘要代替上游完整步骤。账号、许可和商业用途核验按所用版本处理；个人安装成功不等于公司团队、集成或再分发授权已取得。此总控不代签或扩展授权。

## video-shotcraft

用于 B-roll、网页/产品展示、教程画面及解释性动效。

- [官方项目与安装入口](https://github.com/Vincentwei1021/video-shotcraft)
- [动效样片库](https://vincentwei1021.github.io/video-shotcraft/library.html)

本机会话已提供该 skill 时直接读取真实入口。缺失时给官方项目链接与可复制请求：

> 请把 https://github.com/Vincentwei1021/video-shotcraft 安装成 Codex skill，检查实际入口及制作所需依赖，完成后继续当前视频任务。

用户要求代装时按 skill-installer 的 GitHub 安装流程执行；不静默使用浮动远端内容替换用户指定版本。实际使用时仍读取准确镜头卡、变体和 demo，不以安装完成代替镜头理解。

## sound-effects

本片确实需要制作或调整动作音效时，使用 [Barty-Bart 的 sound-effects](https://github.com/Barty-Bart/motion-graphics/blob/main/skills/sound-effects/README.md)。核对实际入口及它引用的脚本、素材清单和运行依赖。缺失时给出该官方入口，并继续可独立完成的画面工作。音效交接与验收见 [字幕、音乐与声音](motion-and-sound.md#动作音效)。

## 剪映及其他依赖

需要原生工程交付时检查目标剪映客户端。未安装或账号状态阻塞时，说明该项并引导用户使用官方客户端；不触发与本片无关的 CapCut 网页 OAuth，不索取密码或 Cookie。

Node、Python、FFmpeg、浏览器、字体等只在下游实际需要时按其工作流检查；不为了预防问题而先安装整套环境。不自动购买会员、接受协议、发布内容或修改系统安全设置。

## 回到当前任务

依赖准备完成后复用已经确认的内容、视觉与时间线，从受阻步骤继续。只验证过安装就说安装通过；只有制作、导出和客户端编辑测试实际做完，才分别确认这些结果。
