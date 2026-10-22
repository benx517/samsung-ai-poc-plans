# 三星 AI 产品 POC 方案集

面向内部评审的 6 个 AI + 三星产品 POC 方向，每个方向包含一份**工程技术方案**（HTML，可直接投屏）和一份**文字版描述**（Markdown，可直接贴进评审材料或邮件）。

## 六个方向

| # | 方向 | 产品载体 | 核心技术组合 | 亮点 |
|---|---|---|---|---|
| 1 | [预演引擎 Rehearsal Engine](poc-1-rehearsal-engine.html) | Galaxy S26 Ultra | 世界模型分镜生成 + 规划 + 智能体执行 | 说一句话先「预演」一遍未来再拍板，生态闭环自动就位 |
| 2 | [厨房实况教练 Kitchen Coach](poc-2-kitchen-coach.html) | AI 神冰箱 + S26 | 多模态视频理解 + 烹饪状态机 + 物理判据 | 模型只判段不发明，食品安全边界可控 |
| 3 | [家的先知 Home Guardian](poc-3-home-guardian.html) | SmartThings 全家桶 + Watch | 设备遥测 + 个人基线分位数 + 多信号印证 | 家电行为数据是竞品拿不到的壁垒 |
| 4 | [跨语言会议官 Meeting Interpreter](poc-4-meeting-interpreter.html) | S26 + Buds4 Pro + Tab | 端侧 VAD/声纹分离 + 分段翻译 + 生成式纪要 | 录音端侧留存，云端只过翻译不留痕 |
| 5 | [全屋物品记忆 Object Memory](poc-5-object-memory.html) | Jet Bot + S26 | 拍摄建库 + 视觉识别 + 位置时间线 | 只记登记物品，隐私设计最干净 |
| 6 | [现场副驾 Field Copilot](poc-6-field-copilot.html) | Galaxy Glasses（AI 智能眼镜） | 关键帧取景 + Live 会话 + 维修知识库 RAG | 唯一能直接算钱的 B2B 方向，公司自己就是客户 |

文字版：`poc-1-rehearsal-engine.md` … `poc-6-field-copilot.md`

## 行业调研

| 主题 | 文件 | 内容 |
|---|---|---|
| 国内智能眼镜 × IoT / 智能家居联动 | [HTML](research-cn-glasses-iot.html) · [Markdown](research-cn-glasses-iot.md) | 小米 / 华为 / 千问 / 雷鸟 / Rokid / INMO 等六家的联动路径与边界；L0–L3 能力模型；四条技术路径；对三星 Galaxy Glasses 的三条判断与一个 4 周 POC 建议 |

调研结论摘要：国内只有小米、华为、千问把家居联动做成了产品能力，且都停在 L1（语音遥控）；跨品牌与视觉理解仍是空白。三星不应在中国打「控制」，应打「看懂」。

## 每份方案的统一结构

1. 概念与主场景
2. 事实基线（硬件 / 平台 / 模型三段表，每项标注「对方案的影响」）
3. 组件级技术架构
4. 具体接口与参数
5. 核心算法 / 状态机
6. 数据契约（字段级，可直接建表）
7. 延迟与成本预算（P50/P90、单次调用成本）
8. 失败矩阵（触发信号 / 降级动作 / 用户看到什么）
9. 隐私与合规边界
10. 4 周计划与验收指标
11. ADR 架构决策记录（每条绑定一个事实依据，便于评审追责）

## 使用说明

- 方案页为单文件 HTML，无外部依赖，双击即可在浏览器打开投屏。
- 所有技术底座均为 2026 年已发布或已开放 API 的能力，文档中逐项标注就绪度（已开放 / 灰度需兜底 / 尚未开放）。
- 涉及未开放接口的假设已在方案中显式标注，并给出降级路径。
