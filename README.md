# sz-skills · 诗中的开源能力套件

把 18 年企业服务的判断力，结晶成可安装、可直接使用的 AI skill。装上它们，等于在具体任务上"雇佣"这套判断。

作者：陈京昌（诗中）——浙江大学人工智能学院教职工、造物云 AI 联合创始人，前钉钉初创产品专家、前支付宝 AI 客服团队核心。这两年带央国企做 AI 实训与落地：云南移动 76 位业务骨干 5 周做出 7 个真实 AI 产品，国机集团结营路演 21 个落地项目，浙江移动连续 5 期复购。

现场实录与更多开源工具：[shizhong.me](https://shizhong.me)

## 为什么开源

会用 AI ≠ 做出成果。中间差的那一步是判断力：选哪个场景、怎么验证、验收标准怎么立。这些判断写成 skill 之后，边际成本为零——藏着不如给出去。方法开源，落地服务收费，这是这套仓库的商业模式，明说。

## Skills

| Skill | 干什么 | 状态 |
|---|---|---|
| [sz-diagnosis](sz-diagnosis/SKILL.md) | 央国企 AI 落地诊断：问诊（消解伪需求）+ 体检（成熟度评估，出一页纸） | v1 |

后续交付里沉淀出的通用方法论（选赛道、MVP 验证、评审打分、路演方法），会持续结晶成 `/sz-*` skill 加进来。

## 工具

- [《AI 落地诊断问卷》v1](tools/AI落地诊断问卷-v1.md) — 12 题三段（现状五问/验收三问/组织资源四问），附《落地评估一页纸》模板。10 分钟自查，答不上来的题本身就是诊断结果。

## 安装

```bash
# Claude Code / 支持 Agent Skills 的环境
git clone https://github.com/jingchang0623-crypto/sz-skills.git
cp -r sz-skills/sz-diagnosis ~/.claude/skills/
```

然后对 Claude 说「帮我看看这个 AI 项目」或 `/sz-diagnosis` 即可触发。

## 致谢与许可

- 结构声明：skill 骨架借鉴 [dbskill](https://github.com/AIGCInnovatorSpace/db-skill) 的公理层→双模式→漏斗→报告设计，内核方法论为诗中自有沉淀。开源利他这条路，dbskill 是先行者。
- 许可：[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.zh) — 随意使用、修改、分发（含商用），注明出处即可。

有类似落地诉求想找人进场：[shizhong.me/work](https://shizhong.me/work)。不需要也没关系，工具本来就是给你用的。
