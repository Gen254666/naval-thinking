# naval-thinking

A decision-making skill for DSH that applies Naval Ravikant's underlying frameworks to questions about money, economics, investing, careers, projects, business models, technology choices, and resource allocation — as a repeatable derivation process, not a quote collection.

一个用于 DSH 的思维框架 skill：把纳瓦尔·拉维坎特的底层逻辑变成可重复的推导流程，用来拆解经济、利益、投资、职业、项目、商业、技术选型与资源分配问题。它不靠引用名言，而靠一套可检验的提问顺序、判据与输出协议。

## 为什么不是"名言合集"

很多"纳瓦尔式"回答只是抛几句金句。这个 skill 的设计目标是让推导过程可复现：

- **八层拆解栈**：计量与利益结构 → 特定知识 → 杠杆 → 复利 → 判断力 → 正和/非竞争 → 时间主权与欲望 → 尾部风险。每层都有要问的问题、通过标准、红旗和常见误用。
- **硬判定规则**：五条否决项优先于总分；评分卡只用于比较选项，不制造伪精确；任何单项 0 分必须解释。
- **反内卷检验**：五个信号 + 四个替代动作，并明确"反内卷 ≠ 不努力"。
- **输出协议**：快判 / 标准 / 深度三档；每个结论必须带关键推理、否决检查、"什么情况下改变结论"、48 小时验证动作。
- **引用纪律**：区分【原话】【转述】【推演】【通用工具】；一段回答名言不超过一句，且必须紧跟推导。

## 文件结构

```
naval-thinking/
├── SKILL.md                        # 主文件：八层栈、判定规则、输出协议、场景剧本、边界
├── README.md
├── LICENSE
└── references/
    ├── sources.md                  # 概念出处、引用纪律、常见误引清单
    └── worked-examples.md          # 职业/项目/学习/资产四个完整推导样例
```

## 安装

skill 的发现规则：把整个 `naval-thinking` 目录放进 DSH 会扫描的任一 skill 根目录，确保 `SKILL.md` 位于该目录根部。

常见位置：

| 范围 | 路径 |
|---|---|
| 用户级（跨项目） | `~/.dsh/skills/naval-thinking/` |
| 用户级（共享 agent 配置） | `~/.agents/skills/naval-thinking/` |
| 项目级 | `<项目根>/.dsh/skills/naval-thinking/` |
| DSH Desktop（Windows） | `%APPDATA%\dsh-desktop\harness\skills\naval-thinking\` |

示例：

```bash
git clone https://github.com/<your-name>/naval-thinking.git ~/.dsh/skills/naval-thinking
```

Windows PowerShell（DSH Desktop）：

```powershell
git clone https://github.com/<your-name>/naval-thinking.git "$env:APPDATA\dsh-desktop\harness\skills\naval-thinking"
```

也可以直接下载 ZIP，把 `naval-thinking` 文件夹复制到上述任一目录。

## 使用

在会话中输入：

```
/naval-thinking
```

或直接说"加载 naval-thinking"。加载后，本会话内涉及金钱、收益、成本、定价、投资、职业选择、项目取舍、商业模式、技术选型、资源分配、时间与注意力配置的话题会自动套用，不需要关键词。

想停用：说"退出纳瓦尔框架 / 只要事实"。

> 说明：DSH 的 skill 是会话级加载。安装到用户级目录只保证"所有会话都能发现它"；每个新会话仍需加载一次。若要永久常驻，需要 profile 级指令（AGENTS.md 或预设）。

## 它适合什么

- 职业选择：offer 比较、转行、降薪换成长
- 项目取舍：定制 vs 产品化、自建 vs 采购
- 商业模式与定价：定价权、边际成本、留存
- 学习规划：证书 vs 作品、通用技能 vs 特定知识
- 资产与风险：期限、流动性、杠杆、尾部风险
- 技术选型与资源分配：锁定、维护成本、瓶颈
- 自我提升：时间主权、模仿性欲望、复利能力

不适合：玄学预测、具体买卖点位、替代医疗/法律/税务/合规等专业意见。硬知识先保证准确，再叠加视角。

## 设计原则

- **框架优先于语录**：正文几乎没有名言，只有推导问题、判据、否决项与输出协议。
- **可证伪**：每个结论都要求写出"什么情况下我会改变结论"。
- **边界清晰**：不做预测、不承诺收益、不替代专业意见；反对 guru 化。
- **反内卷但不反努力**：反对用增加投入替代改变结构，鼓励把努力投向学习曲线、可复用资产、信任与关键判断。
- **承认结构与运气**：不把失败简单归因于"你不够努力"或"你杠杆不够"。

## 自定义

- 改 `SKILL.md` 调整框架、权重与场景。
- 改 `description` 会改变 DSH 技能目录中的触发描述。
- 改 `references/` 增补案例或来源。
- 修改后若安装的是另一份副本，记得同步。

## 免责声明

- 本项目与 Naval Ravikant 无关，不代表其本人观点。
- 文中引用的短句版权归原作者；`references/sources.md` 标注了出处与常见误引，引用请自行核对。
- 内容仅用于思维训练与决策讨论，不构成投资、法律、税务、医疗或任何专业建议。

## License

MIT
